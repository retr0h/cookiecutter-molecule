*******
Install
*******

This set of playbooks have specific dependencies on Ansible due to the modules
being used.

Requirements
============

* Docker Engine

Install OS dependencies on CentOS 7

.. code-block:: bash

  $ sudo yum install -y epel-release
  $ sudo yum install -y gcc python-pip python-devel openssl-devel
  # If installing Molecule from source.
  $ sudo yum install libffi-devel git

Install OS dependencies on Ubuntu 16.x

.. code-block:: bash

  $ sudo apt-get update
  $ sudo apt-get install -y python-pip libssl-dev docker-engine
  # If installing Molecule from source.
  $ sudo apt-get install -y libffi-dev git

Install OS dependencies on Mac OS

.. code-block:: bash

  $ brew install python
  $ brew install git

Install using pip:

Please refer to the `Virtual environment`_ documentation for installation best
practices. If not using a virtual environment, please consider passing the
widely recommended `'--user' flag`_ when invoking ``pip``.

.. _Virtual environment: https://virtualenv.pypa.io/en/latest/
.. _'--user' flag: https://packaging.python.org/tutorials/installing-packages/#installing-to-the-user-site

.. code-block:: bash

    $ pip install 'molecule[docker]'