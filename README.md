[![Build Status](https://travis-ci.org/zeroincombenze/reporting-engine.svg?branch=7.0)](https://travis-ci.org/zeroincombenze/reporting-engine)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/reporting-engine/badge.svg?branch=7.0)](https://coveralls.io/github/zeroincombenze/reporting-engine?branch=7.0)
[![codecov](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/7.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/7.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-7.svg)](https://github.com/OCA/reporting-engine/tree/7.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-7.svg)](http://wiki.zeroincombenze.org/en/Odoo/7.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-7.svg)](http://wiki.zeroincombenze.org/en/Odoo/7.0/man/)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-7.svg)](http://erp7.zeroincombenze.it)


[![en](https://github.com/zeroincombenze/grymb/blob/master/flags/en_US.png)](https://www.facebook.com/groups/openerp.italia/)
================================================================================================
================================================================================================

This repository hosts alternative reporting engines to the ones included on Odoo core (RML and Webkit). It is complemented with the ones that host the reports theirself:
================================================================================================

https://launchpad.net/account-financial-report

https://launchpad.net/purchase-report

https://launchpad.net/sale-reports

...

The convention is to use a suffix to each module to indicate that it's for using with that report engine (for example, account_invoice_report_birt or sale_order_report_pentaho).

It can contain also another utilities directly involved with reports (like merge/split utils, checkers, signing tools and so on).

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


Available addons
----------------
addon | version | OCA version | summary
--- | --- | --- | ---
[base_report_assembler](base_report_assembler/) | 1.0 | :repeat: | Assemble multiple reports in one PDF
[report_custom_filename](report_custom_filename/) | 1.0 | :repeat: | Configure the filename to use when downloading a report
[report_xls](report_xls/) | 0.6 | :repeat: | Excel report engine

[//]: # (end addons)

[![chat with us](https://www.shs-av.com/wp-content/chat_with_us.gif)](https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b)
