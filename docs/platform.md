# Platform

**IN PROGRESS: This section is in the early planning stages and is subject to change. Stay tuned for details. **

Updated 01-17-19

[Code.ca.gov](https://code.ca.gov/) is the central platform for finding California government open source software projects. CDT is leveraging and learning from existing efforts from the federal team at code.gov to create the next iteration of code.ca.gov.

The code.ca.gov platform follows similar government efforts:

* U.S. Government ([code.gov](https://code.gov/))

* National Aeronautics and Space Administration ([code.nasa.gov](https://code.nasa.gov/))

## Acknowledgements

We would like to recognize and thank the team that develops and supports the U.S. Government's open source platform [code.gov](http://code.gov). By leveraging the [code.gov](http://code.gov) code base, we join a broader community and hold true to the spirit of open source collaboration.

## How We Inventory Code on Code.ca.gov

Code.ca.gov works by first harvesting a list of all inventoried code from a single source that is hosted on [Github](https://github.com/ODI-BPA/code.ca.gov/blob/master/remote_metadata.json).

From that file, we run through each agencies entry and fetch their associated json file. We then index each json file and make the open source code available and searchable on our platform.


## Planned Features

Key code.ca.gov planned features:

* Projects: Filterable view (by technology, agency, license) of California state software projects.

* Developer: The ‘Developer’ page includes documentation on:

    * How (internal/external) developers can get involved

    * How agencies can set up their code.json file

* Help wanted: The ‘Help Wanted’ functionality flags key project issues the state is seeking collaboration on.

* Feedback: The universal ‘Feedback’ link allows users to easily and publicly submit comments, bugs, etc., encouraging a culture of collaboration and accessibility.

* Roadmap: The project roadmap with general planned features.

* Dashboard: The participation dashboard showcases open source software adoption.
