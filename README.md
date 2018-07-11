[![Build Status](https://travis-ci.org/zeroincombenze/reporting-engine.svg?branch=8.0)](https://travis-ci.org/zeroincombenze/reporting-engine)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/reporting-engine/badge.svg?branch=8.0)](https://coveralls.io/github/zeroincombenze/reporting-engine?branch=8.0)
[![codecov](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/8.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/8.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-8.svg)](https://github.com/OCA/reporting-engine/tree/8.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-8.svg)](http://wiki.zeroincombenze.org/en/Odoo/8.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-8.svg)](http://wiki.zeroincombenze.org/en/Odoo/8.0/man/)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-8.svg)](http://erp8.zeroincombenze.it)






























































[![en](http://www.shs-av.com/wp-content/en_US.png)](http://wiki.zeroincombenze.org/it/Odoo/7.0/man)

OCA alternative reporting engines and reporting utilities for Odoo
==================================================================

This repository hosts alternative reporting engines to the ones included on Odoo core (RML, QWeb and Webkit). It is complemented with the ones that host the reports theirself:

https://github.com/OCA/account-financial-reporting
https://github.com/OCA/purchase-reporting
https://github.com/OCA/sale-reporting
...

The convention is to use a suffix to each module to indicate that it's for using with that report engine (for example, account_invoice_report_birt or sale_order_report_pentaho).

It can contain also another utilities directly involved with reports (like merge/split utils, checkers, signing tools and so on).

[//]: # (addons)


Available addons
----------------
addon | version | OCA version | summary
--- | --- | --- | ---
[bi_sql_editor](bi_sql_editor/) | 8.0.1.0.0 | :repeat: | BI Views builder, based on Materialized or Normal SQL Views
[bi_view_editor](bi_view_editor/) | 8.0.1.0.0 | :repeat: | Graphical BI views builder for Odoo 8
[report_qweb_element_page_visibility](report_qweb_element_page_visibility/) | 8.0.1.0.0 | :repeat: | Report Qweb Element Page Visibility
[report_qweb_signer](report_qweb_signer/) | 8.0.1.0.0 | :repeat: | Sign Qweb PDFs usign a PKCS#12 certificate
[report_xls](report_xls/) | 8.0.0.6.1 | :repeat: | Excel report engine
[report_xlsx](report_xlsx/) | 8.0.1.0.0 | :repeat: | Base module to create xlsx report
[report_xml](report_xml/) | 8.0.1.0.0 | :repeat: | Allow to generate XML reports
[report_xml_sample](report_xml_sample/) | 8.0.1.0.0 | :repeat: | For developers who want an example


Unported addons
---------------
addon | version | OCA version | summary
--- | --- | --- | ---
[base_report_assembler](base_report_assembler/) | 1.0 (unported) | :repeat: | Base Report Assembler
[report_custom_filename](report_custom_filename/) | 8.0.1.0.1 (unported) | 8.0.1.0.1 | Configure the filename to use when downloading a report

[//]: # (end addons)

----

OCA, or the Odoo Community Association, is a nonprofit organization whose 
mission is to support the collaborative development of Odoo features and 
promote its widespread use.

http://odoo-community.org/

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

[![chat with us](https://www.shs-av.com/wp-content/chat_with_us.gif)](https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b)
