---
title: Discovering Metadata
layout: default
permalink: /discovering-metadata
---

<h1>Metadata</h1>
<p>Data.gov.au uses components of the <a href="http://www.agls.gov.au/">AGLS</a>, <a href="http://dublincore.org/">Dublin Core</a> and <a href="http://www.w3.org/TR/vocab-dcat/">Data Catalog Vocabulary</a> metadata standards as per below. Finance are doing analysis on this approach and expect to improve upon the metadata approach to get consistency of discovery data across all data types. This work is being done in collaboration with several entities and the Australian Government Linked Data Working Group.
</p><p>See the <a href="http://webguide.gov.au/web-2-0/publishing-public-sector-information/">Publishing PSI guide</a> for more information on metadata.
</p><p>You can download a copy of metadata and other schemas used by data.gov.au from the <a href="https://data.gov.au/dataset/data-gov-au-metadata-and-other-schemas">metadata and other schemas dataset on data.gov.au</a>
</p>
<h2>Metadata Fields</h2>
<h3>Metadata Mapping</h3>
<table >

<tbody><tr>
<th>Human Readable Name
</th>
<th>AGLS Map
</th>
<th>DCAT Map
</th>
<th>ANZLIC Map
</th>
<th>G8 ODC Map
</th></tr>
<tr>
<td>Title
</td>
<td>agls:title
</td>
<td>dcat:Dataset/dct:title
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.citation:CI_Citation.title
</td>
<td>2.8.M Title
</td></tr>
<tr>
<td>Description
</td>
<td>agls:description
</td>
<td>dcat:Dataset/dct:description
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.abstract
</td>
<td>2.5.M Description
</td></tr>
<tr>
<td>Keyword
</td>
<td>agls:subject
</td>
<td>dcat:Dataset/dct:keyword
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.topicCategory:MD_TopicCategoryCode<br>
<p>MD_Metadata.identificationInfo:MD_DataIdentification.descriptiveKeywords:MD_Keywords.keyword
</p>
</td>
<td>2.6.M Keyword
</td></tr>
<tr>
<td>Theme
</td>
<td>agls:function
</td>
<td>dcat:Dataset/dcat:theme
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.topicCategory:MD_TopicCategoryCode<br>
<p>MD_Metadata.identificationInfo:MD_DataIdentification.descriptiveKeywords:MD_Keywords.keyword
</p>
</td>
<td>2.9.M Category
</td></tr>
<tr>
<td>Language
</td>
<td>agls:language
</td>
<td>dcat:Dataset/dct:language
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.language
</td>
<td>5.7.M Language
</td></tr>
<tr>
<td>Licence
</td>
<td>agls:license
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dct:license
</p>
</td>
<td>MD_LegalConstraints
</td>
<td>5.1.M Licence
</td></tr>
<tr>
<td>Rights
</td>
<td>agls:rights
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:rights
</p>
</td>
<td>MD_Metadata.identificationInfo.resourceConstraints.useLimitation; MD_LegalConstraints (with MD_REstrictionCode = 'copyright' or 'intellectualPropertyRights')
</td>
<td>5.2.M Copyright
</td></tr>
<tr>
<td>Data Status
</td>
<td>-
</td>
<td>-
</td>
<td>MD_Metadata.identificationInfo:MD_Identification.status
</td>
<td>-
</td></tr>
<tr>
<td>Update Frequency
</td>
<td>-
</td>
<td>dcat:Dataset/dct:accrualPeriodocity
</td>
<td>MD_MaintenanceInformation.maintenanceAndUpdateFrequency in 19115 (have not checked ANZLIC profile)
</td>
<td>2.7.H Frequency of Update
</td></tr>
<tr>
<td>Expose User Contact Information
</td>
<td>-
</td>
<td>-
</td>
<td>-
</td>
<td>-
</td></tr>
<tr>
<td>Landing page
</td>
<td>agls:identifier<br>
<p>agls:source
</p>
</td>
<td>dcat:Dataset/dcat:landingPage
</td>
<td>anzlic:linkage<br>
<p>MD_DigitalTransferOptions.onLine:CI_Onlineresoiurce.linkage:URL
</p>
</td>
<td>4.1.M Documentation URL - resource
</td></tr>
<tr>
<td>Publish date
</td>
<td>agls:date
</td>
<td>dcat:Dataset/dct:issued
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.citation:CI_Citation.date:CI_Date.date where CI_Date.dateType = 'publication'
</td>
<td>2.2.M Release Date
</td></tr>
<tr>
<td>Update date
</td>
<td>agls:modified
</td>
<td>dcat:Dataset/dct:modified
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.citation:CI_Citation.date:CI_Date.date where CI_Date.dateType = 'revision'
</td>
<td>2.3.M Modified
</td></tr>
<tr>
<td>Identifier
</td>
<td>agls:fileIdentifier
</td>
<td>dcat:Dataset/dct:identifier
</td>
<td>MD_Metadata.fileIdentifier
</td>
<td>2.1.M Unique Identifier
</td></tr>
<tr>
<td>Metadata URI
</td>
<td>-
</td>
<td>-
</td>
<td>MD_Metadata.dataSetURI
</td>
<td>-
</td></tr>
<tr>
<td>Download URL
</td>
<td>agls:identifier
</td>
<td>dcat:Dataset/dcat:distribution/dcat:Distribution/dcat:downloadURL
</td>
<td>MD_Metadata.datasetURI or MD_DigitalTransferOptions.onLine:CI_Onlineresoiurce.linkage:URL
</td>
<td>5.4.M URL - resource
</td></tr>
<tr>
<td>File size
</td>
<td>agls:SizeorDuration
</td>
<td>dcat:Dataset/dcat:distribution/dcat:Distribution/dcat:byteSize
</td>
<td>MD_DigitalTransferOptions.transferSize
</td>
<td>5.3.M Size
</td></tr>
<tr>
<td>Access URL
</td>
<td>agls:identifier<br>
<p>agls:source
</p>
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:accessURL
</p>
</td>
<td>anzlic:linkage.URL Also CI_OnlineResource (19115) MD_DigitalTransferOptions.onLine:CI_Onlineresoiurce.linkage:URL
</td>
<td>5.4.M URL - resource
</td></tr>
<tr>
<td>Media type
</td>
<td>-
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:mediaType
</p>
</td>
<td>MD_Metadata.identificationInfo.resourceFormat:MD_Format.name<br> MD_Metadata.identificationInfo.resourceFormat:MD_Format.version (version is mandatory in the ISO 19115/ANZLIC if a format name is specified)<br>
<p>MD_Metadata.identificationInfo.distributionFormat:MD_Format.name<br> MD_Metadata.identificationInfo.distributionFormat:MD_Format.version
</p>
</td>
<td>5.6.M Format - resource
</td></tr>
<tr>
<td>Format
</td>
<td>agls:medium<br>
<p>agls:format
</p>
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:format
</p>
</td>
<td>MD_Metadata.identificationInfo.resourceFormat:MD_Format.name<br>
<p>MD_Metadata.identificationInfo.resourceFormat:MD_Format.version (version is mandatory in the ISO 19115/ANZLIC if a format name is specified)<br>
MD_Metadata.identificationInfo.distributionFormat:MD_Format.name<br>
MD_Metadata.identificationInfo.distributionFormat:MD_Format.version<br>
MD_Metadata.identificationInfo:MD_Distribution:MediumName
</p>
</td>
<td>5.6.M Format - resource
</td></tr>
<tr>
<td>Publisher
</td>
<td>agls:corporateName
</td>
<td>dct:publisher<br>
<p>(foaf:agent)
</p>
</td>
<td>MD_Metadata.contact:CI_Responsibleparty.organisationName<br>
<p>MD_Metadata.identificationInfo:MD_DataIdentification.citation:CI_Citation.citedResponsibleParty:CI_ResponsibleParty
</p>
</td>
<td>1.4.M Publisher<br>
<p>1.3.M Organisation (Owner)
</p>
</td></tr>
<tr>
<td>Contact
</td>
<td>agls:AglsAgent
</td>
<td>dcat:contactPoint (vCard)
</td>
<td>MD_Metadata.contact:CI_ResponsibleParty.organisationName
</td>
<td>1.1.M Person<br>
<p>1.2.M Contact Email - Dataset
</p>
</td></tr>
<tr>
<td>Data Portal
</td>
<td>-
</td>
<td>-
</td>
<td>-
</td>
<td>-
</td></tr>
<tr>
<td>Jurisdiction
</td>
<td>agls:jurisdiction
</td>
<td>-
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.extent:EX_Extent:EX_GeographicDescription
</td>
<td>3.4.M Geographic Region Name
</td></tr>
<tr>
<td>Homepage
</td>
<td>agls:agentterms:web
</td>
<td>dct:publisher (foaf:homePage)
</td>
<td>19115:CI_Contact/onlineResource.linkage
</td>
<td>5.5.M Homepage URL
</td></tr>
<tr>
<td>Publisher (User Account)
</td>
<td>-
</td>
<td>dct:publisher (foaf:agent)
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.citation:CI_Citation.citedResponsibleParty:CI_ResponsibleParty
</td>
<td>1.4.M Publisher
</td></tr>
<tr>
<td>Contact(User Account)
</td>
<td>agls:AglsAgent
</td>
<td>dcat:contactPoint (vCard)
</td>
<td>MD_Metadata.contact:CI_ResponsibleParty.organisationName
</td>
<td>1.1.M Person<br>
<p>1.2.M Contact Email - Dataset
</p>
</td></tr>
<tr>
<td>Temporal coverage from
</td>
<td>agls:temporal<br>
<p>agls:coverage
</p>
</td>
<td>dcat:Dataset/dct:temporal
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.extent:EX_Extent.temporalElement
</td>
<td>3.10.M Temporal coverage starts
</td></tr>
<tr>
<td>Temporal coverage to
</td>
<td>agls:temporal<br>
<p>agls:coverage
</p>
</td>
<td>dcat:Dataset/dct:temporal
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.extent:EX_Extent.temporalElement
</td>
<td>3.11.M Temporal coverage ends
</td></tr>
<tr>
<td>Geospatial coverage
</td>
<td>agls:spatial
</td>
<td>dcat:Dataset/dct:spatial
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.extent:EX_Extent:EX_GeographicDescription
</td>
<td>3.1.M Spatial coverage
</td></tr>
<tr>
<td>ISO19115 Topic
</td>
<td>agls:subject
</td>
<td>dcat:Dataset/dcat:theme
</td>
<td>19115 MD_TopicCategoryCode
</td>
<td>-
</td></tr>
<tr>
<td>Field(s) of Research
</td>
<td>-
</td>
<td>dcat:Dataset/dcat:theme
</td>
<td>MD_Metadata.identificationInfo:MD_DataIdentification.descriptiveKeywords:MD_Keywords.keyword<br> MD_Metadata.identificationInfo:MD_DataIdentification.descriptiveKeywords:MD_Keywords.thesaurusName (e.g. New Zealand Standard Research Classification (ANZSRC), 2008)
</td>
<td>-
</td></tr>
<tr>
<td>Data Models
</td>
<td>-
</td>
<td>-
</td>
<td>-
</td>
<td>-
</td></tr>
</tbody></table>
<h3>Dataset</h3>
<table>

