Get |galaxy_vm|
===============

The |galaxy_vm| section allows user to deploy a standard `Galaxy production environment <https://docs.galaxyproject.org/en/latest/admin/production.html>`_.

The service instantiate a CentOS 7 Virtual Machine with Galaxy, all its companion software and tools already embedded. Once deployed each Galaxy instance can be further customized with tools and reference data.

.. seealso::

   For a detailed descreption of all Web UI options see section: :doc:`feat_options`.

.. seealso::

   To login into the portal see section: :doc:`feat_auth`.

Instantiate Galaxy
------------------

#. Enter in the |galaxy_vm| section:

   .. figure:: _static/qs_galaxy_vm/qs_galaxy_main.png
      :scale: 70 %
      :align: center
      :alt: Galaxy express main window

#. Describe your instance using the ``Instance description`` field, which will identfy your Galaxy in the job list, once your request is submitted.

#. Select the Instance flavor, (virtual CPUs and RAM):

   Currently, the following pre-sets are available, but not all of them are enabled.

   =========  =======  =======  =============  =============
   Name       VCPUs    RAM      Total Disk     Root Disk
   =========  =======  =======  =============  =============
   small      1        2 GB     20 GB          20 GB
   medium     2        4 GB     20 GB          20 GB
   large      4        8 GB     20 GB          20 GB
   xlarge     8        16 GB    20 GB          20 GB
   xxlarge    16       32 GB    20 GB          20 GB
   =========  =======  =======  =============  =============

#. Copy & Paste your SSH key, to login in the Galaxy instance:

   .. figure:: _static/qs_galaxy_vm/qs_galaxy_SSHkey.png
      :scale: 50 %
      :align: center
      :alt: SSH public key injection

#. Storage section allows to select the user storage volume size. The ``Enable encryption`` flag is explained here: :doc:`qs_encryption`.

   .. figure:: _static/qs_galaxy_vm/qs_galaxy_Storage.png
      :scale: 50 %
      :align: center
      :alt: Galaxy express Storage section

#. Select the Galaxy version, the instance administrator e-mail and your custom Galaxy:

   .. figure:: _static/qs_galaxy_vm/qs_galaxy_GalaxyConfig.png
     :scale: 50 %
     :align: center
     :alt: Galaxy express Galxy configuration section

  .. Warning::

     Please insert a vail mail address. No check is performed on its syntax, but entering an incorrect email address will cause deployment failure if the ``encryption`` option is set.

#. Select Galaxy tools pre-set:

   .. figure:: _static/qs_galaxy_vm/qs_galaxy_Tools.png 
      :scale: 50 %
      :align: center
      :alt: Galaxy express Tools section

#. and reference dataset:

   .. figure:: _static/qs_galaxy_vm/qs_galaxy_refdata.png 
      :scale: 50 %
      :align: center
      :alt: Galaxy express Tools section

#. Finally, ``SUBMIT`` your request:

   .. figure:: _static/qs_galaxy_vm/qs_galaxy_view.png
      :scale: 50 %
      :align: center
      :alt: Galaxy express submit request

Galaxy login
------------
The galaxy administrator password is automatically generated during the instatiation procedure and is the same for each deployed instance:

::

  User: galaxy administrator e-mail

  Password: galaxy_admin_password

.. Warning::

   The anonymous login is by default disabled.

.. Warning::

   Change Galaxy password and the API key as soon as possible!
