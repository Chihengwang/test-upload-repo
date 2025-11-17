Examples
========

This section contains various examples demonstrating how to use AmalgamationAI.

Basic Usage
-----------

Simple text generation:

.. code-block:: python

   from amalgamationai import Client

   client = Client(api_key="your-api-key")
   result = client.generate("Write a short story about AI")
   print(result)

Chat Example
------------

Interactive chat:

.. code-block:: python

   from amalgamationai import Client

   client = Client(api_key="your-api-key")
   
   messages = [
       {"role": "user", "content": "What is machine learning?"}
   ]
   
   response = client.chat(messages=messages)
   print(response)

Advanced Example
----------------

Using custom configuration:

.. code-block:: python

   from amalgamationai import Client

   client = Client(
       api_key="your-api-key",
       base_url="https://custom-api.example.com",
       timeout=60
   )
   
   result = client.generate(
       prompt="Explain quantum computing",
       model="gpt-4",
       temperature=0.5,
       max_tokens=1000
   )
   
   print(result)

Error Handling
--------------

Handle errors gracefully:

.. code-block:: python

   from amalgamationai import Client
   from amalgamationai.exceptions import APIError

   try:
       client = Client(api_key="your-api-key")
       result = client.generate("Test prompt")
   except APIError as e:
       print(f"API Error: {e}")
   except Exception as e:
       print(f"Unexpected error: {e}")