<tbody><tr>
<th>Human Readable Name
</th>
<th>Class Attribute
</th>
<th>Description
</th>
<th>Example
</th>
<th>Vocab Control
</th>
<th><i>Commonwealth Definition</i>
</th>
<th>System Generated
</th>
<th>Mandatory
</th>
<th>Repeatable
</th></tr>
<tr>
<td>Title
</td>
<td>dcat:Dataset/dct:title
</td>
<td>Title of dataset
</td>
<td>Location of Medicare offices
</td>
<td>Free text
</td>
<td><i>N/A</i>
</td>
<td>No
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Description
</td>
<td>dcat:Dataset/dct:description
</td>
<td>Description of the dataset
</td>
<td>The Department of Human Services Service Centre locator contains information updated weekly, a search function and maps.
</td>
<td>Free text
</td>
<td><i>N/A</i>
</td>
<td><b>No</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Keyword
</td>
<td>dcat:Dataset/dct:keyword
</td>
<td>Keywords, subjects, topics of dataset
</td>
<td>health, health-care
</td>
<td>Free text tagging with autocompletion / LCSH
</td>
<td><i>N/A</i>
</td>
<td><b>No</b>
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr>
<td>Theme
</td>
<td>agls:function
</td>
<td>The government jurisdiction defined business function to which the resource relates
</td>
<td>Communications, broadcasting standards
</td>
<td><a href="http://www.naa.gov.au/records-management/publications/agift.aspx">Limited choice</a>
</td>
<td><i>AGIFT top level categories</i>
</td>
<td><b>No - selected from a list (list defined per jurisdiction)</b>
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr>
<td>Language
</td>
<td>dcat:Dataset/dct:language
</td>
<td>If not English, language should be assigned a value
</td>
<td>en
</td>
<td>Language codes (consider user of <a href="http://www.ietf.org/rfc/rfc4646.txt">RFC4646</a>)
</td>
<td><i>en</i>
</td>
<td><b>Yes (default set, but changable)</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Licence
</td>
<td>dcat:Dataset/dcat:distribution
<p>dcat:Distribution/dct:license
</p>
</td>
<td>License details
</td>
<td>Creative Commons Attribution 3.0 Australia
</td>
<td>Predefined list determined by the jurisdiction.
</td>
<td><i>As currently defined</i>
</td>
<td><b>No - selected from a list</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Rights
</td>
<td>dcat:Dataset/dcat:distribution
<p>dcat:Distribution/dcat:rights
</p>
</td>
<td>Will automatically populate based on what is chosen in the license field.
</td>
<td>
</td>
<td>Text (automatic)
</td>
<td>
</td>
<td><b>No</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Data Status
</td>
<td>Boolean
</td>
<td>The status of the data with regard to whether it is kept updated (active, yes) or historic (inactive, no)
</td>
<td>Active
</td>
<td>Limited choice
</td>
<td><i>Active</i>
<p><i>Inactive</i>
</p>
</td>
<td><b>No</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Update Frequency
</td>
<td>dcat:Dataset/dct:accrualPeriodocity
</td>
<td>How often the dataset is updated
</td>
<td>Daily
</td>
<td>Limited choice
</td>
<td><i>Daily</i>
<p><i>Weekly</i><br>
<i>Monthly</i><br>
<i>Quarterly</i><br>
<i>Yearly</i><br>
<i>As Required</i>
</p>
</td>
<td><b>No</b>
</td>
<td>Yes - conditional on Active Status
</td>
<td>No
</td></tr>
<tr>
<td>Expose User Contact Information
</td>
<td>
</td>
<td>Whether the user contact details should be exposed as well as the organisation contact details. Relevant only to researcher/scientist users who want
</td>
<td>No
</td>
<td>Limited choice
</td>
<td><i>Yes</i>
<p><i>No</i>
</p>
</td>
<td><b>No</b>
</td>
<td>Yes - is selected as "No" by default
</td>
<td>No
</td></tr>
<tr>
<td colspan="9"><i> <b>NOTE: the rest of the dataset-specific attributes are automatically generated</b> </i>
</td></tr>
<tr>
<td>Landing page
</td>
<td>dcat:Dataset/dcat:landingPage
</td>
<td>URL with information on resource.
</td>
<td><a href="https://data.gov.au/dataset/559708e5-480e-4f94-8429-c49571e82761">https://data.gov.au/dataset/559708e5-480e-4f94-8429-c49571e82761</a>
</td>
<td>URL - Automatically generated from system. Must be the UUID URL.
</td>
<td><i>N/A</i>
</td>
<td><b>Yes</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Publish date
</td>
<td>dcat:Dataset/dct:issued
</td>
<td>Original publish date of record
</td>
<td>1994-11-05T08:15:30-05:00
</td>
<td>Datetime - automated
</td>
<td><i><a href="http://www.w3.org/TR/NOTE-datetime">ISO 8601</a></i>
</td>
<td><b>Yes</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Update date
</td>
<td>dcat:Dataset/dct:modified
</td>
<td>Date modified
</td>
<td>1994-11-05T08:15:30-05:00
</td>
<td>Date - automated (date of most recently updated resource)
</td>
<td><i><a href="http://www.w3.org/TR/NOTE-datetime">ISO 8601</a></i>
</td>
<td><b>Yes</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Identifier
</td>
<td>dcat:Dataset/dct:identifier
</td>
<td>The fileIdentifier for a metadata record must never change, irrespective of where that metadata record is stored. Should be system generated. In CKANs case the UUID is common to dataset and metadata record, and takes the UUID with it across new systems.
</td>
<td><a href="URN:UUID">URN:UUID</a> (example 559708e5-480e-4f94-8429-c49571e82761)
</td>
<td>Automatically generaled unique ID. Decided against DOI as unique ID already generated in CKAN. DOI records created in ANDS can be leveraged for those who want them given data.gov.au metadata to be harvested by ANDS.
</td>
<td><i>N/A</i>
</td>
<td><b>Yes</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Metadata URI
</td>
<td>MD_Metadata.dataSetURI
</td>
<td>Automatically generated metadata URI.
</td>
<td><a href="https://data.gov.au/dataset/559708e5-480e-4f94-8429-c49571e82761.rdf">https://data.gov.au/dataset/559708e5-480e-4f94-8429-c49571e82761.rdf</a>
</td>
<td>
</td>
<td><i>N/A</i>
</td>
<td><b>Yes</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
</tbody></table>
<p><br>
</p>
<h3>Individual Resources (within datasets)</h3>
<table>

