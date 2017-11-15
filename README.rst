=============================
Welcome to python-idex v0.1.0
=============================

.. image:: https://img.shields.io/pypi/v/python-idex.svg
    :target: https://pypi.python.org/pypi/python-idex

.. image:: https://img.shields.io/pypi/l/python-idex.svg
    :target: https://pypi.python.org/pypi/python-idex

.. image:: https://img.shields.io/travis/sammchardy/python-idex.svg
    :target: https://travis-ci.org/sammchardy/python-idex

.. image:: https://img.shields.io/coveralls/sammchardy/python-idex.svg
    :target: https://coveralls.io/github/sammchardy/python-idex

.. image:: https://img.shields.io/pypi/wheel/python-idex.svg
    :target: https://pypi.python.org/pypi/python-idex

.. image:: https://img.shields.io/pypi/pyversions/python-idex.svg
    :target: https://pypi.python.org/pypi/python-idex

This is an unofficial Python wrapper for the `IDEX exchanges REST API v1 <https://github.com/AuroraDAO/idex-api-docs>`_. I am in no way affiliated with IDEX, use at your own risk.

PyPi
  https://pypi.python.org/pypi/python-idex

Source code
  https://github.com/sammchardy/python-idex

Documentation
  https://python-idex.readthedocs.io/en/latest/


Features
--------

- Implementation of all non trading REST endpoints.
- Helper functions for your wallet address
- Response exception handling

Quick Start
-----------

Register an account with `IDEX <https://idex.market/>`_.

.. code:: bash

    pip install python-idex


.. code:: python

    from idex.client import Client
    client = Client(address, private_key)

    # get currencies
    currencies = client.get_currencies()

    # get market depth
    depth = client.get_order_book('ETH_SAN')

    # get your balances
    balances = client.get_my_balances()

    # get your open orders
    orders = client.get_my_open_orders('ETH_SAN')


For more `check out the documentation <https://python-kucoin.readthedocs.io/en/latest/>`_.

TODO
----

- Trading endpoints
- Websocket endpoints

Donate
------

If this library helped you out feel free to donate.

- ETH: 0xD7a7fDdCfA687073d7cC93E9E51829a727f9fE70
- NEO: AVJB4ZgN7VgSUtArCt94y7ZYT6d5NDfpBo
- BTC: 1Dknp6L6oRZrHDECRedihPzx2sSfmvEBys

Other Exchanges
---------------

If you use `Binance <https://www.binance.com/register.html?ref=10099792>`_ check out my `python-binance <https://github.com/sammchardy/python-binance>`_ library.

If you use `Quoinex <https://accounts.quoinex.com/sign-up?affiliate=PAxghztC67615>`_
or `Qryptos <https://accounts.qryptos.com/sign-up?affiliate=PAxghztC67615>`_ check out my `python-quoine <https://github.com/sammchardy/python-quoine>`_ library.

If you use `Kucoin <https://www.kucoin.com/#/?r=E42cWB>`_ check out my `python-kucoin <https://github.com/sammchardy/python-kucoin>`_ library.