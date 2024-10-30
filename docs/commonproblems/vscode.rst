.. _vscodeproblems:

Common Problems with Visual Studio Code
==========================================

Here you'll find fixes for some common problems with VS Code. 


.. dropdown:: EPERM: Operation Not Permitted

    This error occurs when your folder is in restricted mode, when you do not have access to the folder or when the folder is not trusted. To fix this:

    1. Check if the folder is in restricted mode. If it is, change the permissions.

    2. Check if you have access to the folder. If you do not, ask the owner for access.

    3. Check if the folder is trusted. If it is not, make sure that VS Code is allowed to access the folder.




.. dropdown:: "Module not found... "


    This error occurs when you either have not installed the module or when the module is installed in a different environment. To fix this:

    1. Try to import the module in another environment (see :ref:`here <learn-more-vscode-script-select-interpreter>`).

    2. If the module is not installed, install it using the command ``conda install module_name``.


.. dropdown:: Missing "Run and debug" in Python files

    This error occurs when you have not installed the Python extension. To fix this:

    1. Install the Python extension by clicking on the Extensions icon in the Activity Bar on the side of the window, searching for Python, and clicking on the Install button.

    2. If it still does not work, right-click on the three dots in the upper right corner next to where the run and debug button normally is. Then make sure that the run and debug have a checkmark.

    .. image:: /commonproblems/images/Run-and-debug.png
        :alt: Run and Debug
        :align: center
        :width: 400px