<tbody><tr>
<th>Human Readable Name
</th>
<th>Class Attribute
</th>
<th>Description
</th>
<th>Example
</th>
<th>Vocab Control
</th>
<th><i>Commonwealth Definition</i>
</th>
<th>System Generated
</th>
<th>Mandatory
</th>
<th>Repeatable
</th></tr>
<tr>
<td>Download URL
</td>
<td>dcat:dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:downloadURL
</p>
</td>
<td>URL with information on resource.
</td>
<td><a href="https://data.gov.au/dataset/559708e5-480e-4f94-8429-c49571e82761">https://data.gov.au/dataset/559708e5-480e-4f94-8429-c49571e82761</a>
</td>
<td>URL - Automatically generated from system. Must be the UUID URL.
</td>
<td><i>N/A</i>
</td>
<td><b>Yes</b>
</td>
<td>Conditional
</td>
<td>No
</td></tr>
<tr>
<td>File size
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:byteSize
</p>
</td>
<td>Conditional if download URL is used. Automatically generated from the system where locally hosted, otherwise numerical entry.
</td>
<td>84MB
</td>
<td>Automatically generated
</td>
<td><i>N/A</i>
</td>
<td><b>Yes</b>
</td>
<td>Conditional
</td>
<td>No
</td></tr>
<tr>
<td>Access URL
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:accessURL
</p>
</td>
<td>Conditional: Use Access URL when resource is not a direct download (i.e. index page, SPARQL endpoint, feed etc.)
</td>
<td><a href="https://data.gov.au/geoserver/geelong-trees/wfs?request=GetCapabilities">https://data.gov.au/geoserver/geelong-trees/wfs?request=GetCapabilities</a>
</td>
<td>URL
</td>
<td><i>N/A</i>
</td>
<td><b>Yes</b>
</td>
<td>Conditional
</td>
<td>No
</td></tr>
<tr>
<td>Media type
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:mediaType
</p>
</td>
<td>Conditional: Media type of distribution as defined by IANA
</td>
<td>text/csv
</td>
<td>Automatically generated based on file type from IANA defitions - <a href="http://www.iana.org/assignments/media-types/media-types.xhtml">http://www.iana.org/assignments/media-types/media-types.xhtml</a>
</td>
<td><i>IANA definitions</i>
</td>
<td><b>Yes</b>
</td>
<td>Conditional
</td>
<td>No
</td></tr>
<tr>
<td>Format
</td>
<td>dcat:Dataset/dcat:distribution<br>
<p>dcat:Distribution/dcat:format
</p>
</td>
<td>Conditional:File format of the distribution. If available in IANA, use Media Type
</td>
<td>
</td>
<td>Free text
</td>
<td><i>N/A</i>
</td>
<td><b>No - conditional only if media type isn't automatically detected.</b>
</td>
<td>Conditional
</td>
<td>No
</td></tr>
</tbody></table>
<h3>Entity</h3>
<table>

