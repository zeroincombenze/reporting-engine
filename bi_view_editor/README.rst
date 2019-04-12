
=====================
|icon| BI View Editor
=====================


**Graphical BI views builder for Odoo**

.. |icon| image:: https://raw.githubusercontent.com/zeroincombenze/reporting-engine/10.0/bi_view_editor/static/description/icon.png

|Maturity| |Build Status| |Coverage Status| |Codecov Status| |license gpl| |Tech Doc| |Help| |Try Me|

.. contents::


Overview / Panoramica
=====================

|en| BI View Editor is a tool integrated in Odoo that allows users define and
execute their own reports without the need to code.

Purpose:

* The BI View Editor is used to create reports not already contained in the
  standard Odoo, combining data from existing sources.

* It has been designed to be used by users with little or no knowledge of
  the technical architecture of Odoo. Users visually link business objects
  and select the fields to visualize.

* The BI View Editor offers users different types of representations,
  including tree, graph, pivot views.


|

|it| Odoo è una suite di prodotti web open-source.

Le principali applicazioni di Odoo includono un Open Source CRM e Enterprise Resource Planning.
I principali moduli ERP sono: gestione Magazzino, gestione Progetti, Contabilità e Fatturazione, Punto vendite, Dipendenti, Produzione, gestione Acquisti, gestione vendite e molto altro ancora.


Distributions / Distribuzioni Odoo 10.0:
========================================


+-------------+----------------------------------+------------------------------------+--------------------------------------------------------------+-------------------+
| name / nome | description / descrizione        | Italy / Localizzazione Italiana    | Maintainers                                                  | License / Licenza |
+-------------+----------------------------------+------------------------------------+--------------------------------------------------------------+-------------------+
|             | Odoo EE - Enterprise Edition     | |check| Tramite partner        (1) | `Odoo S.A. <https://www.odoo.com/>`__                        | |license opl|     |
+-------------+----------------------------------+------------------------------------+--------------------------------------------------------------+-------------------+
| odoo        | Odoo CE - Community Edition      | |no_check|                         | `Odoo S.A. <https://www.odoo.com/>`__                        | |license gpl|     |
+-------------+----------------------------------+------------------------------------+--------------------------------------------------------------+-------------------+
| oca         | Odoo CE by OCA                   | |warning| Norme fiscali < 2107 (2) | `Odoo Community Association <http://odoo-community.org/>`__  | |license gpl|     |
+-------------+----------------------------------+------------------------------------+--------------------------------------------------------------+-------------------+
| oia         | Odoo CE by OIA                   | |warning| Norme fiscali < 2107 (3) | `Associazione Odoo Italia <https://www.odoo-italia.org/>`__  | |license gpl|     |
+-------------+----------------------------------+------------------------------------+--------------------------------------------------------------+-------------------+
| zero        | Zeroincombenze(R)                | |warning| Norme fiscali < 2107 (3) | `SHS-AV s.r.l. <http://www.shs-av.com/>`__                   | |license gpl|     |
+-------------+----------------------------------+------------------------------------+--------------------------------------------------------------+-------------------+

Notes / Note:
-------------

1. Localizzazione con supporto a pagamento tramite partner
2. Manca software per norme fiscali 2017; OCA sta sviluppando il supporto per la Fattura Elettronica B2B
3. Software per Fattura elettronica B2B in sviluppo



|

Usage / Utilizzo
----------------

To graphically design your analysis data-set:

- From the Dashboards menu, select "Custom BI Views"
- Browse trough the business objects in the Query tab
- Pick the interesting fields (Drag & Drop)
- For each selected field, right-click on the Options column and select whether it's a row, column or measure; if you want to remove the field from the list view, unflag the checkbox ´List´ in the Options column
- Save and click "Generate BI View"
- Click "Open BI View" to view the result
- If module Dashboard (board) is installed, the standard "Add to My Dashboard" functionality would be available
- Click "Create a menu" to create a new menu item directly linked to your new BI view (this feature is available in developer mode); when the BI view is reset back to draft this menu will be removed, and you will need to re-create the menu entry.


|

OCA comparation / Confronto con OCA
-----------------------------------

+-----------------------------------------------------------------+-------------------+-----------------------+--------------------------------+
| Description / Descrizione                                       | Odoo Italia       | OCA                   | Notes / Note                   |
+-----------------------------------------------------------------+-------------------+-----------------------+--------------------------------+
| Coverage / Copertura test                                       |  |Codecov Status| | |OCA Codecov Status|  | |OCA project|                  |
+-----------------------------------------------------------------+-------------------+-----------------------+--------------------------------+

|
|

Getting started / Come iniziare
===============================

|Try Me|


Prerequisites / Prerequisiti
----------------------------


* python2.7+
* postgresql 9.2+

|

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

From UI: go to:

* |menu| Setting > Activate Developer mode 
* |menu| Apps > Update Apps List
* |menu| Setting > Apps |right_do| Select **bi_view_editor** > Install

|

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

From UI: go to:

* |menu| Setting > Activate Developer mode
* |menu| Apps > Update Apps List
* |menu| Setting > Apps |right_do| Select **bi_view_editor** > Update

|

Support / Supporto
------------------


|Zeroincombenze| This module is maintained by the `SHS-AV s.r.l. <https://www.zeroincombenze.it/>`__


|
|

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

|
|

Credits / Titoli di coda
========================

Copyright
---------

Odoo is a trademark of `Odoo S.A. <https://www.odoo.com/>`__ (formerly OpenERP)



|

Authors / Autori
----------------

* SHS-AV s.r.l. <https://www.zeroincombenze.it/>

Contributors / Collaboratori
----------------------------

* Simon Janssens <s.janssens@onestein.nl>
* Diego Luis Neto <diegoluis.neto@gmail.com>
* Dennis Sluijk <d.sluijk@onestein.nl>
* Kevin Graveman <k.graveman@onestein.nl>
* Richard Dijkstra <r.dijkstra@onestein.nl>
* Andrea Stirpe <a.stirpe@onestein.nl>
* Antonio Esposito <a.esposito@onestein.nl>
* Jordi Ballester Alomar <jordi.ballester@eficent.com>


|

----------------


|en| **zeroincombenze®** is a trademark of `SHS-AV s.r.l. <https://www.shs-av.com/>`__
which distributes and promotes ready-to-use **Odoo** on own cloud infrastructure.
`Zeroincombenze® distribution of Odoo <https://wiki.zeroincombenze.org/en/Odoo>`__
is mainly designed to cover Italian law and markeplace.

|it| **zeroincombenze®** è un marchio registrato di `SHS-AV s.r.l. <https://www.shs-av.com/>`__
che distribuisce e promuove **Odoo** pronto all'uso sullla propria infrastuttura.
La distribuzione `Zeroincombenze® è progettata per le esigenze del mercato italiano.


|chat_with_us|


|

Last Update / Ultimo aggiornamento: 2019-04-12

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
