.. _user_installation:

Get Started
===========

Install Gemtest
---------------

``gemtest`` requires: Python 3.8+

Run the following command in your command line:

.. code-block:: bash

    pip install gemtest


Create your first test
----------------------

Create a new file called ``test_sin_metamorphic.py``:

.. code-block:: python

    import gemtest as gmt
    import math

    mr_1 = gmt.create_metamorphic_relation(name='mr_1', data=range(100))


    @gmt.transformation(mr_1)
    def example_transformation(source_input: float) -> float:
      return source_input + 2 * math.pi


    @gmt.relation(mr_1)
    def example_relation(source_output: float, followup_output: float) -> bool:
      return gmt.relations.approximately(source_output, followup_output)


    @gmt.system_under_test(mr_1)
    def test_example_sut(input: float) -> float:
      return math.sin(input)

And execute it with:

.. code-block:: shell

    $ pytest test_sin_metamorphic.py
    =============== test session starts ===============
    platform linux -- Python 3.10.12, pytest-8.3.4,
    pluggy-1.5.0
    rootdir: /home/user/gemtest
    plugins: typeguard-2.13.3, html-3.2.0,
    metadata-3.1.1, xdist-3.6.1, gemtest-1.0.0,
    cov-4.1.0, hypothesis-6.113.0
    collected 100 items

    test_sin_metamorphic.py ..................
    ..........................................
    ........................................

    =============== 100 passed in 0.28s ===============