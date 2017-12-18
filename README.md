[![Build Status](https://travis-ci.org/zeroincombenze/reporting-engine.svg?branch=10.0)](https://travis-ci.org/zeroincombenze/reporting-engine)
[![license agpl](https://img.shields.io/badge/licence-AGPL--3-blue.svg)](http://www.gnu.org/licenses/agpl-3.0.html)
[![Coverage Status](https://coveralls.io/repos/github/zeroincombenze/reporting-engine/badge.svg?branch=10.0)](https://coveralls.io/github/zeroincombenze/reporting-engine?branch=10.0)
[![codecov](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/10.0/graph/badge.svg)](https://codecov.io/gh/zeroincombenze/reporting-engine/branch/10.0)
[![OCA_project](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-oca-10.svg)](https://github.com/OCA/reporting-engine/tree/10.0)
[![Tech Doc](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-10.svg)](http://wiki.zeroincombenze.org/en/Odoo/10.0/dev)
[![Help](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-10.svg)](http://wiki.zeroincombenze.org/en/Odoo/10.0/man/)
[![try it](http://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-10.svg)](http://erp10.zeroincombenze.it)














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
[report_py3o](report_py3o/) | 10.0.1.1.0 | 10.0.1.2.0 | Reporting engine based on Libreoffice (ODT -> ODT, ODT -> PDF, ODT -> DOC, ODT -> DOCX, ODS -> ODS, etc.)
[report_qweb_element_page_visibility](report_qweb_element_page_visibility/) | 10.0.1.0.0 | :repeat: | Report Qweb Element Page Visibility
[report_qweb_parameter](report_qweb_parameter/) | 10.0.1.0.1 | :repeat: | Add new parameters for qweb templates in order to reduce field length and check minimal length
[report_qweb_pdf_watermark](report_qweb_pdf_watermark/) | 10.0.1.0.0 | 10.0.1.0.1 | Add watermarks to your QWEB PDF reports
[report_wkhtmltopdf_param](report_wkhtmltopdf_param/) | 10.0.1.0.1 | :repeat: | Add new parameters for a paper format to be used by wkhtmltopdf command as arguments.
[report_xlsx](report_xlsx/) | 10.0.1.0.1 | :repeat: | Base module to create xlsx report
[report_xml](report_xml/) | 10.0.1.0.0 | :repeat: | Allow to generate XML reports


Unported addons
---------------
addon | version | OCA version | summary
--- | --- | --- | ---
[base_report_assembler](base_report_assembler/) | 1.0 (unported) | :repeat: | Base Report Assembler

[//]: # (end addons)

----

OCA, or the Odoo Community Association, is a nonprofit organization whose 
mission is to support the collaborative development of Odoo features and 
promote its widespread use.

https://odoo-community.org/

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