<tbody><tr>
<th>Human Readable Name
</th>
<th>Class Attribute
</th>
<th>Description
</th>
<th>Example
</th>
<th>Vocab Control
</th>
<th><i>Commonwealth Definition</i>
</th>
<th>System Generated
</th>
<th>Mandatory
</th>
<th>Repeatable
</th></tr>
<tr>
<td>Publisher
</td>
<td>dct:publisher<br>
<p>(foaf:agent)
</p>
</td>
<td>Name of the Entity/publishing organisation. Controlled via CKAN accounts.
</td>
<td>Department of Human Services
</td>
<td>Automatically taken from "Organisation", able to be modified.
</td>
<td><i>N/A</i>
</td>
<td><b>Yes - inherited from organisation information. Able to be overridden</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Contact
</td>
<td>dcat:contactPoint<br>
<p>(vCard)
</p>
</td>
<td>Contact details of the publishing organisation. Controlled via CKAN accounts. Inc full name, telephone, email
</td>
<td>FN: Spatial Team<br>
<p>Tel Type: work<br>
Tel: xx xxx xxxx<br>
Email: spatial@entity.gov.au
</p>
</td>
<td>Automatically taken from additional metadata added to the CKAN "Organisation" with these details able to be modified.
</td>
<td><i>N/A</i>
</td>
<td><b>Yes - inherited from organisation information. Able to be overridden</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Data Portal
</td>
<td>
</td>
<td>Which data portal, necessary for representing search results in search federation project.
</td>
<td><a href="https://data.gov.au/">https://data.gov.au/</a>
</td>
<td>Automatic, drawn from data portals.
</td>
<td><i><a href="https://data.gov.au/">https://data.gov.au/</a></i>
</td>
<td><b>Yes - inherited from system.</b>
</td>
<td>Yes
</td>
<td>Yes
</td></tr>
<tr>
<td>Jurisdiction
</td>
<td>agls:jurisdiction
</td>
<td>Which Australian Government Jurisdiction
</td>
<td>Commonwealth of Australia, New South Wales, Adelaide City Council, Etc
</td>
<td>Drop down choice of jurisdiction.
</td>
<td><i>"Commonwealth of Australia" and any existing jurisdictions already on data.gov.au. To add as required.</i>
</td>
<td><b>Yes - inherited from organisation information, available from list. Able to be overridden</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Homepage
</td>
<td>dct:publisher<br>
<p>(foaf:homePage)
</p>
</td>
<td>Entity/Publisher homepage
</td>
<td><a href="http://www.humanservices.gov.au/">http://www.humanservices.gov.au/</a>
</td>
<td>Automatically taken from homepage of the "Organisation".
</td>
<td><i>N/A</i>
</td>
<td><b>Yes - inherited from organisation information, available from list. Able to be overridden</b>
</td>
<td>No
</td>
<td>No
</td></tr>
</tbody></table>
<h3>User Account</h3>
<table>

