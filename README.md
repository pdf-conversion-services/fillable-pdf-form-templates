# Fillable PDF Form Templates

Collect a contact, project purpose and requirements in a reusable interactive form. Download unbranded interactive PDF samples for the United States, United Kingdom and Australia, inspect actual PDF screenshots, or adapt the source.

## Download a fillable template

| Country | Paper and date format | Blank interactive PDF | Completed example screenshot |
|---|---|---|---|
| United States | Letter; MM/DD/YYYY | [Download US template](intake-us-fillable.pdf) | [View US example](intake-us-filled.png) |
| United Kingdom | A4; DD/MM/YYYY | [Download UK template](intake-uk-fillable.pdf) | [View UK example](intake-uk-filled.png) |
| Australia | A4; DD/MM/YYYY | [Download Australia template](intake-au-fillable.pdf) | [View Australian example](intake-au-filled.png) |

![Client intake form with fictional sample entries, rendered directly from an interactive PDF](intake-us-filled.png)

Screenshots show filled examples for illustration. The downloadable PDFs are blank and editable. All names and entries in screenshots are fictional. No sample contains a company name or logo.

## How to use the sample

Choose a template, save a copy, enter the contact details, select a project purpose and describe the information you need to collect. The form uses text fields, a dropdown and a checkbox. It has no automatic submission, calculation or digital signature.

Download the PDF before filling it. Save it, close it, reopen it and check that the values remain. Form support depends on your PDF viewer; test your intended reader before distributing a custom version.

## What is included

- Three country variants of the client intake form.
- Blank and filled screenshots rendered with Poppler, not designed mockups.
- Python source, field schema and automated fill/save/reopen validation results.
- [Usage and quality guide](USAGE.md), [country notes](COUNTRIES.md) and [search intent map](SEARCH-INTENT.md).

## Need a custom version?

For project-specific work, see [custom fillable PDF forms](https://pdfserviceexperts.com/services/fillable-pdf-forms/). Include your source format, approximate volume and desired output when asking for a quote.

## Rebuild and validate

```sh
python -m pip install -r requirements.txt
python build_samples.py
# Optional: install Poppler and put pdftoppm on PATH to regenerate PNGs
python build_samples.py --render
```

The validation checks canonical AcroForm fields, unique page widgets, saved values and appearance streams. Automated checks were run during preparation; interactive clicking in third-party desktop or mobile readers has not been tested. These general business samples have not been audited for PDF/UA, WCAG or jurisdiction-specific compliance. They contain no JavaScript or remote submission actions.

## License

Original templates, screenshots, code and documentation are provided under the [MIT License](LICENSE). External websites retain their own terms and branding.
