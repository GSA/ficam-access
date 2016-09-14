---
layout: page_collection
title: Step 6 - Choose Your Access Control Model
permalink: 6_step-6
---
<script>
$(function() {
  $( "#accordion" ).accordion({
    heightStyle: "content",
    collapsible: "true",
    active: "false"
  });
});
</script>

<script src="https://use.fontawesome.com/e20c671b68.js"></script>
-----------------------------------------------------------

You can use many access control models to determine how to handle user and resource attributes within access control transactions. Access control models are conceptual ways to express how an access control system implements specific policies using its underlying infrastructure components and security mechanisms. 

We’ve listed the five access control models below. When considering access control models, it’s important to evaluate the capabilities of each resource being protected, their access control needs, and the overall risk to that resource. Your agency must implement some form of access control for each protected resource it owns. Below you will find five access control models including a brief description. 

### Static Models

| <center> Model </center> | <center> Description </center> |
|-----------------------------------------------------------|
| **Access Control List (ACL)** |  This model is based on a list of permissions that specify who or what is allowed to access the object and what operations may be performed on the object. ACLs allow resource owners to grant specific access permissions based on defined privileges associated with each user within a resource. When a new user requires access to the protected resource, a request is submitted to the resource owner. If the user is authorized, the resource owner, or its agent, provisions the user’s account with the appropriate permissions (e.g., edit a file or unlock a door).  This is typically a manual process. |
| **Role-based Access Control (RBAC)** |This model is used to control access to resources where a permitted action on a resource is allowable based on the individual’s assigned role rather than their identity. In this model, when a new user needs to be provisioned access to a resource, their account is added to the role for which they’ll be granted access. For example, when a new manager joins an organization, their account is added to the Manager role within the RBAC system, providing access to all resources granted to managers within the organization. In comparison, an ACL system would require the user’s account and their permission to be manually added separately to each resource. |

<br>

### Dynamic Models

| <center> Model </center> | <center> Description </center> |
|-----------------------------------------------------------|
| **Attribute-based Access Control (ABAC)** | ABAC grants or denies access based on attributes (e.g., demographic data, employment affiliation, citizenship status, data [tags], environmental) that are submitted or retrieved in response to an access request.  The ability to retrieve attributes associated with a user provides resource owners with the flexibility of facilitating access to external users as long as attributes associated with the user are available and meet the defined requirements for access.  These attributes can be submitted directly by a subject or collected from various internal and external attribute sources (such as an employer’s database). The values associated with the attributes submitted are then compared with the attribute values required by the access control policy. If the values meet the requirements of the access control policy, access is granted. |
| **Policy-based Access Control (PBAC)** | PBAC can be said to be a standardization of the ABAC model at an enterprise level in support of specific governance objectives. In an ABAC-only model, the attributes required to gain access to a particular resource are determined on a local level and can vary greatly from one organizational unit to the next.  PBAC combines attributes from the resource, the environment, and the requester with information on the particular set of circumstances under which the access request is made, and uses rule sets that specify whether the access is allowed under organizational policy for those attributes under those circumstances.  It expands on the variety of attributes employed in the access control decision process and addresses the need for organizations to adhere to abstract policy requirements and regulations (e.g., Sarbanes-Oxley Act [SOX] and Gramm-Leach-Bliley Act), when implementing access control measures. |
| **Risk-Adaptable Access Control (RAdAC)** | RAdAC extends upon other earlier access control models by introducing environmental conditions and risk levels into the access control decision process, in addition to the concept of “operational need.” RAdAC goes beyond the traditional reliance on static attributes and polices to combine information about a person (or machine’s) trustworthiness, information about the corporate IT infrastructure, and environmental risk factors to create an overall quantifiable risk metric. Under RAdAC, policies would be able to specify the set of circumstances under which ordinarily weak access control could be strengthened during a heightened security risk or relaxed to allow access based upon a determination of operational need to access a resource.RAdAC is the most complex access control model for agencies to implement. |

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Access Control List (ACL)</span></h3>
<p><span>Access to resources is granted on a resource-by-resource basis, based upon an individual’s inclusion and corresponding privileges, as noted on the resource’s ACL.</span></p>

<strong><span>Benefits</span></strong>
<p><span>• Simple framework which doesn't require pre-existing infrastructure.<br>• Supported by common operating systems.<br>• Widely used and accepted throughout the Federal Government.<br>• Controlled locally at the resource level.</span></p>

<strong><span>Limitations</span></strong>
<p><span>• Managing individual access privileges can become extremely complex over time due to volume and fluidity of roles/job duties.<br>• Difficult to manage at an enterprise level due to the sheer volume of resources and ACLs.<br>• Prone to manual changes and entry errors.<br>• Granting and revoking of access may be delayed due to non-automated communication methods (e.g., word of mouth, e-mail, paper form distribution, etc.).</span></p>

