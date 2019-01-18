# Workflow

**IN PROGRESS: This section is in the early planning stages and is subject to change. Stay tuned for details.**

Updated 01-17-19

Publishing California state government open source projects to code.ca.gov adopts the code.json data management protocol, the same employed by the U.S. Government’s [code.gov](https://code.gov) and NASA’s [code.nasa.gov](https://code.nasa.gov).

## code.json

As code.gov and code.nasa.gov do, code.ca.gov will leverage the JSON protocol to publish publicly-available state open source projects.

About JSON:

*In computing, JavaScript Object Notation or JSON is an open-standard file format that uses human-readable text to transmit data objects consisting of attribute–value pairs and array data types (or any other serializable value). It is a very common data format used for asynchronous browser–server communication. ([Wikipedia](https://en.wikipedia.org/wiki/JSON)*)

The code.json file allows agencies to create a simple file from an established template, input information related to all of the organization’s public open source projects (i.e., repositories), then post this file on its primary website for data harvesting into the code.ca.gov platform.

## code.json Placement
Each code.json file needs to be placed in a public facing location where the raw json can be read. This can be accomplished by either placing the file on github and using a raw link [(example)](https://raw.githubusercontent.com/ODI-BPA/code.ca.gov/master/code.json) or the file can be placed in a publicly available location on an agencies website.

## Updating the Metadata Location File
In order for Code.ca.gov to inventory agency code, a single source with reference to each code.json file is necessary.

We house this file on [GitHub](https://github.com/ODI-BPA/code.ca.gov/blob/master/remote_metadata.json) . To update this file with the location of a new code.json file, make a pull request with the new changes and we will review and merge the changes.

## Resources

California will leverage existing tools and resources created through the federal government’s Code.gov team:

* [Creating your enterprise code inventory](https://code.gov/#!/policy-guide/docs/compliance/inventory-code) (code.gov)

* [code.json template](https://github.com/GSA/code-gov-web/blob/master/src/assets/sample_code_200.json)

* [code.json generators](https://github.com/GSA/code-gov/blob/master/CODE_JSON_GENERATORS.md)

    * [Scraper](https://github.com/LLNL/scraper) (U.S. Department of Energy - LLNL)

    * [Code-JSON Generator](https://github.com/usgs/code-json-generator) (U.S. Department of Interior - USGS)

    * [Code Inventory](https://github.com/GSA/codeinventory-github) (U.S. General Services Administration)

    * [Code-Inventory Generator](https://github.com/cfpb/code-inventory-generator) (Consumer Financial Protection Bureau)

* [code.gov Harvester](https://github.com/GSA/code-gov-harvester)

* [code.json Validator](https://code.gov/#!/policy-guide/docs/compliance/inventory-code/tools/validate-schema)
