---
layout: default
title: Step 9 - Implement the Policy Administration Life Cycle
permalink: step9/
---
<script src="https://use.fontawesome.com/e20c671b68.js"></script>
-----------------------------------------------------

You should create well-defined, meaningful policies that address the security needs of your agency for effective access control. The Policy Administration Life Cycle produces policies that meet the requirements of the resource and access control model which are converted into digital policies in the Enablers part of the Framework. When using the more advanced access control models, these policies can support an agency’s efforts for establishing a centralized, enterprise-wide access control solution.

### Checklist

> <i class="fa fa-check-square-o"></i> &nbsp;**Define the access control policy scope and requirements for a target asset or resource.** The following considerations and inputs influence the access control policy definition process, including but not limited to: environment, users, unauthorized access risks, and existing policies, rules or internal processes that currently govern access to the resource or asset. The purpose of the Policy Definition process is to hone the general access control requirements of the protected resource into specific, well-defined requirements while taking other factors into account, such as federal standards and agency policies.

> <i class="fa fa-check-square-o"></i> &nbsp;**Analyze policy definitions.** During this process, you’ll examine and analyze the policy definition outputs and findings that will help refine or create new access control policies. The analysis of the risks, rules, and inputs discovered is used to determine the authentication token type, the access control model, the relevant authorization model, and the tools used to enforce access. As previously mentioned, the access control model has an effect on every aspect of the Framework and should be selected appropriately.

> <i class="fa fa-check-square-o"></i> &nbsp;**Create access control policies using access control mechanisms and technology platforms.** During this creation phase, you’ll focus on building access control policies based on the rules, requirements, and designs developed in previous phases. You’ll also need to test use cases to evaluate the efficacy of the policy created are developed during this phase.

<div style="background-color: #edf1f3;color: black;margin: 10px;padding: 10px">

<h3><span>How are digital policies created?</span></h3>
<p><span>Each access control model has different requirements for the Digital Policy. As a result, the type of access control model being used ultimately determines the format of the digital policy. The differences between the access control models and how digital policies are created are outlined below:</span></p>

<strong><span>ACL</span></strong><p><span>The creation of a digital policy for an ACL involves building the ACL based on the Access Permissions that define which subjects are approved for access to a resource and at what access levels. This is usually done by referencing a list of users that have been approved to access the resource, adding their account to the ACL within the resource, and associating the proper permissions with their account. The ACL is referenced when a subject makes an access attempt and access is granted accordingly.</span></p>

<strong><span>RBAC</span></strong><p><span>An RBAC Digital Policy requires the creation of well-defined roles that can be used to distinguish different sets of subjects based on their relationship to the agency or resource. These pre-defined roles carry a specific set of privileges associated with them. Once roles are defined, subjects can be assigned as many roles as needed based on their Access Permissions in order gain access to resources required to perform their work. Depending on the implementation, these roles can be stored in centralized systems for an enterprise solution or can be managed locally for a smaller set of resources. These roles and rights are used to make access control decisions.</span></p>

<strong><span>ABAC, PBAC, and RAdAC</span></strong><p><span>These models may involve a significant number of external systems that host attribute data. Once the elements required to access a resource are defined, the Digital Policy is created based on those requirements. The Access Permissions from the Privilege Management Life Cycle are associated with the various requirements for accessing a specific resource defined in the Digital Policy. This policy is implemented via a centrally managed authorization engine. During the Policy Execution part of the Framework, this engine compares the data received during an access attempt, the data required by the resource, and the Access Permission information within the policy. A successful grant access decision is made if all requirements are met and the appropriate permissions are applied.</span></p>

</div>

> <i class="fa fa-check-square-o"></i> &nbsp;**Evaluate the policy or policies.** During this phase you’ll evaluate the policies designed and developed on test assets or resources. The use cases developed during the creation phase are used to independently test how well the requirements are being met. The results of these tests can then be used to improve the policy to validate that defined metrics and goals are being met.

> <i class="fa fa-check-square-o"></i> &nbsp;**Implement and enforce new policies.** During this process, you’ll carry out the new or revised policy on a production physical or logical asset or resource.  Once implemented, the policy can be tested to verify compliance with requirements.

> <i class="fa fa-check-square-o"></i> &nbsp;**Review and revise policies.** During this process, you’ll measure the effectiveness of the policy implemented and determine if the access control policy should be revised or retired. This phase includes the periodic review and testing of an access control policy to confirm that it continues to satisfy requirements and meet metrics goals. This process may also help identify policies that are either no longer necessary or that should be revised, allowing an agency to take appropriate action.
