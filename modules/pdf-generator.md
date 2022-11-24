# PDF Generator

The "PDF Generator" module enables you to generate PDF files based on any data.

> Please note, templates for generation of PDF files are needed to be individually coded for this module to work. Usually these are coded directly by AtroCore Team or by our Solution Partner.

PDF document can be generated for:
- single item, eg some product
- list of items, eg list of products.

> Please note, templates are created based on HTML/CSS. So anything is possible, what is possible with a modern HTML/CSS technology.

## Administrator Functions

"PDF Generator" module has no administrator settings.

## User Functions 

### PDF Creating for Single Item (e.g. Product)

If a template for creating of PDF for a single item is available following option appears in the actions menu on the detail page of the respective entity:

![pdf-generator-function](./_assets/pdf-generator/pdf-generator-function.png)

Click on "Generate PDF" to open the new window, where you have additional configuration options:

![pdf-generator-popup](./_assets/pdf-generator/pdf-generator-popup.png)

Here you can select the template (if you have more than one), which is/are created for you, select the language for PDF file to be generated (if enabled in the template), select the channel (if enabled in the template), for which the PDF file is determined, and set the file name. You can open the pdf document in a new tab or download it directly with the fine name you have defined previously.

It is also possible to create PDF directly from list page. Open the actions menu for the respective record and choose "generate PDF" for that.

![generate-pdf-item-menu](./_assets/pdf-generator/generate-pdf-item-menu.png)

Generated PDF looks exactly as defined in your template:

![Generated PDF](./_assets/pdf-generator/generated-pdf.jpg)

You can save pdf as an asset (to do it check the checkbox when generating pdf). PDf and asset default names are similar to products name plus SKU (after "-"). You can also select `Asset Category(s)` for your future asset.

![saving-pdf-as-an-asset](_assets/pdf-asset/saving-pdf-as-an-asset-generate.png) 

> Please note, saving PDF as an asset fastens generating new PDFs for this product because new PDFs will be created from an asset.

### PDF Creating for Item List (e.g. Product List)

If a template for the generating of the PDF document for a list of items is created (e.g. product list for some offer etc.) you can select some items, than go actions and select "Generate PDF". 

![generate-pdf-for-selected-items](./_assets/pdf-generator/generate-pdf-for-selected-items.png)

In the new window you can select the template for PDF generation (if you have more than one) and download your PDF:

![pdf-generator-popup-for-list](./_assets/pdf-generator/pdf-generator-popup-for-list.png)
