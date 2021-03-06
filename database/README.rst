Installation
============

Clone this repository.

.. code-block:: bash

	git clone git@github.com:holatuwol/liferay-faster-deploy.git

Make sure that you've got all the prerequisite binary tools and Python packages:

* `Initial Setup <../SETUP.rst>`__

Then, add this section to ``.bash_aliases`` (or the equivalent on whichever shell you're using) which calls the script, making sure to change ``/path/to/clone/location`` to wherever you cloned the repository:

.. code-block:: bash

	MCD_RD_CLONE_PATH=/path/to/clone/location

	mysql() {
		DRIVERS_FOLDER=/path/to/jdbc/drivers \
			${MCD_RD_CLONE_PATH}/database/mysql
	}

	oracle() {
		DRIVERS_FOLDER=/path/to/jdbc/drivers \
			${MCD_RD_CLONE_PATH}/database/oracle
	}

	sybase() {
		DRIVERS_FOLDER=/path/to/jdbc/drivers \
			${MCD_RD_CLONE_PATH}/database/sybase
	}