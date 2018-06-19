 .. note:: We are currently moving the documentation to a new platform. Please visit `Trezor Wiki <https://wiki.trezor.io/FAQ:Overview>`_ for the latest version of this page.

Product Overview
================

What is TREZOR?
---------------

TREZOR is a single purpose device which allows you to make secure Bitcoin transactions. With TREZOR, transactions are completely safe even when initiated on a compromised or vulnerable computer.  Because the use of TREZOR is very easy and intuitive we believe it will help Bitcoin adoption among people not familiar with the security issues.

.. image:: images/trezor_transparent.png


How does TREZOR work?
---------------------

The Bitcoin protocol works by sending signed notes of payment across the Internet. These messages (which are referred to as Transactions) are signed using a special algorithm. In order to sign a Bitcoin transaction, you need to have a special key or password. TREZOR holds that key. Since TREZOR's job is to help you securely sign Transaction messages, you can think of your TREZOR as a modern-day stamp.

.. image:: images/stamp.jpg

(image credit  `Petr Kvashin <http://www.publicdomainpictures.net/view-image.php?image=038943>`_)

TREZOR is better than an ordinary mechanical stamping mechanism, however. Each TREZOR has a PIN code. If your TREZOR gets stolen, thieves cannot misuse it to steal your money. Due to TREZOR's clever design, even if the computer with which you use your TREZOR is hacked, the hackers will never know your PIN.

In contrast to the various pieces of software and web services that allow you to store your Bitcoins TREZOR is secure. Software and web-based solutions keep your Bitcoin signing keys either on your computer or worse, on the Internet! When you use such a service, hackers can easily steal your Bitcoins by hacking your computers or hacking the servers of the services that you use.


Which operating systems and devices support TREZOR?
---------------------------------------------------

There is full support for Windows (version 7 and higher), OS X (version 10.11 and higher) and Linux. You can also use your TREZOR with Android devices which have USB On-The-Go (aka USB Host).

Which browsers are currently supported by TREZOR wallet?
---------------------------------------------------

The major supported browsers are Chrome and Firefox. The other browsers may be usable but we can't guarantee a full functionality.

Which wallets are compatible with TREZOR hardware?
--------------------------------------------------

The list of wallets that can be used with TREZOR device is constantly growing. These include
`TREZOR Wallet <../trezor-apps/trezorwallet.html>`_ or
`Mycelium <../trezor-apps/mycelium.html>`_.
To see the full list, please check out our `TREZOR Apps <../trezor-apps/index.html>`_.

Which wallets are compatible with TREZOR recovery seed?
-------------------------------------------------------

In case your TREZOR is not available you can still recover your bitcoins using your :download:`recovery seed <../trezor-user/images/recovery_card.pdf>`
and a compatible wallet like
`Mycelium <https://play.google.com/store/apps/details?id=com.mycelium.wallet>`_ or
`Electrum <https://electrum.org/#download>`_.
Check out our `TREZOR Apps <../trezor-apps/index.html#recovering-funds-without-trezor-device>`_ for the full list of wallets compatible with the recovery seed.


Which wallets or services can import TREZOR account public keys (xpub)?
-----------------------------------------------------------------------

There is a growing number of wallets and online services, which you can use to **watch your TREZOR account balances** or **receive bitcoins directly into your TREZOR** without connecting the device.
These apps cannot spend your coins but can check balances online or generate new receiving addresses for you.

To find out more about these apps, please look for wallets and services with "Watch-only mode" feature icon :icon:`eye-slash` in `TREZOR Apps <../trezor-apps/index.html>`_

Which coins are currently supported?
------------------------------------

At this moment it is Bitcoin, Litecoin, Dash, Zcash, Bitcoin Cash, Bitcoin Gold, Ethereum (+ all ERC-20 tokens), Ethereum Classic, Expanse, UBIQ, NEM, Namecoin, Dogecoin and Bitcoin Testnet.

================================= =========================================================
Wallet Interfaces for TREZOR by Currency
-------------------------------------------------------------------------------------------
Bitcoin (BTC)                     `TREZOR Wallet <../trezor-apps/trezorwallet.html>`_
Litecoin (LTC)                    `TREZOR Wallet <../trezor-apps/trezorwallet.html>`_
DASH                              `TREZOR Wallet <../trezor-apps/trezorwallet.html>`_
Zcash (ZEC)                       `TREZOR Wallet <../trezor-apps/trezorwallet.html>`_
Bitcoin Cash / Bcash (BCH)        `TREZOR Wallet <../trezor-apps/trezorwallet.html>`_
Bitcoin Gold (BTG)                `TREZOR Wallet <../trezor-apps/trezorwallet.html>`_
Ethereum (ETH)                    `MyEtherWallet <../trezor-apps/mew.html>`_
Ethereum Classic (ETC)            `MyEtherWallet <../trezor-apps/mew.html>`_
ERC-20 Tokens                     `MyEtherWallet <../trezor-apps/mew.html>`_
Expanse (EXP)                     `MyEtherWallet <../trezor-apps/mew.html>`_
UBIQ (UBQ)                        `MyEtherWallet <../trezor-apps/mew.html>`_
NEM (XEM)                         NEM Nano Wallet
Namecoin                          No interface
Dogecoin                          No interface
Bitcoin Testnet                   Custom TREZOR Wallet
================================= =========================================================

Please check the `TREZOR Apps <../trezor-apps/index.html>`_ for detailed information about the wallets supporting TREZOR
