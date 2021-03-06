======================
Python Kong Management
======================


.. image:: https://img.shields.io/pypi/v/python_kong_management.svg
        :target: https://pypi.python.org/pypi/python_kong_management

.. image:: https://travis-ci.org/mwisner/python-kong-management.svg?branch=master
    :target: https://travis-ci.org/mwisner/python-kong-management

.. image:: https://readthedocs.org/projects/python-kong-management/badge/?version=latest
        :target: https://python-kong-management.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status

.. image:: https://pyup.io/repos/github/mwisner/python-kong-management/shield.svg
     :target: https://pyup.io/repos/github/mwisner/python-kong-management/
     :alt: Updates


Python api wrapper for Kong API Gatway


* Free software: MIT license
* Documentation: https://python-kong-management.readthedocs.io.


Features
--------

* This is very much a work-in-progress. Implemented functionality

Consumers
`````````
* `create`
* `update_or_create`
* `retrieve`
* `list`
* `update`
* `delete`
* `add_key`
* `remove_key`

Node
````
* `information`
* `status`

Errors
``````

```
error_codes = {
    'unauthorized': AuthenticationError,
    'forbidden': AuthenticationError,
    'bad_request': BadRequestError,
    'action_forbidden': BadRequestError,
    'missing_parameter': BadRequestError,
    'parameter_invalid': BadRequestError,
    'parameter_not_found': BadRequestError,
    'not_found': ResourceNotFound,
    'service_unavailable': ServiceUnavailableError,
}
```

Testing
---------
```bash
cp .env.example .env
python3 -m venv venv
source venv
eval $(cat .env | sed 's/^/export /')
setup.py pytest
```