<tbody><tr>
<th>Human Readable Name
</th>
<th>Class Attribute
</th>
<th>Description
</th>
<th>Example
</th>
<th>Vocab Control
</th>
<th><i>Commonwealth Definition</i>
</th>
<th>System Generated
</th>
<th>Mandatory
</th>
<th>Repeatable
</th></tr>
<tr>
<td>Publisher
</td>
<td>dct:publisher<br>
<p>(foaf:agent)
</p>
</td>
<td>Name of the individual who has published the data in the organisation. Controlled via CKAN accounts.
</td>
<td>Bruce Wayne
</td>
<td>Automatically taken from the user account. Only enabled for public visibility if chosen by the user on a dataset by dataset basis. Only likely to be taken up by scientists and those who want personal citation.
</td>
<td><i>N/A</i>
</td>
<td><b>Yes - inherited from user details.</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Contact
</td>
<td>dcat:contactPoint<br>
<p>(vCard)
</p>
</td>
<td>Contact details of the publisher. Controlled via CKAN accounts. Inc full name, telephone, email.
</td>
<td>FN: Joe Bloggs<br>
<p>Tel Type: work<br>
Tel: xx xxx xxxx<br>
Email: info@entity.com
</p>
</td>
<td>Automatically taken from additional metadata added to the CKAN "Organisation" with these details able to be modified.
</td>
<td><i>N/A</i>
</td>
<td><b>Yes - inherited from user details.</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
</tbody></table>
<h3>Extent</h3>
<table>

