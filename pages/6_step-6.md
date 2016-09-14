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
    active: "true"
  });
});
</script>

<script src="https://use.fontawesome.com/e20c671b68.js"></script>
-----------------------------------------------------------

To successfully manage access to resources, you must ensure that certain elements of information about the user and the resource are paired within the proper context to make an access decision. Your agency can use many access control models to determine how to handle user and resource attributes within access control transactions. Access control models are conceptual ways to express how an access control system implements specific policies using its underlying infrastructure components and security mechanisms. 

We’ve listed the five access control models below. When considering each option, it’s important for you to evaluate their access control needs, the capabilities of each resource being protected, and the overall risk to that resource. Your agency must implement some form of access control for each protected resource it owns. 

### Static Models

| <center> Model </center> | <center> Description </center> |
|-----------------------------------------------------------|
| **Access Control List (ACL)** |  Based on a list of permissions associated with an object. The list specifies who or what is allowed to access the object and what operations are allowed to be performed on the object. An ACL is a popular access control model used within the Federal Government. ACLs provide a simple way for resource owners to grant specific access permissions based on defined privileges associated with each user within a resource. The management of ACLs is typically performed by an agent of the protected resource owner and normally requires manual intervention. When a new user requires access to the protected resource, a request is submitted to the resource owner. If the user is authorized, the resource owner, or its agent, provisions the user’s account with the appropriate permissions (e.g., edit a file or unlock a door). User permissions are typically tracked via a decentralized system often developed by the resource owner, such as a spreadsheet, database, or even a list of users in a notebook associated with their access rights. |
| **Role-based Access Control (RBAC)** |Used for controlling access to resources where permitted actions on resources are identified with roles rather than with individual subject identities. Using roles can simplify the administration of user permissions; they can be functional, organizational, or even customized to suit the needs of a particular agency. Each role is associated with a specific set of permissions to a set of protected resources and each user is assigned to and provisioned into one or more roles. In an RBAC system, when a new user needs to be provisioned access to a resource, their account is added to the role for which they’ll be granted access. For example, when a new manager joins an organization, their account is added to the Manager role within the RBAC system, providing access to all resources granted to managers within the organization. In comparison, an ACL system would require the user’s account and their permission to be manually added separately. |

<br>

### Dynamic Models

| <center> Model </center> | <center> Description </center> |
|-----------------------------------------------------------|
| **Attribute-based Access Control (ABAC)** | Introduces specific characteristics or “attributes” (e.g., demographic data, employment affiliation, and citizen status) associated with and about subjects, objects, targets, initiators, resources, or the environment. An access control rule set defines the combination of attributes under which an access may take place. The ability to retrieve attributes associated with a user provides resource owners with the flexibility of facilitating access to external users as long as attributes associated with the user are available and meet the defined requirements for access. Policies define attribute requirements for given resources. ABAC grants or denies access based on attributes that are submitted or retrieved in response to an access request. Examples of attributes are demographic data, employment affiliation, citizenship status, data attributes (tags), environmental attributes, etc. These attributes can be submitted directly by a subject or collected from various internal and external attribute sources (such as an employer’s database). The values associated with the attributes submitted are then compared with the attribute values required by the access control policy. If the values submitted or retrieved meet the requirements of the access control policy, access is granted. |
| **Policy-based Access Control (PBAC)** | Uses authorization policy that is flexible in the types of evaluated parameters (e.g., identity, role, clearance, operational need, risk, heuristics). It expands on the variety of attributes employed in the access control decision process and addresses the need for organizations to adhere to abstract policy requirements and regulations (e.g., Sarbanes-Oxley Act [SOX] and Gramm-Leach-Bliley Act), when implementing access control measures. PBAC uses enterprise-wide attributes from the protected resource, the environment, the action performed, and the requester to make an access control decision based on the applicable access control policies, the attributes provided, and the given access request circumstances. Once an access attempt is made, the access control decision is determined by assessing each of the submitted attributes, the given circumstances, and the appropriate policy that applies to those circumstances. The required enablers for policy execution are retrieved and an access control decision is made based on whether the data match the requirements defined in the policy. |
| **Risk-Adaptable Access Control (RAdAC)** | Uses an authorization policy that takes into account operational need, risk, and heuristics. The RAdAC model further expands on the variety of attributes considered during an access control decision and enhances security by introducing a threat level element into the access control equation. Organizations can calculate a quantifiable risk metric based on factors such as a user’s trustworthiness, information about the corporate IT infrastructure, and other environmental risk factors. This calculated risk metric can then be used to dictate what types and amount of user-related information is required during an access attempt. This information may vary so that the level of security is commensurate with the threat level. When accessing a resource protected by RAdAC, a user’s access attempt will require certain information elements that are determined by the risk metric. Once information is transmitted, it’s assessed against the access control policies related to the current threat level. These policies could include a wide variety of factors such as determining the operational needs of a user based on the current threat level. Additionally, the requirements for access control decisions should be made based on a diverse set of situations and risk levels. RAdAC also allows for a certain level of machine learning (heuristics) that involves considering past access control decisions as a factor when making future access control decisions. This heuristic information can then be used to improve access control policies by targeting risk and operational need determinations. Considering the vast amount of data being referenced and the technology involved during the Policy Execution part, RAdAC is the most complex access control model for agencies to implement. |

