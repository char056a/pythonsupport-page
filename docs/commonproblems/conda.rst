.. _condaproblems:

Common Problems with Conda and Packages
========================================

Here you'll find fixes for some common problems related to conda, environments and packages. 

.. dropdown:: Incompatible Architecture

    This is common when switching computers and transferring files through one drive and icloud.
    The solution is the same on MacOS, Linux and Windows:

    .. code-block:: bash
        
        conda install --upgrade --force-reinstall <package>


.. dropdown:: "Module not found... " or "No Module Named"

    If you have not previously installed the package the solution is to open your `Terminal` and write:

    .. code-block:: bash
        
        conda install <package>


.. dropdown:: "Module not found" - when you've installed the module

    If you have installed the package before, you need to change your kernel.
    If you are using a `Jupyter Notebook` you have to go to the to right corner, where it says `Python 3.XX.XX` (this is the python version you are using). You need to click on it, after which a dropdown will come down.
    Here you need to click `Select Another Kernel...` -> `Python Environments` -> `base (Python 3.11.XX)`.
    This will open the Python downloaded using our installation guides.

    If you are using a normal Python script, go to the bottom right corner. Her it will only show the Python version, for example `3.12.XX 64-bit`. You need to click this, after which a dropdown will come down. Here you can see your Python versions. If you want to use the version installed using our guides, select `Python 3.11.XX ('base')`. 


.. dropdown:: Sympy pretty print not functioning properly

    When using sympy and the printing does not work after writing:

    .. code-block:: python

        import sympy as*
        init_printing()

    Most of the cases can be solved by wrinting the following in stead:

    .. code-block:: python

        import sympy as*
        init_printing(use_latex='mathjax')


.. dropdown:: Multiple conda installations

    If you have multiple installations of conda we highly recommend that you uninstall Anaconda using `this link <https://pythonsupport.dtu.dk/uninstall/conda.html>`__ .



