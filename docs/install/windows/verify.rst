
Verification
--------------------------------------

Verify that your installation is successful by following these steps:

1. Open PowerShell by opening the menu bar, then search for :menuselection:`Windows PowerShell`.
   Verify that ``(base)`` is shown to the left of the
   text.
   Something like the image below:

   .. card::

      .. image:: /os/gifs/PS/conda-check-base.gif
         :width: 100% 
         :align: center

2. Type ``idle`` in the Powershell window, then press :kbd:`Enter`.
   This should open a new window in which you can run Python code.

3. Verify the :guilabel:`IDLE` window says ``Python {{ python_version }}.X``
   in the top left
   (or in the range of {{python_version_min}} -- {{python_version_max}}).

4. Copy the following Python code into the :guilabel:`IDLE` window, then press :kbd:`Enter`:

   .. code:: python

      import dtumathtools, pandas, scipy, statsmodels, uncertainties

   Verify that a new line (``>>>``) appears without any text (indicating everything got imported correctly).
   See the below image for an example:

   .. card::

      .. image:: /images/install/windows-IDLE-import.png
         :width: 100% 
         :align: center

If some steps result in a different than described above, please continue reading the Troubleshooting section.


Troubleshooting
^^^^^^^^^^^^^^^^

Only follow these troubleshooting steps if something in the previous section did not check out.

* Ensure that Miniconda is installed:
  Search for the ``Anaconda Powershell`` prompt (it will say ``Anaconda Powershell Prompt (Miniconda3)``)
  on your computer and open it up.

  If you cannot find it, press :ref:`here to install Miniconda <install-python-windows-conda>`.

* After opening the Anaconda Powershell, type ``conda init`` and press :kbd:`Enter`.

* Ensure the packages are installed (if they are already installed, this will not do anything).

  Paste the following line of code to the PowerShell window and press :kbd:`Enter`:

  .. code:: pwsh

     conda install python={{ python_version_recommended }} dtumathtools pandas scipy statsmodels uncertainties -y


* Go back to the previous Verification section and check them again.

If you are still having trouble or have any questions, please do not hesitate to visit us during office hours
or contact us via :mail:`email <pythonsupport@dtu.dk>`
or `Discord <ps-discord-invite_>`_.
More information can be found on our :ref:`homepage <reach-us-reference>`.

