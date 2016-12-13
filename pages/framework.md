---
layout: default
title: Access Management Framework
permalink: framework/
---
<script src="https://use.fontawesome.com/e20c671b68.js"></script>
-----------------------------------------------------
The Access Management Framework was developed to provide you with the guidance to implement access control in your enterprise environment. It shows the many areas and components used to establish access management policies.

The picture below is a view of the Access Management Framework and its key components.

<div style="text-align:center"><img src="{{site.baseurl}}/img/framework.png"/></div>

<br>

You should consider each part of this Framework while implementing access control measures. The diagram shows how each component is related and builds upon each other to protect and ensure the appropriate sharing of resources. It describes the design-time elements that are addressed during the planning stages and the run-time actions that occur in real-time during an attempt to access a resource. Policy Execution is the run-time process that results in a determination as to whether access to a protected resource is granted or denied based on the enablers that have been developed in the design-time phase. Policy execution is the culmination of each component of the Framework coming together to achieve the targeted level of protection for a resource.

Policy execution is initiated when a user attempts to access a protected resource. The various tools and technologies then retrieve elements that are required by the access control model and evaluate the data inputs and the requirements of the policy to render an access control decision that is compliant with the appropriate policy. Each access control model involves different enablers in the decision making process as outlined in the figure below. The access models below will be discussed in more detail in Step 6.

| <center> Access Control Model </center> | <center> Enablers Retrieved/Referenced </center> | <center> Access Granted If: </center>|
|:----------------------------------------|----------------|---------------------|
| **ACL** | • The ACL associated with the resource | The subject attempting to access the resource is listed in the ACL with appropriate access permissions associated with their account. |
| **RBAC** |• Role-based access permissions<br><br>•The associated digital policy that associates roles with defined permissions | The subject attempting to access the resource is associated with a role that is assigned specific permissions to the resource. |
| **ABAC** | • The required attributes defined by the policy associated with the resource<br><br>• Environmental/Contextual Data<br><br>• The digital policy that defines the required attribute values for accessing the resource | The values of the retrieved attributes match the attribute values required to access the resource. |
| **PBAC** | • The required attributes defined by the policy associated with the resource<br><br>• Environmental/Contextual Data<br><br>• The digital policy that is based governmental, agency, or organizational regulations and policies | The values of the retrieved attributes match the attribute values required by the digital policy to access the resource. |
| **RAdAC** | •	The required attributes defined by the policy associated with the resource<br><br>•	Environmental/Contextual Data<br><br>• Past access decision information<br><br>• The appropriate digital policy identified for use based on the consideration of environmental factors | All requirements of the dynamic digital policy are met given the information provided by the Enablers part of the Framework. |