<strong><span>Key Takeaways</span></strong>
<p><span>ACLs are useful and often sufficient when granting access to resources to a relatively small number of internal users that can be easily managed and monitored by a resource owner.</span></p>

</div>

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Role-Based Access Control (RBAC)</span></h3>
<p><span>Individuals are assigned to various roles within an organization, down to the resource level based upon certain identity and entitlement attributes. Access is determined by having a particular role assignment that corresponds to one or more resources.</span></p>

<strong><span>Benefits</span></strong>
<p><span>• Supports groupings of individuals with particular roles based upon well-defined and trusted attributes.<br>• Can accommodate centralized management.<br>• Can be implemented at various levels within an organization, as long as a valid role is defined.<br>• Supported by common operating systems and capable of group support as well.</span></p>

<strong><span>Limitations</span></strong>
<p><span>• Can be difficult to manage as each protected resource generally has unique role requirements, thereby resulting in large numbers of potential role assignments within an organization.<br>• Difficult to manage granular access of individuals due to the rigid nature of role assignments.<br>• Difficult to implement in a highly distributed agency (not centrally managed).<br>• Requires significant level of effort to determine appropriate alignment of privileges for users not linked to the agency’s organizational structure.</span></p>

<strong><span>Key Takeaways</span></strong>
<p><span> RBAC can be useful in agencies that have established and well-defined roles for their users. Additionally, this model is effective when external users either do not require access to protected resources or when the host agency can easily control the roles assigned to external users.</span></p>

</div>

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Attribute-Based Access Control (ABAC)</span></h3>
<p><span>ABAC focuses on characteristics that describe people, resources and environments. The requester provides attributes which are compared to those documented as requirements for granting or denying access, at which point a decision is made.</span></p>

<strong><span>Benefits</span></strong>
<p><span>• Requires no advance knowledge of requestors.<br>• An individual’s attributes can be correlated from multiple sources to create a unified identity.<br>• Highly adaptable to changing needs; efficient for agencies where individuals come and go frequently.</span></p>

<strong><span>Limitations</span></strong>
<p><span>• Lengthy implementation time due to the need to correlate information and attributes from multiple sources for all potential users.<br>• Reliant on authoritative identity/entitlement data – difficulty managing attribute conflicts between source systems.<br>• Not natively supported by common operating systems.<br>• Not appropriate for all environments (i.e., those with significant changes in risk level).</span></p>

<strong><span>Key Takeaways</span></strong>
<p><span> ABAC requires the ability to request and retrieve a variety of attributes and attribute sources for it to be an effective model in making access control decisions. <br><br>Since ABAC is not natively supported by most systems, the availability of tools and technologies is extremely important. </span></p>

</div>

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Policy-Based Access Control (PBAC))</span></h3>
<p><span>Access to resources is granted on a resource-by-resource basis, based upon an individual’s inclusion and corresponding privileges, as noted on the resource’s ACL.</span></p>

<strong><span>Benefits</span></strong>
<p><span>• Promotes compliance with standardized access controls.<br>• Flexible in not being linked to only one type of access control.<br>• Adapts quickly to new policy rules.</span></p> 

<strong><span>Limitations</span></strong>
<p><span>• PBAC requires the design, deployment, and seamless integration of enterprise level systems (databases, directory services, etc.).<br>• Policies must be absolutely unambiguous to avoid unintentional, unauthorized access.<br>• Entire enterprise must use the same attributes for access and those attributes must be authoritative.• Not natively supported by common operating systems.</span></p>

<strong><span>Key Takeaways</span></strong>
<p><span>PBAC can benefit agencies that have resources which require varying levels of security and the budget to invest in the development of the standard elements required by the solution. </span></p>

</div>

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Risk-Adaptable Access Control (RAdAC)</span></h3>
<p><span>Amount of information (peronsonal trustworthiness and enviornmental factors) required of requesters to verify their identity depends on the current threat level.</span></p>

<strong><span>Benefits</span></strong>
<p><span>• Has the ability to make real time access control available.<br>• Can control multiple diverse systems- including digital policies as some systems may require different authentication levels for the same user based transactions.<br>• Supports flexible situations. </span></p>

<strong><span>Limitations</span></strong>
<p><span>• Cannot always be automatic, user judgments are needed.<br>• Integrated systems must use standardized data exchange formats.<br>• Policies must be unambiguous to avoid unintentional, unauthorized access.<br>• Extensive considerations in adhering to policy and law; great care must be taken to ensure compliance.<br>• Not natively supported by common operating systems.</span></p>

<strong><span>Key Takeaways</span></strong>
<p><span>Agencies that may benefit from implementing a RAdAC system are those that:<br><br>• Need the flexibility to adapt their access control based on environmental conditions, such as risk and/or the need for situational awareness;<br>• Have well defined internal policies and/or may be required to comply with additional federal and regulatory policies; and<br>• Have tightly controlled enterprise environments consisting of well integrated systems that operate using standardized data exchange formats. </span></p>

</div>
