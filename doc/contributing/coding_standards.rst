.. _coding_standards:

Coding Standards
============================================================================

Formatting 
----------

Code formatting is necessary for consistency, readability, and maintainability throughout the project.
As a contributor, it is essential to follow the `PEP8 Style Guide for Python Code <https://peps.python.org/pep-0008/>`_.

We recommend using IDE-specific tools for automated formatting: 

- For PyCharm users, utilize the built-in formatter to enforce a consistent style throughout your code.
- If you are using VSCode, consider using Black formatter, a popular code formatter adhering to PEP8 Guidelines. 
- To contribute to the Documentation Page, we are using reStructuredText. We recommend this `VS Code Extension <https://www.restructuredtext.net/>`_.

Best Practices
--------------

Adopting best practices ensures code quality and consistency throughout the project. Here are some essential practices to consider:

- **Documentation**: Provide clear and concise comments and docstrings to explain code functionality. Comments should clarify complex logic, describe assumptions, or provide context that isn't immediately clear from the code itself.
- **Modularity**: Break down complex tasks into smaller, reusable functions and classes. Refactor code if possible to reduce redundancy and increase reusability. 
- **Code Reviews**: Engage in code reviews to increase the overall code quality, find bugs early on, and form a sense of community between contributors.
- **Simplicity, Clarity, and Correctness**: Keep your code as simple and clear as possible while ensuring correctness and safety. This ensures that your code is understandable to other contributors and reviewers.

By incorporating these practices, you contribute to building maintainable, efficient, and secure code.

Docstring Guidelines
--------------------

To ensure consistent and well-documented code as well as provide helpful function tooltips for users, please follow the following docstring conventions:

We use **Numpy style** docstrings, which should be properly rendered as tooltips in supported IDEs such as VSCode or PyCharm. This format organizes function parameters, return values, examples, and other helpful information. The following sections should be used where appropriate:

- **Parameters**: List the function arguments, including their types and descriptions.
- **Returns**: Provide a description of the return value(s) as well as their types, if applicable.
- **Examples**: Include code examples if possible. 
- **See Also**: Refer to related functions, methods, or classes.

Sections should be formatted using ``-----`` to create headers.

For further reading on the Numpy style, you can visit the  `Numpydoc Style Guide <https://numpydoc.readthedocs.io/en/latest/format.html>`_.

Code Examples
~~~~~~~~~~~~~

When providing code examples, use the **`>>>`** prompt for Python code to illustrate how a function or method works. The line is then rendered as code when viewing the docstring as a tooltip. For example:

.. code-block:: python

    Examples
    --------
    >>> equality(1, 1)  # Holds
    True
    >>> equality(2, 3)  # Does not hold
    False

Grammar and Spelling
~~~~~~~~~~~~~~~~~~~~

All docstrings must adhere to proper grammar and spelling. We recommend using third-party tools to verify the correctness of the docstrings.