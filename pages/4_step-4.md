---
layout: default
title: Step 4 - Identify Protected Resources
permalink: step4/
---
<script src="https://use.fontawesome.com/e20c671b68.js"></script>
-----------------------------------------------------

Identifying your protected resources requires you to gather information from multiple resource inventories because the processes used to identify, track, and catalog resources are often distributed across multiple programs and systems within your agency. Each program or system collects and manages information about a subset of your agency’s resources.  For example, all agencies are required under FISMA to have a complete, current inventory of IT systems. ICAM implementers must be able to retrieve information about these resources quickly and efficiently to effectively manage access to them in a coordinated fashion. Additionally, physical and logical resources are typically managed separately from each other within an agency.

For many existing resources, your agency has already determined which resources require protection and the necessary level of protection. Guidance for determining protection requirements for information systems, devices, and infrastructure is outlined in existing policy and guidance documents (e.g., M-04-04, FIPS 199, M-06-16). Guidance for determining levels of protection for facilities and work sites which require electronic security systems is provided by the Interagency Security Committee (ISC). An agency’s physical security group will have previously evaluated all existing facilities and sites within the agency’s custody and determined physical protection requirements; however, for geographically dispersed organizations, this information may be managed locally. The figure below discusses several common programs and functions that collect and manage this information, and may therefore provide a starting point for ICAM implementers.

<br>

| <center> Agency Function </center> | <center> Information Available </center> | <center> Resource Type </center> |
|-------------------------------------------------------------------------------------|
| Facility Management Group / Physical Security Group | Information regarding resources that must be secured using Physical Access Control System (PACS). | <center> Physical </center> |
| Real Property Group | Information regarding land, building, and improvements that are owned or leased by a federal agency. | <center> Physical </center> |
| Capital Planning and Investment Control (CPIC) Program | Investment information for capital assets submitted by a federal agency to OMB for funding. | <center> Physical </center><center> Logical </center> |
| Helpdesk/Trouble Ticket Solutions and Records | Often contain lists of resources and/or targets of privilege/access management requests, as they are frequent sources of problems and issues for users. | <center> Physical </center><center> Logical </center> |
| Enterprise Data Warehouse | Enterprise Architecture (EA) repository of electronically stored data about an organization’s resources and data, commonly maintained to facilitate reporting and analysis. | <center> Physical </center><center> Logical </center> |
| Information Resources Catalog (IRC) | Some agencies may have an existing IRC, which is a comprehensive catalog of resources and resource information. | <center> Physical </center><center> Logical </center> |
| IT System Inventory | Inventory of IT applications and security compliance and reporting information. | <center> Logical </center> |
| Change Control Board (CCB) and/or Change Management System | Maintains the software, hardware, and application baselines for resources within the enterprise as a means of supporting change/upgrade efforts. | <center> Logical </center> |

<br>

### Checklist

> <i class="fa fa-check-square-o"></i> &nbsp;**Identify Content and Information.** Identify content and information within your systems used in the business functions of your agency. Protecting your content and information is important to achieve and maintain confidentiality, integrity, and availability of your resources.

> <i class="fa fa-check-square-o"></i> &nbsp;**Identify Applications and Web Services.** Identify applications and web services (e.g., employee timekeeping, reporting, and other agency-specific software hosted on local workstations, agency servers, and web-based services, such as a cloud environment) to protect against unauthorized users accessing your IT systems that host sensitive information, which could affect the availability and reliability of those systems.

> <i class="fa fa-check-square-o"></i> &nbsp;**Identify Networks and Infrastructure.** Identify any tangible interconnected technological assets (e.g., computer networks, servers, switches, hubs, mainframes, and the physical technology that support them) that make up or support the agency’s enterprise IT environment.

> <i class="fa fa-check-square-o"></i> &nbsp;**Identify Facilities.** Identify facilities occupied by your organization, including specific floors and corridors, to prevent physical attacks on your agency’s locations and your resources housed within.

> <i class="fa fa-check-square-o"></i> &nbsp;**Organize your agency’s resources.** Organize your agency’s resources by examining the resource attributes that determine how users are granted access and looking for similarities that drive access control decisions.   Resources may be grouped in several ways, including:

>> * **Geographical Location.** Grant access to all facilities within a specified area as a means of ensuring that personnel can easily attend meetings in nearby offices; this may also extend to network/system access associated with the area.

>> * **Project/Program Affiliation.** Projects or programs that rely on a subset of information systems or specified work locations can group those resources and grant access based upon affiliation with the project or program rather than granting each person access to each individual resource.

>> * **Organizational Relationship.** Within an agency there may be components or bureaus that grant access to resources based upon organizational affiliation (i.e., a component/bureau specific information sharing tool).

>> * **Function/Purpose.** Similar to Project/Program affiliation, certain resources may support a common function or purpose within an organization (i.e., HR systems, accounting systems, etc.).

> You must collect, analyze, and understand your agencies resources to determine the necessary level of protection to establish effective access control policies. Background information about a resource is often required to support access control decisions and can often be obtained by reviewing resource documentation and meeting with resource owners/administrators to discuss how and why access is currently controlled. Examples of contextual information that can be used to support access control are provided below.

<br>

| <center> Information Componenent </center> | <center> Description </center> |
|-----------------------------------------------------------------------------|
| **Time-based access restriction** | Access to the resource is restricted during particular hours or certain times of the day, week, or year based upon resource requirements |
| **Certification-based access restriction** | Access to the resource requires possession of a particular certification or permit |
| **Organizational affiliation restriction** | Resource access requires a particular affiliation with the organization (e.g., IT systems for federal employee access only), or affiliation with a particular bureau/component/office, etc. |
| **Location-based restriction** | Access to the resource is restricted based on geographical location for both physical and logical resources, and/or Internet Protocol (IP) and Media Access Control (MAC) address for IT resources and data |
| **Resource-based restriction** | Access to certain data or information is dependent upon it being accessed through a particular resource, thereby preventing direct access. |
| **Data sensitivity restriction** | Certain IT resources or data elements may require that users possess a level of public trust or clearance (National Agency Check with Written Inquiries [NACI], Public Trust, Secret, etc.) before being accessed. |

<br>

### Benefits

> <i class="fa fa-thumbs-o-up" aria-hidden="true"></i> &nbsp;**Each resource has its own role in your agency’s mission and is subject to potential vulnerabilities and threats.** Consider how to minimize vulnerabilities and mitigate threats while maximizing the effective use of the resource and making it available to the appropriate users. As you perform risk assessments of the resources, you’ll be able to identify resource vulnerabilities and the associated risks, and devise solutions to mitigate the risks. The results of this process will determine what other specific elements of the Access Management Framework you should apply during implementation. This assessment should consist of evaluating how alternative access control models might be applied to the resource, including centrally-controlled enterprise systems and the capabilities of the local resource.
