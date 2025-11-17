API Reference
==============

This section provides detailed documentation for the AmalgamationAI API.

Client
------

.. autoclass:: amalgamationai.Client
   :members:
   :undoc-members:
   :show-inheritance:

Methods
-------

generate()
~~~~~~~~~~

Generate a response using the AI model.

.. code-block:: python

   response = client.generate(
       prompt="Your prompt here",
       model="gpt-4",
       temperature=0.7
   )

Parameters
^^^^^^^^^^

* ``prompt`` (str): The input prompt
* ``model`` (str, optional): The model to use
* ``temperature`` (float, optional): Sampling temperature

Returns
^^^^^^^

The generated response as a string.

chat()
~~~~~~

Send a chat message and get a response.

.. code-block:: python

   response = client.chat(
       messages=[
           {"role": "user", "content": "Hello!"}
       ]
   )

Parameters
^^^^^^^^^^

* ``messages`` (list): List of message dictionaries

Returns
^^^^^^^

The chat response.

