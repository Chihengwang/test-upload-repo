Getting Started
================

This guide will help you get started with AmalgamationAI.

Installation
------------

Install AmalgamationAI using pip:

.. code-block:: bash

   pip install amalgamationai

Quick Start
-----------

Here's a simple example to get you started:

.. code-block:: python

   from amalgamationai import Client

   client = Client(api_key="your-api-key")
   response = client.generate("Hello, world!")
   print(response)

Configuration
------------

You can configure AmalgamationAI through environment variables or a configuration file.

Environment Variables
~~~~~~~~~~~~~~~~~~~~~

Set the following environment variables:

* ``AMALGAMATIONAI_API_KEY``: Your API key
* ``AMALGAMATIONAI_BASE_URL``: Base URL for the API (optional)

Configuration File
~~~~~~~~~~~~~~~~~~

Create a ``config.yaml`` file:

.. code-block:: yaml

   api_key: your-api-key
   base_url: https://api.example.com
   timeout: 30

Next Steps
----------

* Read the :doc:`api-reference` for detailed API documentation
* Check out the :doc:`examples` for more code samples

