# 3. BioSamples

## Preamble
Originally the BioSamples database was where metadata describing sequence data
submitted to ENA was stored. Today it is a standalone repository where sample
metadata can be accessioned even if not associated with sequence data. While you
can still obtain a new BioSamples accession by submitting sample metadata in
conjuction with sequence data to ENA, this is considered a legacy mechanism.
Submitters are now encouraged to first register a BioSamples accesssion and
reference the accession when submitting derived sequence data to ENA.

Because of it's origins and wide range of potential metadata than can be
included to describe a sample - note that a sample may be many different types of
artefact, not just DNA samples - data submitted to BioSamples must be in the
form of a spreadsheet of values with each row being a separate sample. That is
to say, there is no online form where you can fill in data values, rather you
create the spreadsheet of data offline then drop the file into the submission
box. There is also an extensive API for submitting sample records
programmatically - [a guide can be found here](https://read-docs-biosamples.readthedocs.io/en/latest/submit/programmatically.html).

## How to register one or many BioSamples accessions

The Biosamples [step-by-step guide can be found here](https://read-docs-biosamples.readthedocs.io/en/latest/submit/interactively/step-by-step.html).

The BioSamples submission data are based on a number of checklists that define
mandatory data fields for different data, and project data types. These
checklists are described [here](https://www.ebi.ac.uk/ena/browser/checklists).
For EUREMAP projects, we recommend you [use this checklist](https://raw.githubusercontent.com/cymon/euremap-data-management-book/refs/heads/main/book/EUREMAP-Default-Sample-Checklist-ERC000011.tsv)
template that is based on the [ENA default sample checklist (ERC000011)](https://www.ebi.ac.uk/ena/browser/view/ERC000011).
You can of course add additional fields to the submission if necessary, but you
should understand what you are doing.

In the checklist template spreadsheet, the *term* in the columns labeled
"Characteristic[*term*]" are the "Field Name" identified in the checklist e.g.
[ERC000011](https://www.ebi.ac.uk/ena/browser/view/ERC000011). From the
checklist you can identifiy which fields are mandatory. Each
"Characteristic[*term*]" column is followed by two further columns labeled "Term
Source REF" and "Term Accession Number". If you don't know what these mean,
leave them blank - **BUT** they must still be included in the submission spreadsheet.

Please note that the spreadsheet must be in tab-separated format (TSV) and all
columns in the template should be included even if left blank.