<tbody><tr>
<th>Human Readable Name
</th>
<th>Class Attribute
</th>
<th>Description
</th>
<th>Example
</th>
<th>Vocab Control
</th>
<th><i>Commonwealth Definition</i>
</th>
<th>System Generated
</th>
<th>Mandatory
</th>
<th>Repeatable
</th></tr>
<tr>
<td>Temporal coverage from
</td>
<td>dcat:Dataset/dct:temporal
</td>
<td>Start of temporal series in dataset. If only a point in time, then the user doesn't fill in the "to" temporal coverage. Can make it very usef friendly
</td>
<td>2001/10/1
</td>
<td>Date
</td>
<td><i><a href="http://www.w3.org/TR/NOTE-datetime">ISO 8601</a></i>
</td>
<td><b>No</b>
</td>
<td>Yes
</td>
<td>No
</td></tr>
<tr>
<td>Temporal coverage to
</td>
<td>dcat:Dataset/dct:temporal
</td>
<td>End of temporal series used in dataset
</td>
<td>2001/10/2
</td>
<td>Date
</td>
<td><i><a href="http://www.w3.org/TR/NOTE-datetime">ISO 8601</a></i>
</td>
<td><b>No</b>
</td>
<td>Conditional
</td>
<td>No
</td></tr>
<tr>
<td>Geospatial coverage
</td>
<td>dcat:Dataset/dct:spatial
</td>
<td>Spatial description of resource (gazetteer)
</td>
<td>Sydney
</td>
<td>Free text with a <b>mandatory</b> requirement to use one of the following:<br>
<ol><li>a point/polygon (WKT);</li>
<li>an administrative boundary API; or,</li>
<li>a reference URL (website address) from the <a href="http://www.ga.gov.au/place-names/">National Gazatteer</a>. Gazetteer reference URLs can be found by searching for a place at <a href="http://www.ga.gov.au/place-names/">http://www.ga.gov.au/place-names/</a> then clicking through to the most appropriate location "Reference ID", and then copying and pasting the URL from the page into the Geospatial field in data.gov.au.</li></ol>
</td>
<td><i>N/A but with explanatory text linking to Gazatteer and WKT information and strongly recommending either a Gazatteer record ID link or a point/polygon definition.</i>
</td>
<td><b>No</b>
</td>
<td>Yes - default to the Jurisdiction by default (Australia, South Australia, Geelong, etc)
</td>
<td>No
</td></tr>
</tbody></table>
<h3>Additional Commonwealth Specific Options</h3>
<table>

