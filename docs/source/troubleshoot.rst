#################
Troubleshoot MIUI
#################

Error notification
==================
"find device storage corrupted your device is unsafe now"

This means your persist.img is corrupted. Restoring your persist.img will patch this damage. There are several ways for you to restore persist.img.

.. note:: Make sure you have backed up your data before starting this step.
    
.. code-block:: bash

    fastboot %* flash persist "%~dp0images\persist.img" || @echo "Flash persist error" && exit /B 1

Add this line to your fastboot ROM bat file before flashing.