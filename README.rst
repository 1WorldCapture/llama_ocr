=========
LLAMA OCR
=========

Using LLAMA Vision Model for OCR, allowing configuring any OpenAI compliant endpoints and model names. This is the python version of `llama-ocr <https://github.com/Nutlope/llama-ocr/tree/main>`_.


* Free software: MIT license

Installation
------------

.. code-block:: bash
    :linenos:

    pip install llama-ocr

Usage
--------

.. code-block:: python
    :linenos:

    from llama_ocr import ocr

    data = ocr(
      file_path="./test.png", 
      api_key="xxxxx",
      base_url="https://openrouter.ai/api",
      model="meta-llama/llama-3.2-11b-vision-instruct:free"
    ) 
    # file_path: Path to the image file
    # api_key: Your LLM API key
    # base_url: The base URL of the LLM API
    # model: The model to use

By default, this project will use the free model from OpenRouter. So you just need to provide your API key and image path.

Credits
-------

This package was created with `Cookiecutter <https://github.com/audreyr/cookiecutter>`_ and the `audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`_ project template.
