==============================================================================================
Python wrapper for the SonarQube(Community Edition and Enterprise Edition) and SonarCloud API.
==============================================================================================

Version
=======
This version of the Python-Sonarqube-api is forked from shijl0925 repository. It is based on the version before the changes to move to GNU and remove free features


Installation
============

The easiest way to install the latest version is by using pip to pull it from PyPI::

    pip install  --upgrade python-sonarqube-api

You may also use Git to clone the repository from Github and install it manually::

    git clone https://github.com/shijl0925/python-sonarqube-api.git
    cd python-sonarqube-api
    python setup.py install


Documentation
=============

The full documentation for API is available on `readthedocs
<https://python-sonarqube-api.readthedocs.io/en/latest/>`_.


Compatibility
=============

* This package is compatible Python versions 2.7, 3.3+.
* Tested with SonarQube Community Edition 7.9.x LTS and SonarCloud Server.

Donate
======

donations are not mandatory but very welcomed
If you like shijl0925's work and want to support development or buy shijl0925 a coffee `PayPal Donate <https://paypal.me/shijialiang0925>`_

Paypal
------
.. image:: https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg
    :target: https://paypal.me/shijialiang0925

Wechat Pay
----------
.. image:: https://raw.githubusercontent.com/shijl0925/python-sonarqube-api/master/docs/wechat.jpg

Alipay
------
.. image:: https://raw.githubusercontent.com/shijl0925/python-sonarqube-api/master/docs/alipay.jpg

Usage
=====

For SonarQube Community Edition
-------------------------------

The Client is easy to use, you just need to initialize it with the
connection parameters (default sonarqube url is http://localhost:9000).

Example::

    from sonarqube import SonarQubeClient

    h = SonarQubeClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')


Sonar authentication tokens can also be used in place of username and password::

    h = SonarQubeClient(sonarqube_url="http://localhost:9000", token='*****************')


For SonarCloud
--------------

Example::

    from sonarqube import SonarCloudClient
    h = SonarCloudClient(sonarcloud_url="https://sonarcloud.io", token='*****************')


For SonarQube Enterprise Edition
--------------------------------

The Client is easy to use, you just need to initialize it with the
connection parameters (default sonarqube url is http://localhost:9000).

Example::

    from sonarqube import SonarEnterpriseClient

    h = SonarEnterpriseClient(sonarqube_url="http://localhost:9000", username='admin', password='admin')


Sonar authentication tokens can also be used in place of username and password::

    h = SonarEnterpriseClient(sonarqube_url="http://localhost:9000", token='*****************')


API example
-----------

The example documentation for SonarQubeClient APIs is available on `API examples
<https://python-sonarqube-api.readthedocs.io/en/latest/examples.html>`_.

