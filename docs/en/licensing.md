# Licensing

**IN PROGRESS: This section is in the early planning stages and is subject to change. Stay tuned for details.**

Whenever possible, custom-developed code created by California State Government should be licensed for public re-use, subject to the limited exceptions outlined in SAM Section 4819.2. Specifying the license is important because by default no one has permission to use the code. It is necessary to specify the license because otherwise other agencies and individuals will not  know if they have the right to use the code. 

There are few steps you need to take to license any project as open source. Some steps are administrative and some involved adding this to your code base. We are working on developing a template and step-by-step guidance that participating agencies can consider when licensing open source projects. 

## Step 1: Approval

Agencies should follow the review and release process prior to releasing source code.

This requires two approval reviews:

1. **Necessary Rights Review.** Determine if the agency has the rights necessary to release the custom developed code including any pre-existing code owned by third parties under an open source license. If the code base was contributed to solely by state employees while at work the state generally has the rights to release the code as open source. If your code base includes contributions from vendors you may need to review the contract.

2. **Security Risk Review.** Consult with the Agency CIO and Information Security Officer to determine if there are any identifiable security risks according to SAM 4984.2. If the Agency determines that the code will not be publicly released as open source, the particular risks identified must be logged in the code inventory.

## Step 2: Choose a license

When making custom-developed code available to the public as open source software, the agency must attribute these with Copyleft Licenses. Agencies should release all custom developed code under a copyleft such as the "Gnu General Public License v3 or any later version," unless the use of a pre-existing copyleft library requires otherwise. The agency should also make available under the same or compatible copyleft license any documentation or designs associated with the custom-developed code.

If you are making bug fixes or small modifications to a pre-existing code base you should make reasonable efforts to contribute those changes back to the pre-existing code base to minimize the costs associated with the State maintaining a fork of the pre-existing code base. When contributing back to a pre-existing code base you should follow the pre-existing code bases contribution procedures. You may need to consult with your agency counsel prior to contributing back if you need to sign a contributor agreement or use a license other than any version of GNU General Public License. If the original project is not licensed under a copyleft license the Agency, generally contributing modifications to a back to a pre-existing work under the terms of the 3-Clause BSD License or the Apache 2.0 License will be acceptable.

## Step 3: Define contribution process

An essential process for releasing custom code as open source is defining the contribution process. Each agency should adopt a policy describing the procedure for individual members of the general public acting in their own capacity to contribute code to Agency custom-developed code. Each agency should ensure that members of the public who make contributions to the custom developed code.

Two common methods are acceptable:

