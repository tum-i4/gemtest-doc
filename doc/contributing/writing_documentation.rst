Documentation Guide
====================

The following section guides you on how to contribute to the documentation page:

Documentation Tools
-------------------

Sphinx
######

This documentation is automatically generated using ``Sphinx``, using the ReadTheDocs HTML theme. The documentation configuration can be found in the conf.py, where you can further customize the HTML output or add useful extensions.
If you have implemented your changes and want to view them locally, run the ``make HTML`` command in the /docs directory. The HTML files are built in the ``_build/html`` directory. You can open up the HTML files in your local browser and view your changes!

reStructuredText
################
We use reStructuredText as the plaintext markup language because of its compatibility with Sphinx. 

You can learn more about the RST syntax here: https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html.

Make sure to use the various functionalities provided by reStructuredText and Sphinx, as they greatly enhance the user-friendliness and clarity of the overall docs page.
Highlight important keywords and add visualizations where possible.

GitLab Pages
############

The documentation is currently deployed on GitLab Pages, making it reachable via a URL. 

Grammar and Spelling Tools
##########################
Please make use of online grammar and spelling tools, such as https://languagetool.org. These tools help ensure correctness throughout the documentation and mitigate any spelling errors or typos.

Creating Diagrams
------------------

The following tools can help you efficiently design and generate a wide range of diagrams. We encourage you to use visualizations.

Available Tools
##################

- To visualize processes as in the :ref:`Test Execution Workflow <test_workflow>` section. You can use the tools `plantuml <https://plantuml.com/en/>`_ or `sequencediagram.org <https://sequencediagram.org/>`_ . The sequence diagram was created by logging function calls within the ``gemtest`` framework and writing them in the plantuml syntax. Save the file as a **.puml** file. You can then run plantuml <your-file-name>.puml to automatically create the diagram. The diagram was further edited with `sequencediagram.org <https://sequencediagram.org/>`_.

- Another free online tool is draw.io, which one can use to create various charts and diagrams. The tool can be used here: https://app.diagrams.net/.

Including the Diagrams
#######################

The diagrams you create should be located in the resource folders of the subsections you are working on (e.g., docs/contributing/resources). You can display an image in reStructuredText using:

.. code::
    
     .. image:: <path-to-your-image>.

.. note:: 

    When including a new diagram or chart in the resource folder, please make sure to also include an editable file, such as a ``.xml``. This way, future contributors can extend your charts if necessary.


Automated Build and Deployment
------------------------------

We have set up an automatic build and deployment process using the GitLab CI pipeline. Any changes made to the documentation and pushed to certain branches are automatically built and deployed to GitLab Pages. 
The changes made will be directly visible.




By following these guidelines, you can help maintain high-quality documentation that benefits all users and developers involved in the project.