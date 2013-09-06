proposal-template
=================

A latex proposal / whitepaper template - including a templated BAA required coversheet

NOTE:  The copyright for logo.png belongs to the OpenBSD project.  You should
replace logo.png with your own logo.


Configuration
-------------

There are numerous items you can configure to build the proposal.

If you plan on building a proposal, use the following:
* \proposalcover: Generate a cover page formatted appropriately for US Government BAA responses.  Various fields at the top of proposal.tex will be generated table when uncommented, and will not be displayed when commented out.

If you plan on building a whitepaper, use the following:
* \whitepapercover: Generate a standard document cover page
* \docinfo: Generate a document information page

The following fields should be filed out if you intend on using proposalcover or whitepapercover:

* \projectname:  NOTE, whatever you name your project, add \xspace to the end of the definition, as to make use in future macros work out correctly
* \company: Your Company Name
* \companyref: Your Company reference (big companies need this)
* \companytype: OTHER SMALL BUSINESS
* \team: Companies you are teaming with (N/A if you are on your own)
* \restrictions: Proprietary Information
* \biline: Short phrase describing the project
* \author: Your Name
* \email: your-email@example.com
* \phone: your phone number
* \address: your company address

The following fields should be filed out if you intend on using proposalcover: 

* \baa: BAA-2013-001
* \techarea: Technical Area 1 (Your mom's tech area)
* \doctitle: Volume I (Technical and Management Proposal)
* \cost: \$1,000,000
* \duns: 111111111
* \cagecode: 222222
* \tin: 33-3333333
* \awardtype: Cost Plus Fixed Fee (CPFF)
* \pop: January 1, 2000 - December 31, 2020 (3 days)
* \submitdate: January 1, 2020

Document Controls
-----------------

If you have to restrict release of the document, uncomment the fields from proposal.tex

* \exportcontrol: this includes a blurb about the fact that it is ITAR restricted
* \proposalcontrol: this includes a blurb about the proposal is restricted release for .gov proposal review purposes only

On pages that have restricted information, set the page style to "restricted", which will add appropriate messages to the header and footer.  Note, if the document is classified, change "Proprietary Information" in the restrictions definition to appropriate classification marker.  Example:

    \pagestyle{restricted}