1. Require that individuals contributing ["sign-off"](https://wiki.linuxfoundation.org/dco) a certification with each contribution that the contribution is done in accordance with the [Developer Certificate of Origin](https://developercertificate.org/) (“DCO”). The DCO is a light way for contributors to certify that the contributor has the right to give the state permission to use their contribution. It is widely used most notably by the Linux Foundation and by the Department of Defense’s Defense Digital Service.

2. Agencies may choose instead to require individuals to submit a individual contributor license agreement prior to their first contribution. The Apache Software Foundation’s [Individual Contributor License Agreement](https://www.apache.org/licenses/icla.pdf) (ICLA) is widely used agreement widely accepted by prominent nonprofits and corporate entities. 

Each agency should adopt a policy describing the procedure for accepting contributions from employees acting or purporting to act on the behalf of other legal entities. If the Agency already has a contract or agreement in place with the legal entity then you should review the agreement to ensure that the agreement grants the Agency the right to release the entities contributions under the open source license used by the project. If there is no agreement in place, the agency should not accept any contributions from the entity or it’s employees until the Agency has an agreement in place granting the agency the rights necessary to release the code under the project’s open source license. The Apache Software Foundation Software Grant and [Corporate Contributor License Agreement](https://www.apache.org/licenses/cla-corporate.pdf) ("Agreement") is a commonly used agreement widely accepted by prominent non-profits and corporate entities.

## Step 4: Add license documents 

You must add the following licensing documents to your project:

1. LICENSE

    1. This file should include the copyright notices for all copyright holders and the full text of all applicable license to the project including a copy of the GNU General Public License version 3 and 

    2. If the State owns the copyright either because it was created by a state employ in the course of their work or by assignment through a vendors contract you must include the following copyright notice including the year (NOTE:  The year should include a list of all of the years in which a copyrightable change to the code base was made. For example if changes when made in 2018 and 2019 then you would list the year as:
 Copyright 2018-2019 State of California
If changes were only made in 2017 and 2019, but not 2018 you would list it as 
 Copyright 2017, 2019 State of California
) (NOTE:  Although common a properly formed copyright notice does not use (c) . You should instead of Copr., Copyright, ©. It is challenging to use © since it is not possible easily to put that in most text files. ):

*Copyright 2019 State of California, Agency Name*

You should also include any other applicable copyright notices in this file as well.

    3. You can find a copy of the GPLv3 here: [https://www.gnu.org/licenses/gpl-3.0.txt](https://www.gnu.org/licenses/gpl-3.0.txt)

2. README

    4. A brief paragraph consisting of 1 to 4 sentences  succinctly describe what the software does (what problem does it solve?).

    5. Your README file must include the following statement clearly indicating the project is being distributed under the terms of the GNU General Public License v3 or any later version.

LICENSE

This project is free and open-source software and is distributed under the terms of the GNU General Public License v3 or any later version. It is subject to the license terms in the LICENSE file found in the top-level directory of this distribution and at http://www.example.org/foo/license.html. By submitting a contribution to this project you agree and acknowledge that your contribution may be used under the terms of the GNU General Public License v3 or any later version and you are authorized to submit the contribution on behalf of the copyright holder. No part of this project, including this file, may be copied, modified, propagated, or distributed except according to the terms contained in the LICENSE file.

    6. Your README file should also include sections on:

        1. **Reporting bugs.** This section should provide information on how State employees, contractors, and the general public can provide feedback (as bug reports or enhancements), and contribute to the software. The most common way is for people to submit Issues on the publicly available GitHub repository.

        2. **Contributing.** This section should  include instructions on how to contribute and explain the contribution process (e.g., are pull requests used?) The instructions should also include the requirements for acceptable contributions (e.g., a reference to any required coding standard or required automated tests) if they exist.

        3. **Getting Started.** This section should include basic documentation on the project or link to the basic documentation stored in a separate file in the code base. The basic documentation should include how to install it, how to start it, how to use it (possibly with a tutorial using examples), and how to use it securely (e.g., what to do and what not to do) if that is an appropriate topic for the software. The security documentation need not be long.

3. When reasonable you should include at the top of each file in the code base the following license notice:

Copyright 2012 The Foo Project Developers. See the LICENSE file at the top-level directory of this distribution and at [http://example.org/project/](http://example.org/project/). No part of the Project, including this file, may be copied, modified, propagated, or distributed except according to the terms contained in the LICENSE file.

## Step 5: Update the inventory

Now that you have all of the pieces in place you need to update the code inventory. If you are not going to release it publically you must still record it in the code inventory.

## Step 6: Release

Publish the code publicly on GitHub, unless a specific identifiable risk has been recorded in the code inventory. 

## Resources

* Sample code bases

    * https://github.com/cagov/sample-repo-java

    * [https://github.com/cagov/sample-repo-csharp](https://github.com/cagov/sample-repo-csharp)

    * https://github.com/cagov/sample-repo-python

* [Best Practices Criteria for Free/Libre and Open Source Software (FLOSS)](https://github.com/coreinfrastructure/best-practices-badge/blob/master/doc/criteria.md)

* [Getting Started](https://code.mil/getting-started.html) (Code.mil)

* [How to Open Source](https://code.mil/how-to-open-source.html) (Code.mil)

* [New Zealand GOAL Software Extension](https://www.ict.govt.nz/assets/Uploads/NZGOAL-Software-Extension-July-2016.pdf)

* [Open source policy](https://18f.gsa.gov/open-source-policy/) - see ‘Open source licenses’ section (18F)
