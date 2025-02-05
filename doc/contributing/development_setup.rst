.. _development_setup: 

Development Setup
=================

Requirements
------------

Currently supported: Python Versions 3.8 - 3.13

- Tested under Ubuntu 20.04 with Poetry 1.4.0 and Python 3.10.12
- Tested under Windows 11 running WSL2 with Poetry 1.5.1 and Python 3.10.6 
- Tested under Windows 11 native with Poetry 1.5.1 and Python 3.10.6

Installation Steps
------------------

1. **Poetry Installation**

   To install Poetry, follow the official installation instructions found at
   `Poetry Installation <https://python-poetry.org/docs/#installation>`_.

2. **Navigate to the Project's Root Directory**

   Open your terminal and navigate to the root directory of your project:

   .. code-block:: shell

      cd /path/to/your/project

3. **Create a Virtual Environment**

   Run the following command to create a virtual environment using Python 3.10:

   .. code-block:: shell

      poetry env use python3.10

4. **Activate the Virtual Environment**

   Activate the virtual environment by running:

   .. code-block:: shell

      poetry shell

5. **Update poetry.lock File**

   Ensure the **poetry.lock** file is up-to-date with the **pyproject.toml** file by running:

   .. code-block:: shell

      poetry lock --no-update

6. **Install Project Dependencies**

   Install the project dependencies using Poetry:

   .. code-block:: shell

      poetry install

7. **Install Git Pre-commit Hook**

   Install a Git pre-commit hook to perform linting before commits:

   .. code-block:: shell

      poetry run install-hook

8. **Set Poetry Virtual Environment as Project Interpreter**

   Set the Poetry virtual environment as the project interpreter. You can find the path to the virtual environment by running:

   .. code-block:: shell

      poetry env info

Use this path to configure your IDE or text editor to use the Poetry virtual environment.

Following these steps will give you a properly configured development environment for the ``gemtest`` framework.

Available poetry Scripts
------------------------

To run tests (with outputs), use:

.. code-block:: shell

    poetry run test

To run tests on an example, use:

.. code-block:: shell

    poetry run example <example-name>

To run tests with coverage and show results, use:

.. code-block:: shell

    poetry run cov

To run linters (equivalent to **poetry run prospector**), use:

.. code-block:: shell

    poetry run lint

Coding Standards
----------------

Make sure to read our :ref:`Coding Standards <coding_standards>` before getting started. This ensures consistency, maintainability, and code quality throughout the project.

Contributing on GitLab
----------------------

If you want to learn how to contribute on GitLab, check out the :ref:`GitLab Contribution Guide <gitlab_contribution>`.