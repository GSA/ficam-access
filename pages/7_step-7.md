---
layout: default
title: Step 7 - Establish the Data Management Life Cycle
permalink: step7/
---
<script src="https://use.fontawesome.com/e20c671b68.js"></script>
-----------------------------------------------------
The Data Management Life Cycle focuses on identifying, obtaining, and maintaining required data elements that enable access control decisions. Maintaining current data is essential to effective access management. Using incorrect or out of date data can lead to successful access attempts by unauthorized users that put an agency’s resources in jeopardy. The Data Management Life Cycle defines the phases agencies can follow to maintain current data.

### Checklist

> <i class="fa fa-check-square-o"></i> &nbsp;**Identify requirements and obtain data required by your access control model.** This data includes attributes and their associated metadata about subjects, resources, and the contextual environment. Once you’ve have identified what data is required, you’ll need to determine where it’s located, how to obtain authorization to regularly retrieve it, and establish the authoritative source for required attributes. Required data could be within your resource’s systems (and therefore accessible) or it may be located elsewhere within your agency, or at an external source. Acquiring data that’s not currently available to a resource requires coordinating with the owner of that data and coming to an agreement on its use, definition, and how it will be obtained or transferred.

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>What is data and what types of data exist?</span></h3>
<p><span>NIST defines data as “a subset of information in an electronic format that allows it to be retrieved or transmitted.” The data components in the Framework serve to enable access control decisions by providing the information necessary to make those decisions. This information can include details about subjects, protected resources and other information that is considered when granting access to a resource.
There are three main types of data:</span></p>

<strong><span>Subject/Identity Data</span></strong><p><span>Information about a subject and the available details about their identity. A subject is an individual, process, or device causing information to flow among objects or changes to the system state. Subject/identity data is a product of the Data Management Life Cycle and is used to uniquely identify a subject, which allows an access control model to map the subject to their appropriate access permissions. The Policy Execution part of the Framework then uses this information to grant access accordingly. Subject/identity data includes attributes and their associated metadata about a specific subject.</span></p>

<strong><span>Protected Resource Data</span></strong><p><span>The details about a protected resource relevant to making an access control decision. Protected resource data is a product of the Data Management Life Cycle and is used to identify characteristics of a protected resource. This information can include elements such as the security clearance level required for access to a resource or specified emergency situations during which access can be restricted even further with increased requirements.</span></p>

<strong><span>Environmental/Contextual Data</span></strong><p><span>Data about situational elements that can affect access control decisions. Environmental/contextual data is the product of the Data Management Life Cycle and allows for more flexibility in access control decisions and policy. Environmental data can include information such as the time of day or current security threat level. This data provides the Policy Execution part of the Framework with more data elements to consider when making a decision. For instance, access to a resource may need to be limited to a smaller number of subjects if the security threat level is raised. If that information is available, it can be incorporated into the decision to automatically restrict access to only those authorized during a period when the security threat level is elevated.</span></p>

</div>

> <i class="fa fa-check-square-o"></i> &nbsp;**Define Enterprise Data and Attribute Format Standards.** Define standard data formats for identity and entitlement attributes to streamline provisioning and application integration processes. Agencies should leverage the guidance provided in the <a href="https://bnbuckler.github.io/ficam-identity/">Streamline Identity Management Playbook.</a>

> <i class="fa fa-check-square-o"></i> &nbsp;**Process and integrate data.** Once data is obtained, you must integrate and possibly format the data so that it can be used to make an access control decision. This processing can include entering data, verifying its authenticity, extracting data into a usable form, or simply importing it from the data source. Processing formats data so that it can be appropriately consumed during an access control decision.

> <i class="fa fa-check-square-o"></i> &nbsp;**Analyze data.** During this phase, you’ll analyze data to capitalize on any opportunities that may require further interpretation of data. This can involve tagging data to make it more useful to a wider array of resources, performing quality assurance practices, or even detecting patterns that can be used in the development of policies that advance access security.

> <i class="fa fa-check-square-o"></i> &nbsp;**Preserve data.** Data preservation involves the processes and procedures performed to store data for future reuse. During this phase, you’ll store timeframes and establish intervals. Preservation may include the archival of certain data elements for historical purposes. The preservation of data minimizes the amount of duplicative work performed because it eliminates the need to acquire data that’s already stored and/or archived. It also provides additional opportunities to share the stored data with business partners to exercise in their own access control processes, including the real-time retrieval of subject/identity data from authoritative sources.

> <i class="fa fa-check-square-o"></i> &nbsp;**Use data to make decisions.** Data is used during the Policy Execution part of the Framework to determine if the subject is authorized to access the protected resource. The access control model components in the Framework diagram reference the data necessary to render an access control decision in the Policy Execution part.
