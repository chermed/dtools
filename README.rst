Dtools Package
==============

**Dtools** package provide a wrapper object around relativedelta to manage date and datetime strings

Installation :
==============


.. code-block:: shell

    pip install dtools

Examples :
==========

**Example 1:**

.. code-block:: python

    >>> from dtools import Date
    >>> Date('2017-06-04').relativedelta(days=2)
    '2017-06-06'
    >>> type(Date('2017-06-04').relativedelta(days=2))
    <class 'str'>


**Example 2:**

.. code-block:: python

    >>> from dtools import Date
    >>> Date('2017-06-04').relativedelta(month=2, day=3)
    '2017-02-03'
    >>> Date('2017-06-04').relativedelta(last_day=True)
    '2017-06-30'
    >>> Date('2017-06-04').relativedelta(months=4, last_day=True)
    '2017-10-31'

**Example 3:**

.. code-block:: python

    >>> from dtools import Date
    >>> Date('2017-06-04').relativedelta(hour=12)
    >>> '2017-06-04'
    >>> Date('2017-06-04').relativedelta(hour=12, rtype='datetime')
    >>> '2017-06-04 12:00:00'

**Example 4:**

.. code-block:: python

    >>> from dtools import Date
    >>> Date('2017-06-04 04:30:00').relativedelta(days=4, hour=12)
    >>> '2017-06-08 12:30:00'
    >>> Date('2017-06-04 04:30:00').relativedelta(days=4, hour=12, rtype='date')
    >>> '2017-06-08'


Licence
=======

This software is made available under the LGPL v3 license.

Bug Tracker
===========

Please, feel free to report bugs or suggestions in the `Bug Tracker <https://github.com/chermed/dtools/issues>`_!

Credits:
========

Mohamed Cherkaoui <http://mohamedcherkaoui.com>



News
====

2.0.0
-----

*Release date: 04-Jun-2017*

* First stable version