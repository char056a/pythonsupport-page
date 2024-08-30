.. _automated-reference-macos:


{{ apple_icon }} --- Automated Installation
============================================

.. button-ref:: ../windows/automated
   :ref-type: doc
   :align: right
   :color: primary
   
    Press here for Windows {{ windows_icon }}


.. dropdown:: {{ video_install }}
    :open:
    :color: info

    .. raw:: html

       <iframe src="https://panopto.dtu.dk/Panopto/Pages/Embed.aspx?id=d6e006c1-7b71-4f49-bced-b1d8013632d8" height="405" width="640" style="border: 1px solid #464646;" allowfullscreen allow="autoplay"></iframe>


Install everything at once
---------------------------------------------------

.. card::

   Installs all packages and tools required for the 1\ :sup:`st` year
   Polytechnical Foundation courses at DTU. 

   #.    
      Search for :menuselection:`Terminal` using your Spotlight search (:kbd:`Command+Space`) and press :kbd:`Enter`.

       .. image:: /images/install/MacOS-SpotlightSearch-Terminal.png
          :width: 100%
          :align: center

   #.
       Paste the following code into your Terminal and press :kbd:`Enter`.
       You might get asked for permissions.
       Please do this, note that your password will not be shown while typing it. 

       .. code:: bash

          /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/dtudk/pythonsupport-scripts/main/MacOS_AutoInstall.sh)"

       .. include:: /_rst_includes/tip-copy.rst

   #.
       Follow the script instructions.

       The script has finished when you see something like:

       .. code:: bash

          Script has finished. You may now close the terminal...

       Now, Python and Visual Studio Code will be ready to use.

       .. note::

          During the installation, you will see warnings and caveats, etc.
          The script will resolve these automatically.
          Please let the script finish.


.. include:: /_rst_includes/tip-finish.rst

.. include:: verify.rst
