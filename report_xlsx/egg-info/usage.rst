An example of XLSX report for partners:

A python class ::

    from odoo.addons.report_xlsx.report.report_xlsx import ReportXlsx

    class PartnerXlsx(ReportXlsx):
    
        def generate_xlsx_report(self, workbook, data, partners):
            for obj in partners:
                report_name = obj.name
                # One sheet by partner
                sheet = workbook.add_worksheet(report_name[:31])
                bold = workbook.add_format({'bold': True})
                sheet.write(0, 0, obj.name, bold)


    PartnerXlsx('report.res.partner.xlsx',
                'res.partner')

To manipulate the ``workbook`` and ``sheet`` objects, refer to the
`documentation <http://xlsxwriter.readthedocs.org/>`_ of ``xlsxwriter``.

A report XML record ::

    <report 
        id="partner_xlsx"
        model="res.partner"
        string="Print to XLSX"
        report_type="xlsx"
        name="res.partner.xlsx"
        file="res.partner.xlsx"
        attachment_use="False"
    />
