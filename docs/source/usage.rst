Usage
=====

.. _installation:

Installation
------------

To use PoliPrompt, first install it using pip:

.. code-block:: console

   (.venv) $ pip install PoliPrompt

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``poliprompt.get_random_ingredients()`` function:

.. autofunction:: poliprompt.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`poliprompt.get_random_ingredients`
will raise an exception.

.. autoexception:: poliprompt.InvalidKindError

For example:

>>> import PoliPrompt
>>> PoliPrompt.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