<br>

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>Access Control List (ACL)</span></h3>
<p><span>Access to resources is granted on a resource-by-resource basis, based upon an individual’s inclusion and corresponding privileges, as noted on the resource’s ACL.</span></p>

<strong><span>Benefits</span></strong>
<p><span>• Simple framework which does not require pre-existing infrastructure.<br>• Supported by common operating systems.<br>• Widely used and accepted throughout the Federal Government.<br>• Controlled locally at the resource level.</span></p>

<strong><span>Limitations</span></strong>
<p><span>• Ability to evaluate individual access privileges becomes extremely complex as the list grows larger over time.<br>• Criteria for access and individual role/job duties are fluid over time, thereby placing a significant administrator burden on resources owners.<br>• Nearly impossible to manage at an enterprise level due to the sheer volume of resources and ACLs.<br>• Requires manual changes to ACL, a time consuming and error prone process.<br>• Revocation of access privileges may be delayed due to non-automated communication methods (e.g., word of mouth, e-mail, paper form distribution, etc.).</span></p>

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
<p><span>Focuses on characteristics that describe people, resources and environments. The requester provides attributes which are compared to those documented as requirements for granting or denying access, at which point a decision is made.</span></p>

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
<p><span>Amount of information required of requesters to verify their identity depends on the current threat level, information includes personal trustworthiness and environmental factors.</span></p>

<strong><span>Benefits</span></strong>
<p><span>• Has the ability to make real time access control available.<br>• Can control multiple diverse systems- including digital policies as some systems may require different authentication levels for the same user based transactions.<br>• Supports flexible situations. </span></p>

<strong><span>Limitations</span></strong>
<p><span>• Cannot always be automatic, user judgments are needed.<br>• Integrated systems must use standardized data exchange formats.<br>• Policies must be unambiguous to avoid unintentional, unauthorized access.<br>• Extensive considerations in adhering to policy and law – involves great care to be taken to ensure compliance.<br>• Not natively supported by common operating systems.</span></p>

<strong><span>Key Takeaways</span></strong>
<p><span>Agencies that likely will benefit from implementing a RAdAC system are those that:<br><br>• Need the flexibility to adapt their access control based on environmental conditions, such as risk and/or the need for situational awareness;<br>• Have well defined internal policies and/or may be required to comply with additional federal and regulatory policies; and<br>• Have tightly controlled enterprise environments consisting of well integrated systems that operate using standardized data exchange formats. </span></p>

</div>
