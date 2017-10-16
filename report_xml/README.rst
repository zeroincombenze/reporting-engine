[![Build Status](https://travis-ci.org/zeroincombenze/reporting-engine.svg?branch=10.0)](https://travis-ci.org/zeroincombenze/reporting-engine)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/reporting-engine/badge.svg?branch=10.0)](https://coveralls.io/github/zeroincombenze/reporting-engine?branch=10.0)
[![codecov](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/10.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/10.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-10.svg)](https://github.com/OCA/reporting-engine/tree/10.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-10.svg)](http://wiki.zeroincombenze.org/en/Odoo/10.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-10.svg)](http://wiki.zeroincombenze.org/en/Odoo/10.0/man/)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-10.svg)](http://erp10.zeroincombenze.it)


[![en](https://github.com/zeroincombenze/grymb/blob/master/flags/en_US.png)](https://www.facebook.com/groups/openerp.italia/)

    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
=================================================================
    :alt: License: AGPL-3
	
XML Reports
===========

This module was written to extend the functionality of the reporting engine to
support XML reports and allow modules to generate them by code or by QWeb
templates.

Installation
------------






To install this module, you need to:

* Install lxml_ in Odoo's ``$PYTHONPATH``.
* Install the repository `reporting-engine`_.

But this module does nothing for the end user by itself, so if you have it
installed it's probably because there is another module that depends on it.

Configuration
-------------





Usage
-----







=====

If you are a user

You will be able to download XML reports from the *Print* menu found on form
and list views.

If you are a developer

To learn from an example, just check the `sample module`_.

To develop with this module, you need to:

* Create a module.
* Make it depend on this one.
* Follow `instructions to create reports`_ having in mind that the
  ``report_type`` field in your ``ir.actions.report.xml`` record must be
  ``qweb-xml``.

In case you want to create a `custom report`_, the instructions remain the same
as for HTML reports, and the method that you must override is also called
``render_html``, even when this time you are creating a XML report.

You can make your custom report inherit ``report_xml.xsd_checked_report``, name
it like your XML ``<template>`` id prepended by ``report.``, add a ``xsd()``
method that returns a XSD in a string, and have XSD automatic checking for
free.

You can visit ``http://<server-address>/report/xml/<module.report_name>/<ids>``
to see your XML report online as a web page.

For further information, please visit:

* https://www.odoo.com/forum/help-1
* https://github.com/OCA/reporting-engine

Known issues / Roadmap
----------------------





Bug Tracker
-----------





Credits
-------






* Icon taken from http://commons.wikimedia.org/wiki/File:Text-xml.svg.






### Contributors






* Jairo Llopis <j.llopis@grupoesoc.es>
* Enric Tobella <etobella@creublanca.es>

### Funders

### Maintainer










.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit http://odoo-community.org.


.. _custom report: https://www.odoo.com/documentation/8.0/reference/reports.html#custom-reports
.. _instructions to create reports: https://www.odoo.com/documentation/8.0/reference/reports.html
.. _reporting-engine: https://github.com/OCA/reporting-engine
.. _sample module: https://github.com/OCA/reporting-engine/tree/8.0/report_xml_sample
.. _lxml: http://lxml.de/

[//]: # (copyright)

----

**Odoo** is a trademark of [Odoo S.A.](https://www.odoo.com/) (formerly OpenERP, formerly TinyERP)

**OCA**, or the [Odoo Community Association](http://odoo-community.org/), is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

**zeroincombenze®** is a trademark of [SHS-AV s.r.l.](http://www.shs-av.com/)
which distributes and promotes **Odoo** ready-to-use on its own cloud infrastructure.
[Zeroincombenze® distribution](http://wiki.zeroincombenze.org/en/Odoo)
is mainly designed for Italian law and markeplace.
Everytime, every Odoo DB and customized code can be deployed on local server too.

[//]: # (end copyright)

[//]: # (addons)

[//]: # (end addons)

[![chat with us](https://www.shs-av.com/wp-content/chat_with_us.gif)](https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b)
