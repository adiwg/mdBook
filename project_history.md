# Project History

In last few years the International Organization for Standardization (ISO) 19115 family of metadata standards has become the predominantly accepted
worldwide standard for sharing information about the availability and usability of scientific datasets
among researchers.  US interests in the ISO standard have also been growing as global-scale science
demands participation with the broader international community.  Yet, due to the complexity and rigor of
the ISO metadata standards, adoption has been slow. In addition, support for data content in current
implementations of the standard has been minimal.

In 2009 the Alaska Data Integration working group members (ADIwg) mobilized to jointly address the
common data integration efforts.  Beginning in 2012, ADIwg started to focus on difficulties associated
with generating and exchanging ISO 19115-2 metadata among its partners which vary in size, from small
NGO research groups to state offices, universities, and large federal bureaus.  This differential in size and technical capabilities among its membership brings with it a diversity in metadata requirements and the ability to provide the necessary technical support to its researchers.
The ISO 19115 metadata standard is not a single standard but a family of ISO and GML (Geography
Markup Language Encoding Standard published and maintained by the Open Geospatial Consortium,
Inc.) standards.  Understanding this amalgamation of standards to a degree sufficient to generate a valid
metadata record requires an investment of time well beyond what should be reasonably expected of any
PI or end user.  These issues are not specific to ADIwg and its members; they are shared by many
organizations striving to transition to the ISO metadata standard.

#Project Scope

After much discussion, the ADIwg membership agreed to co-author a software toolkit with an
architecture that has the flexibility to achieve the following goals:

 - Isolate the complexity, rigor, formatting, and terminology of the ISO standards from the user.  Users should not be required to know anything about the ISO standards.
 - Provide clear developer and user documentation.
 - Design a layered architecture so developers will have access to each layer. Developers should be
able to enter the toolkit at whatever layer best fits their needs; e.g. download the code library to
do some custom programming or post JSON metadata to a hosted JSON to ISO translator.
 - Design the architecture to accommodate incremental development cycles. Add features without
disrupting previous implementations.
 - Implement all code and services as open-source software projects using a GitHub repository.
 - Use simple JSON (JavaScript Object Notation) for storing and transferring user metadata.
 - Provide flexibility to write to multiple metadata standards, including ISO 19115-2:2009, 19115-
1:2014, 19110, and possibly FGDC.
 - Provide an online, interactive metadata editor written in JavaScript to gather and edit a
user’s metadata and format it in the mdJson format.
 - Host a publicly available version of the online metadata editor for end users to enter and edit
metadata then request a valid ISO standard metadata record to be returned.
 - All code should be written in a popular computer language, be platform independent, royalty-free,
and available through an open-source repository to encourage participation from and benefit to
the widest possible user base.

To be clear, these tools are for the generation metadata only.  This project is not intended to provide
services as a metadata clearinghouse, metadata storage, or search and modify capabilities.
