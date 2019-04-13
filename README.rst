
======================================
|Zeroincombenze| reporting-engine 10.0
======================================

|Maturity| |Build Status| |Coverage Status| |Codecov Status| |license gpl| |Tech Doc| |Help| |Try Me|

.. contents::


Overview / Panoramica
=====================

|en| Reposting Engine

This repository hosts alternative reporting engines to the ones included on Odoo core (RML, QWeb and Webkit). It is complemented with the ones that host the reports theirself:

* https://github.com/OCA/account-financial-reporting
* https://github.com/OCA/purchase-reporting
* https://github.com/OCA/sale-reporting

The convention is to use a suffix to each module to indicate that it's for using with that report engine (for example, account_invoice_report_birt or sale_order_report_pentaho).

It can contain also another utilities directly involved with reports (like merge/split utils, checkers, signing tools and so on).


|it| Motore Rendiconti

Progetto basato sui moduli OCA motore rendiconti

Avaiable Addons / Moduli disponibili
------------------------------------

+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| Name / Nome                         | Version    | OCA Ver.   | Description / Descrizione                                                        |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| base_report_assembler               | |halt|     | |halt|     | Base Report Assembler                                                            |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| bi_sql_editor                       | 10.0.1.0.0 | |same|     | BI Views builder, based on Materialized or Normal SQL Views                      |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| bi_view_editor                      | 10.0.1.0.2 | |same|     | Graphical BI views builder for Odoo                                              |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_py3o                         | |halt|     | |same|     | Reporting engine based on Libreoffice (ODT -> ODT, ODT -> PDF, ODT -> DOC, ODT - |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_py3o_fusion_server           | |halt|     | |same|     | Let the fusion server handle format conversion.                                  |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_qweb_element_page_visibility | 10.0.1.0.0 | |same|     | Report Qweb Element Page Visibility                                              |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_qweb_parameter               | 10.0.1.0.1 | |same|     |  Add new parameters for qweb templates in order to reduce field length and check |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_qweb_pdf_watermark           | 10.0.1.0.2 | |same|     | Add watermarks to your QWEB PDF reports                                          |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_qweb_signer                  | 10.0.1.0.1 | |same|     | Sign Qweb PDFs usign a PKCS#12 certificate                                       |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_qweb_txt                     | 10.0.1.0.0 | |same|     | Use Qweb to generate text and CSV reports                                        |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_wkhtmltopdf_param            | 10.0.1.0.1 | |same|     |  Add new parameters for a paper format to be used by wkhtmltopdf command as argu |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_xlsx                         | 10.0.1.0.1 | |same|     |  Base module to create xlsx report                                               |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_xlsx_helper                  | 10.0.1.0.0 | |same|     | Report xlsx helpers                                                              |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+
| report_xml                          | 10.0.1.0.0 | |same|     | Allow to generate XML reports                                                    |
+-------------------------------------+------------+------------+----------------------------------------------------------------------------------+


OCA comparation / Confronto con OCA
-----------------------------------


+-----------------------------------------------------------------+-------------------+-----------------------+--------------------------------+
| Description / Descrizione                                       | Zeroincombenze    | OCA                   | Notes / Note                   |
+-----------------------------------------------------------------+-------------------+-----------------------+--------------------------------+
| Coverage / Copertura test                                       |  |Codecov Status| | |OCA Codecov Status|  | |OCA project|                  |
+-----------------------------------------------------------------+-------------------+-----------------------+--------------------------------+


Getting started / Come iniziare
===============================

|Try Me|


Prerequisites / Prerequisiti
----------------------------


* python2.7+
* postgresql 9.2+

Installation / Installazione
----------------------------

+---------------------------------+------------------------------------------+
| |en|                            | |it|                                     |
+---------------------------------+------------------------------------------+
| These instruction are just an   | Istruzioni di esempio valide solo per    |
| example to remember what        | distribuzioni Linux CentOS 7, Ubuntu 14+ |
| you have to do on Linux.        | e Debian 8+                              |
|                                 |                                          |
| Installation is built with:     | L'installazione è costruita con:         |
+---------------------------------+------------------------------------------+
| `Zeroincombenze Tools <https://github.com/zeroincombenze/tools>`__         |
+---------------------------------+------------------------------------------+
| Suggested deployment is:        | Posizione suggerita per l'installazione: |
+---------------------------------+------------------------------------------+
| /opt/odoo/10.0/reporting-engine/                                           |
+----------------------------------------------------------------------------+

::

    cd $HOME
    git clone https://github.com/zeroincombenze/tools.git
    cd ./tools
    ./install_tools.sh -p
    export PATH=$HOME/dev:$PATH
    odoo_install_repository reporting-engine -b 10.0 -O zero
    for pkg in os0 z0lib; do
        pip install $pkg -U
    done
    sudo manage_odoo requirements -b 10.0 -vsy -o /opt/odoo/10.0


Upgrade / Aggiornamento
-----------------------

+---------------------------------+------------------------------------------+
| |en|                            | |it|                                     |
+---------------------------------+------------------------------------------+
| When you want upgrade and you   | Per aggiornare, se avete installato con  |
| installed using above           | le istruzioni di cui sopra:              |
| statements:                     |                                          |
+---------------------------------+------------------------------------------+

::

    odoo_install_repository reporting-engine -b 10.0 -O zero -U
    # Adjust following statements as per your system
    sudo systemctl restart odoo


Support / Supporto
------------------


|Zeroincombenze| This project is mainly maintained by the `SHS-AV s.r.l. <https://www.zeroincombenze.it/>`__



Get involved / Ci mettiamo in gioco
===================================

Bug reports are welcome! You can use the issue tracker to report bugs,
and/or submit pull requests on `GitHub Issues
<https://github.com/zeroincombenze/reporting-engine/issues>`_.

In case of trouble, please check there if your issue has already been reported.

Proposals for enhancement
-------------------------


|en| If you have a proposal to change this module, you may want to send an email to <cc@shs-av.com> for initial feedback.
An Enhancement Proposal may be submitted if your idea gains ground.

|it| Se hai proposte per migliorare questo modulo, puoi inviare una mail a <cc@shs-av.com> per un iniziale contatto.

Credits / Titoli di coda
========================

Copyright
---------

Odoo is a trademark of `Odoo S.A. <https://www.odoo.com/>`__ (formerly OpenERP)


----------------


|en| **zeroincombenze®** is a trademark of `SHS-AV s.r.l. <https://www.shs-av.com/>`__
which distributes and promotes ready-to-use **Odoo** on own cloud infrastructure.
`Zeroincombenze® distribution of Odoo <https://wiki.zeroincombenze.org/en/Odoo>`__
is mainly designed to cover Italian law and markeplace.

|it| **zeroincombenze®** è un marchio registrato da `SHS-AV s.r.l. <https://www.shs-av.com/>`__
che distribuisce e promuove **Odoo** pronto all'uso sulla propria infrastuttura.
La distribuzione `Zeroincombenze® <https://wiki.zeroincombenze.org/en/Odoo>`__ è progettata per le esigenze del mercato italiano.


|chat_with_us|


|


Last Update / Ultimo aggiornamento: 2019-04-13

.. |Maturity| image:: https://img.shields.io/badge/maturity-Alfa-red.png
    :target: https://odoo-community.org/page/development-status
    :alt: Alfa
.. |Build Status| image:: https://travis-ci.org/zeroincombenze/reporting-engine.svg?branch=10.0
    :target: https://travis-ci.org/zeroincombenze/reporting-engine
    :alt: github.com
.. |license gpl| image:: https://img.shields.io/badge/licence-LGPL--3-7379c3.svg
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: LGPL-3
.. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
    :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
    :alt: License: OPL
.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/reporting-engine/badge.svg?branch=10.0
    :target: https://coveralls.io/github/zeroincombenze/reporting-engine?branch=10.0
    :alt: Coverage
.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/reporting-engine/branch/10.0/graph/badge.svg
    :target: https://codecov.io/gh/OCA/reporting-engine/branch/10.0
    :alt: Codecov
.. |OCA project| image:: Unknown badge-OCA
    :target: https://github.com/OCA/reporting-engine/tree/10.0
    :alt: OCA
.. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-10.svg
    :target: https://wiki.zeroincombenze.org/en/Odoo/10.0/dev
    :alt: Technical Documentation
.. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-10.svg
    :target: https://wiki.zeroincombenze.org/it/Odoo/10.0/man
    :alt: Technical Documentation
.. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-10.svg
    :target: https://erp10.zeroincombenze.it
    :alt: Try Me
.. |OCA Codecov Status| image:: https://codecov.io/gh/OCA/reporting-engine/branch/10.0/graph/badge.svg
    :target: https://codecov.io/gh/OCA/reporting-engine/branch/10.0
    :alt: Codecov
.. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
   :target: https://odoo-italia.org
   :alt: Odoo Italia Associazione
.. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
   :target: https://www.zeroincombenze.it/
   :alt: Zeroincombenze
.. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
   :target: https://www.facebook.com/groups/openerp.italia/
.. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
   :target: https://www.facebook.com/groups/openerp.italia/
.. |check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/check.png
.. |no_check| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/no_check.png
.. |menu| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/menu.png
.. |right_do| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/right_do.png
.. |exclamation| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/exclamation.png
.. |warning| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/warning.png
.. |same| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/same.png
.. |late| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/late.png
.. |halt| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/halt.png
.. |info| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/awesome/info.png
.. |xml_schema| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/iso/icons/xml-schema.png
   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/iso/scope/xml-schema.md
.. |DesktopTelematico| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/DesktopTelematico.png
   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/Desktoptelematico.md
.. |FatturaPA| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/certificates/ade/icons/fatturapa.png
   :target: https://github.com/zeroincombenze/grymb/blob/master/certificates/ade/scope/fatturapa.md
.. |chat_with_us| image:: https://www.shs-av.com/wp-content/chat_with_us.gif
   :target: https://tawk.to/85d4f6e06e68dd4e358797643fe5ee67540e408b
