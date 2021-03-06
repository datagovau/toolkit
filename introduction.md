---
title: Introduction
layout: default
permalink: /introduction
---

<h1>Introduction to Data.gov.au</h1>
<h2>What is data.gov.au</h2>
<p><a href="https://data.gov.au">data.gov.au</a> is the national open data portal. The vision that all Federal Government data is discoverable in the one place, is machine readable, permissibly licensed and API enabled with some visualisation capability. We are on a journey to realise that vision across all government datasets but have made significant headway in recent times. 
</p>
<h2>How does it work</h2>
<p><a href="https://data.gov.au">data.gov.au</a> is run by the Department of Finance (Finance). It was relaunched 17 July 2013 using the CKAN (Comprehensive Knowledge Archive Network) platform on the Amazon cloud (Australian based) based on the model of data.gov.uk as an example of international best practice. CKAN is a basic but useful tool that provides a catalogue of data sources with good metadata, as well as API enabled hosting of tabular data. By default CKAN supports the hosting of any files but automatically generates API access for machine readable tabular datasets that are uploaded. CKAN itself is a tool for:
</p>
<ul><li><b>Publishing data files</b> – the platform best supports tabular and spatial data files, but any file type can be uploaded to data.gov.au.</li>
<li><b>Searching for data</b> – using the metadata and descriptive information stored on each dataset. Data.gov.au will also share metadata with other Australian data initiatives to make finding data easier across jurisdictions and disciplines.</li>
<li><b>Organising data files</b> – data is organised by government organisation, tags or government functions based on the Australian Governments’ Interactive Function Thesaurus (AGIFT)</li>
<li><b>Accessing data programmatically</b> – CKAN generates API access to uploaded CSV data files and some spatial files for ease of use by analysts and developers.</li>
<li><b>Linking to externally hosted data services (APIs)</b> – data custodians can add links to their external data services, such as ABS or Geoscience Australia data APIs.
<ul><li>Please note however, the new data.gov.au publishing policy is to no longer link to individual files hosted on government websites as these addresses often change and users/entities don’t get the advantage of consistent access to data.</li></ul></li>
<li><b>Basic data visualisation</b> – CKAN supports basic spreadsheet, graphing and mapping views of datasets that are uploaded in CSV or spatial formats. Finance are looking to support additional data visualisation tools down the track and can assist entities in finding appropriate tools in the meantime.</li></ul>
<p>You can read more on the CKAN platform at <a href="http://ckan.org">http://ckan.org</a> – it is an open source community and there are active CKAN usergroups around the world.
</p><p>Since the relaunch, the data.gov.au team have taken an agile and iterative improvements approach, expanding the system to meet the needs of data custodians and data users. Below is a live list of functional improvements the data.gov.au have made to date:
</p>
<ul><li>Software stack architectural design to improve system scalability.</li>
<li>The additional of a <a href="http://geoserver.org/">GeoServer</a>, integrated with CKAN to add spatial web services capability to the platform for hosting spatial datasets.</li>
<li>Integration of the <a href="http://www.finance.gov.au/taxonomy/term/1274/">data.gov.au blog</a> on the front page of data.gov.au.</li>
<li>Integration of Google Analytics with CKAN] for <a href="https://data.gov.au/site-usage">data.gov.au site/data reporting</a>.</li>
<li>Improvements to the metadata schema to meet Australian (AGLS) and international (DCAT, ANZLIC, ISO19115) data discovery best practices.</li>
<li>Improved services around automation for data extraction, transformation and publishing.</li>
<li>The ability to regularly harvest from CSW for ease of data discovery from existing data catalogs.</li></ul>
<p>All code developed for data.gov.au is available on our <a href="http://github.com/datagovau">data.gov.au GitHub</a>.
</p><p>You can see more technical information about the <a href="/platform-information">data.gov.au stack and change log</a>.
</p>
<h2>What datasets should entities publish</h2>
<p>Please see the <a href="/definitions#Types_of_data">'What is open data'</a> section on the wiki, which articulates different data types and how to deal with them.
</p><p>There are broadly three data types found in Government Entities:
</p>
<dl><dd><ul><li>Raw data generated out of business as usual activities – such as spatial data from a program, energy ratings data, crime statistics, administration data, etc. Often this data is stored in databases and primarily used in business applications.</li>
<li>Processed data – new data that results from a process such as tables from annual reports, FOI logs, other data created through the functions and running of entities. This could also be an aggregate view of a raw data set, fit for public access.</li>
<li>System data – data that is automatically generated from other processes such as web analytics, project management, access logs and other systems.</li></ul></dd></dl>
<p>All three types have different values and benefits in publishing.
</p><p>Identifying different data across your organisation means getting out of the traditional data teams and looks at other datasets that exist and how you can leverage them to improve services, policies and efficiencies. For instance, we recommend you analyse your FOI and Helpdesk logs for common requests, as you may be able to identify a number of datasets that you could actively publish. Thereby reducing time and resources spent on repetitively providing the same data to individual requests.
</p><p>It is also beneficial to look at data the entity already publishes, either in data form or PDF form. Where possible, publishing the data form of your data on data.gov.au will improve accessibility, reuse, discoverability and the ability for your Entity to better reuse the data. For instance, publishing the tables from your Annual Report, budget, grants, administrative data or Entity-specific mandatory reporting, is all useful. The 2012-2013 Productivity Commission report largely spoke about the value of administrative data at <a href="http://www.pc.gov.au/annual-reports/2012-13">http://www.pc.gov.au/annual-reports/2012-13</a>
</p><p>The entity may also want to assess what known datasets your entity has and identify a top 10 which would provide greater economic, transparency or policy benefits if made publicly available.
</p>
<h2>Mitigating Cost of FOI</h2>
<p>The FOI Act contains an Information Publication Scheme (IPS) that requires entities to publish certain categories of information online, including information routinely given through FOI requests. <a href="http://www.oaic.gov.au/freedom-of-information/applying-the-foi-act/foi-guidelines/part-13-information-publication-scheme/other-information-to-be-published-under-the-ips">Part 13 of the Information Commissioner’s FOI Guidelines</a> mentions that the IPS is designed to lessen the number of individual FOI requests to entity, including by releasing data frequently requested under FOI.
</p><p>The IPS also gives entities the discretion to publish other information. The FOI Guidelines recommend that entities should exercise that discretion to publish datasets they hold that could be made available for access and reuse, including on data.gov.au (see the <a href="http://www.oaic.gov.au/freedom-of-information/applying-the-foi-act/foi-guidelines/part-13-information-publication-scheme/managing-an-agency-ips-entry">‘Managing an IPS entry’</a> section, under the ‘Publication on a website’ heading). The Guidelines also contain a <a href="http://www.oaic.gov.au/freedom-of-information/applying-the-foi-act/foi-guidelines/part-13-information-publication-scheme/annexure-1-agency-plan-template">template IPS agency plan</a> that includes scope for publishing data on data.gov.au.
</p><p>Section 93A of the FOI Act requires entities to ‘have regard’ to the FOI Guidelines when performing functions or exercising powers under the FOI Act.
</p><p>Finance recommends entities analyse their FOI (and helpdesk) requests to identify specific datasets and other information that would create efficiencies through proactive publishing online.
</p>
