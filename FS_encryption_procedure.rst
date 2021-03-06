Storage encryption procedure
============================

To encrypt the Virtual machine external volume follow this procedure.

Virtual Machine login
---------------------

Log-in into your machine with:

``ssh -i your_private_ssh_key.key galaxy@virtual.machine.ip.address``

.. figure:: _static/encryption/FS_ecrypt_proc_01.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 01

Typical IP addresses are: ``90.147.170.xx``, ``90.147.102.xx`` or ``90.147.75.xx`` and it is reported in the e-mail we sent you. You can copy and past the command from the mail the system send you.

.. figure:: _static/encryption/FS_ecrypt_proc_02.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 02

Probably, you have to permanently accept the connection, typing “yes”.

.. figure:: _static/encryption/FS_ecrypt_proc_03.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 03

and then enter your SSH passphrase.

.. figure:: _static/encryption/FS_ecrypt_proc_04.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 04

Passphrase creation
-------------------
You will be now prompted in the encryption script automatically.
You will be required to insert an alphanumeric key, at least 8 characters.
A key is automatically generated, as example, plase do not use if for production!

You have to type your password three times:

#. | inject your password

#. | Confirm your password

#. | Unlock your encrypted volume

Insert your volume encrypt/decrypt password for the first time:

.. figure:: _static/encryption/FS_ecrypt_proc_05.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 05

and confirm it:

.. figure:: _static/encryption/FS_ecrypt_proc_06.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 06

If the passphrases don't match, restart the procedure.

Unlock the volume
-----------------

Unlock the encrypted volume typing again your password:

.. figure:: _static/encryption/FS_ecrypt_proc_07.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 07

The volume will be now encrypted and you will be automatically log-out the VM, until Galaxy is installed.

.. figure:: _static/encryption/FS_ecrypt_proc_08.png
   :scale: 70 %
   :align: center
   :alt: encrypt procedure 08
