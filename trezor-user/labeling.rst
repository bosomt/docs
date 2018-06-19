 .. note:: We are currently moving the documentation to a new platform. Please visit `Trezor Wiki <https://wiki.trezor.io/User_manual:Labeling>`_ for the latest version of this page.

Labeling
========

By connecting TREZOR Wallet with Dropbox cloud storage, you can enjoy all these useful features:

- **Rename accounts**
- **Label receiving addresses**
- **Comment transactions**

This is a great way to organize your bitcoin wallet and keep a memory of your transaction activity.
Moreover, all your private data are ultimately secured and easily available from any computer. All the information you add is automatically **encrypted by a key derived from your TREZOR device** and uploaded to your personal Dropbox folder.

.. image:: images/labeling-example.png

Set up labeling: Connect Dropbox with your TREZOR
-------------------------------------------------

1. Click on the Dropbox icon in the top of the TREZOR Wallet screen.

.. image:: images/labeling-connecttodropbox.png

2. Click on the **Continue** button in a pop-up window that appears.

.. image:: images/labeling-connecttodropbox2.png

3. Log into your Dropbox account. If you don't have any, create one, it’s free.

.. image:: images/labeling-dropboxlogin.png

.. important:: When you log into your Dropbox account, there is a session cookie on Dropbox server with access to TREZOR Wallet folder valid for about 5 years! We recommend to log out of your Dropbox account manually after you finish working with TREZOR Wallet or use a Private window in your browser for the best possible privacy.

4. Once logged in, TREZOR will ask for your permission to create a folder in your Dropbox where all the labels will be stored.

.. image:: images/labeling-dropboxapproval.png

5. Finally, enable labeling on your TREZOR device. This will encrypt the files with your private key derived from your TREZOR.

.. image:: images/labeling-allowlabeling.png

Congratulations! You are ready to use TREZOR Labeling.


Rename Accounts
---------------

Hover over the Account name area and click on the **tag icon**, enter a new account name and confirm by hitting the **Save icon**.

.. image:: images/labeling-account1.png
.. image:: images/labeling-account1a.png


Label receiving addresses
-------------------------

Labeling receiving addresses helps you identify incoming payments easily. You can label previously used addresses as well as the new ones and assign them to a specific purpose.  Simply type your label into the field next to the freshly created address and hit the **Save icon**.

.. image:: images/labeling-receive.png

Whenever someone sends you a payment to an address that you labeled “For cleaning”, you will see this label in your Transactions history.


Comment transactions
--------------------

Adding comments when sending transaction helps you keep track of your expenses.
Let’s say you want to send money to two separate addresses (Alice and Bob) in one transaction. You can add a comment to every single address (output).

.. image:: images/labeling-send.png

When you switch back to the “Transactions” tab, you will see one transaction with two commented addresses (outputs). You can change each of the comments separately.

.. image:: images/labeling-transactions2.png


How do TREZOR and Dropbox work together?
----------------------------------------

If you are interested how it works in the background, it's actually quite simple! TREZOR Wallet will create a folder "/Apps/TREZOR/" in your Dropbox and store labels for each TREZOR account in a separate file. You can back up those files and use them to restore all the labels in case you lose access to your Dropbox account!

Files are encrypted with AES-256 using a private key derived from your TREZOR for this single purpose. It's also not possible to use Dropbox to reveal your payment history, your actual account balance or to rebuild your recovery seed!
