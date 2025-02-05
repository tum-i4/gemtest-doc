Usage and Commands
==================

Running Metamorphic Tests
-------------------------

To run tests from the project root directory using the command line and ensure consistent
asset location for the test report, use:

.. code-block:: shell

    pytest <options> <path to test file/folder>

If you prefer to use your IDE's GUI to run tests, set the working directory to the project
root using the run configuration of your IDE.



.. _available_options_for_testing:

Available options for Testing Metamorphic Relation
--------------------------------------------------

To enable custom string report output on the console, use the following:

.. code-block:: shell

    pytest --string-report <test-file path>

To enable custom HTML reports, including visualization of inputs and outputs, and store
test results in an SQLite database viewable in the ``gemtest-webapp``, use:

.. code-block:: shell

    pytest --html-report <test-file path>

Launching the Web App
---------------------

To install the ``gemtest-webapp``, execute:

.. code-block:: shell

    pip install gemtest-webapp

To launch the ``gemtest-webapp``, execute the following command:

.. code-block:: shell
    
    gemtest-webapp --results-dir gemtest_results/

If the ``gemtest-webapp`` is running on a remote server at http://127.0.0.1:5000, you can forward that port to your local machine using SSH:

.. code-block:: shell

    ssh -L 127.0.0.1:5001:127.0.0.1:5000 user@host

After forwarding the port, access the web app at http://127.0.0.1:5001.