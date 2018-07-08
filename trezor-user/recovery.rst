 .. note:: We are currently moving the documentation to a new platform. Please visit `Trezor Wiki <https://wiki.trezor.io/User_manual:Recovery>`_ for the latest version of this page.

Recovery
========

What happens if I forget my PIN?
--------------------------------

If you forget your PIN, you can reset it by wiping your TREZOR :doc:`in advanced settings<advanced_settings>` and using the recovery process described below.

Recovery process
----------------

If you lose your TREZOR or if your TREZOR somehow gets destroyed you may have to recover your accounts.  As long as your recovery card is intact and secured, your bitcoins are safe and sound.

What do you need to start your TREZOR recovery:

 - A new or :doc:`wiped<advanced_settings>` TREZOR
 - Your recovery seed
 - A computer with the TREZOR bridge installed

To start your TREZOR recovery, plug your new TREZOR into your computer and go to `TREZOR Wallet <https://wallet.trezor.io>`_.  You should be presented with two options -to either "Create a new wallet" or "Recover wallet". Simply click on the "Recover wallet" button.

First of all, TREZOR will ask you how long is your recovery seed. Select the correct number and then you will be asked to enter the words in their correct order, as displayed on the screen. 

If you are using TREZOR T, the recovery seed words are entered entirely on the device through the touchscreen. Therefore, any leak of sensitive data to a potentially insecure browser or computer is avoided. 

During the standard recovery process with TREZOR One, you will be entering the seed words on your computer. However, you can reach the same security level as with TREZOR T by enabling the  `Advanced Recovery <https://doc.satoshilabs.com/trezor-user/advancedrecovery.html>`_, which uses the on-screen input to load your recovery seed.

.. image:: images/trezor-recovery.jpg

Once you've successfully recovered your TREZOR Wallet, you can name your device and set-up a new PIN. It is important to finish the set-up since freshly recovered wallet is not protected with your old PIN by default. 

If there was a passphrase enabled on your previous device, go to the "Advanced" settings tab and check the box to enable passphrase encryption. Once you re-connect the device, a box will appear where you can type in the passphrase.
