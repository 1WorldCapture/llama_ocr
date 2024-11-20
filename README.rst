=========
LLAMA OCR
=========


.. image:: https://img.shields.io/pypi/v/llama_ocr.svg
        :target: https://pypi.python.org/pypi/llama_ocr

.. image:: https://img.shields.io/travis/1WorldCapture/llama_ocr.svg
        :target: https://travis-ci.com/1WorldCapture/llama_ocr

.. image:: https://readthedocs.org/projects/llama-ocr/badge/?version=latest
        :target: https://llama-ocr.readthedocs.io/en/latest/?version=latest
        :alt: Documentation Status




OCR using LLAMA vision model, allowing configuring any OpenAI compliant endpoints and model names. This is the python version of [llama-ocr](https://github.com/Nutlope/llama-ocr/tree/main).


* Free software: MIT license

Installation
------------

`pip install llama-ocr`

Usage
--------

```python
from llama_ocr import ocr

data = ocr(
  file_path="./test.png", 
  api_key="xxxxx",
  base_url="https://openrouter.ai/api",
  model="meta-llama/llama-3.2-11b-vision-instruct:free"
) 
```

- `file_path`: Path to the image file
- `api_key`: Your LLM API key
- `base_url`: The base URL of the LLM API
- `model`: The model to use

By default, this project will use free model from OpenRouter. So you just need to provide your API key and image path.

Credits
-------

This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
