 .. note:: We are currently moving the documentation to a new platform. Please visit `Trezor Wiki <https://wiki.trezor.io/User_manual:Two-factor_Authentication_with_U2F>`_ for the latest version of this page.

Two-factor Authentication with U2F
==================================

.. image:: images/u2f.png

Two-factor authentication (2FA) is currently the most common way how you can protect your online accounts from unauthorized access. In addition to what you know (your username and password), you use something that only you have — a phone, an app or a specialized hardware token, in order to login securely.

However, some methods of 2FA are inherently insecure. The most popular 2FA implementation, Time-based One-Time Password (TOTP), popularized by its use on Google Auth services, transmits the shared secret (master key) over the internet during the setup process. This weakness has been recognized by major players who created FIDO Alliance and defined new, more secure standards such as U2F.

Starting with firmware 1.4.0, TREZOR officially supports the U2F specification. After updating your device firmware, you can start using TREZOR as your 2nd factor authentication token with services such as Google or Dropbox. Check out services using U2F at dongleauth.info.

One further improvement of TREZOR on top of U2F is that TREZOR users can truly verify what they are about to authorize via the on-device display.

.. note:: You can find a list of websites which support U2F at `dongleauth.info <http://www.dongleauth.info/>`_.

How to Setup TREZOR as a U2F key?
---------------------------------

In this short tutorial, we will use Dropbox as the example, however, all services should have a similar setup procedure.

1. In Settings, click on ‘Add’ to setup TREZOR as your U2F Security Key

.. image:: images/u2f-dropbox1.png


2. Plug in your TREZOR

.. image:: images/u2f-dropbox2.png


3. Wait for the prompt on your TREZOR

.. image:: images/u2f-dropbox3.png


4. Confirm after checking

.. image:: images/u2f-dropbox4.jpg


5. Done! You can start using TREZOR to log into Dropbox alongside with a simple password.

.. image:: images/u2f-dropbox5.png


Using TREZOR as a U2F Key
-------------------------

We are using GitHub as an example, but all services should have similar login procedures.


1. Log in as usual

.. image:: images/u2f-github1.png


2. Plug in TREZOR

.. image:: images/u2f-github2.png


3. The device will not ask you for your PIN. Your login credentials for the service serve as the first factor. Your TREZOR as the second factor.

.. image:: images/u2f-github3.jpg


Restoring U2F Counter on TREZOR
-------------------------------
Restoring a seed on another TREZOR restores all the U2F keys too, as they are derived from one master key. However, due to the design of U2F, some services might implement a **counter** that records the number of sign-ins. When recovering a seed, or cloning a TREZOR, this counter will be off and might have to be **increased**, in order for the recovered TREZOR to work successfully with a service.

.. note:: If you have firmware from version 1.4.2 and higher, U2F counter will be restored automatically on Wallet Recovery. Simply restore your wallet, and the U2F counter will be set to the UNIX time at the moment of recovery.

You can increase the counter manually with `python-trezor <https://github.com/trezor/python-trezor>`_:

``trezorctl set_u2f_counter $(date +%s)``

This command will increase the counter to the current UNIX time. (As long as the counter is higher than the one recorded on provider’s side, login will be successful.)

Relevant discussion: `Reddit Thread <https://www.reddit.com/r/TREZOR/comments/50h8r9/new_trezor_firmware_fidou2f_and_initial_ethereum/d74iw3b/>`_.