<tbody><tr>
<th>Human Readable Name
</th>
<th>Class Attribute
</th>
<th>Description
</th>
<th>Example
</th>
<th>Vocab Control
</th>
<th><i>Commonwealth Definition</i>
</th>
<th>System Generated
</th>
<th>Mandatory
</th>
<th>Repeatable
</th></tr>
<tr>
<td>ISO19115 Topic
</td>
<td>dcat:Dataset/dcat:theme
</td>
<td>Main theme(s) of the dataset if spatial
<p>[options: farming, biota, boundaries, climatology / meteorology / atmosphere, economy, elevation, environment, geoscientific information, health, imagery / base maps / earth cover, intelligence / military,
inland waters, location, oceans, planning / cadastre, society, transportation, utilities /
</p>
</td>
<td>Buildings and Structures
</td>
<td>ANZLIC:Open Spatial Data Taxonomy
</td>
<td><i>[options: farming, biota, boundaries, climatology / meteorology / atmosphere, economy, elevation, environment, geoscientific information, health, imagery / base maps / earth cover, intelligence / military,
inland waters, location, oceans, planning / cadastre, society, transportation, utilities / communication]</i>
</td>
<td><b>No</b>
</td>
<td>No
</td>
<td>Yes
</td></tr>
<tr>
<td>Field(s) of Research
</td>
<td>dcat:Dataset/dcat:theme
</td>
<td><a href="http://www.abs.gov.au/AUSSTATS/abs@.nsf/0/6BB427AB9696C225CA2574180004463E?opendocument">The Australian and New Zealand Standard Research Classification (ANZSRC), 2008 defined field or fields of research relevant to the dataset.</a>
</td>
<td>Atomic and Molecular Physics, Classical and Physical Optics
</td>
<td>Predefined text, but chosen as tags.
</td>
<td><i><a href="http://www.abs.gov.au/AUSSTATS/abs@.nsf/0/6BB427AB9696C225CA2574180004463E?opendocument">Available Here</a></i>
</td>
<td><b>No</b>
</td>
<td>No
</td>
<td>Yes
</td></tr>
<tr>
<td>Data Models
</td>
<td>See notes
</td>
<td>Free text - integrated with CKAN as well as possible.
</td>
<td>
</td>
<td>Free text option for data custodians to add information for any relevant data models, ontologies, taxonomies etc specific to their dataset.
</td>
<td><i>N/A</i>
</td>
<td><b>No</b>
</td>
<td>No
</td>
<td>No
</td></tr>
</tbody></table>