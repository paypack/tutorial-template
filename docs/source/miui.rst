#################
Troubleshoot MIUI
#################

Error notification
==================
"find device storage corrupted your device is unsafe now"

This means your persist.img is corrupted. Restoring your persist.img will patch this damage. There are several ways for you to restore persist.img.

.. code-block:: cmd

    fastboot %* flash persist "%~dp0images\persist.img" || @echo "Flash persist error" && exit /B 1

Add this line to your fastboot ROM bat file before flashing.

Long Term Support
=================

Each major Linux Mint release is supported for 5 years.


.. note:: Make sure you have backed up your data before starting this step.