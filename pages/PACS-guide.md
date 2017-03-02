---
layout: default
title: What Is a PACS
permalink: /PACS-guide/
---

# What is a Physical Access Control System (PACS)

## Introduction
This guide is intended to provide a general overview of Federal Information the Processing Standards (FIPS) 201 Personal Identity Verification (PIV) compliant PACS that are used within the federal government.  It will provide information on the components that make up a PACS solution, how PACS components work together to provide physical access control for federal agencies and where these approved PACS products can be found.  In addition, this guide will discuss the benefits of PIV compliant PACS and the General Services Administration (GSA) FIPS 201 Evaluation Program’s PACS testing and why it’s needed.

## Overview
A PACS is an electronic system that controls the ability of people or vehicles to enter a protected area, by providing authentication and authorization mechanisms at access control points.  More specifically, PACS are electronic devices used in physical access control.

Physical access control is a security method used to help prevent unauthorized access to a building, room or protected area.  It helps to ensure that only individuals who are authorized have unescorted access to these protected areas. There are many ways to provide physical access control - from the utilization of a wall or fence, to the use of a traditional lock and key solution, as seen in cars and homes today.

The most recognizable physical access control method and the one synonymous with security is the use of human security guards to protect important assets.

As technology advanced and matured, electronic PACS have become a critical component in the federal government’s quest to provide better physical access control.  PACS are a reliable way to provide an additional layer of security to enhance traditional physical access control methods (e.g., security guards, fences etc.), and in some instances, replace traditional methods entirely. PACS can be used to protect the outer perimeter such as entry and exit points to a building or they can be used for interior access control to a room.  

PACS can be a proximity reader that reads the information off of a proximity card to electronically unlock a door (replacing the traditional lock and Key solution with an electronic version) or PACS can be a very complex system, comprised of many components used to make physical access control decisions such as the PACS used in federal facilities.  

PACS used for secure federal buildings utilize Public Key Infrastructure (PKI) technology to help with access control decisions.  PKI use public and private keys to facilitate the secure exchange of electronic information via the network.  PKI is a process that binds public keys and identifying information (contained on certificates) to a person.  The binding is established through a process of registration and the issuance of certificates by a trusted source (i.e., Certificate Authority (CA)).  

In PKI, a public key certificate (also known as a digital certificate or identity certificate) is an electronic document used to prove the ownership of a public key.  The certificate includes information about the key, information about its owner's identity, and the digital signature of the trusted source (i.e., CA) that has verified that the certificate's contents are correct.  

If the CA’s digital signature is valid, and the person examining the certificate trusts the signer, then they know they can use that key to communicate with its owner. Smartcards contain public and private keys, and certificates that can be read by federal PACS to help validate the identity of a person entering a federal facility.

Online Certificate Status Protocol (OCSP) Responders are used to determine if a PKI certificate has been revoked or have expired.  
PACS systems access this information to help make access control decisions. If a smartcard holder certificates have been revoked or have expired the smartcard holder will be denied access into the facility. An OCSP Responder is part of the federal government’s existing PKI and is not a component that will need to be purchased with a PACS. 

PACS used to make access control decisions within the federal government may consist of many components to include:

* Smartcard Reader (used to read information about a person stored on the smartcard) 

* PACS Infrastructure Controller (used to control the opening of gates and doors) 

* Secure Controller (located in a secure area and communicates with the PIV Card, Head End System, and PACS Infrastructure Controller to make access control decisions)

*	Database Server (contains the names of smartcard holders and their facility access rights) 

*	Caching Status Proxy Server (used to cache smartcard holders data to optimize the performance of PACS)

*	Head End System/Access Control Server (Used to register PIV Cardholders into the PACS and to refresh the controller with the latest information)


{% include alert-info.html content="To further improve the PACS used in federal buildings and facilities, the federal government has mandated that PACS meet the National Institute of Standards and Technology (NIST) Federal Information Processing Standards (FIPS) 201 standard for Personal Identity Verification (PIV)." %}

## Why Implement the NIST PIV Standard?

The NIST FIPS 201 PIV standard contains the minimum requirements for a Federal PIV system that meets the control and security objectives of Homeland Security Presidential Directive -2 (HSPD-12).  The NIST FIPS 201 PIV standard also provides detailed specifications that will support technical interoperability among PIV systems of Federal departments and agencies.  PIV Cards that meet the NIST FIPS 201 PIV standard will be interoperable with all PIV PACS within the Federal Government.  In order to achieve interoperability within the Federal Government, all Federal agencies must configure their PACS to meet the PIV standard to support the PIV Card.

## What is HSPD-12 and what was its intended goal?

HSPD-12 is a strategic initiative intended to enhance security, increase Government efficiency, reduce identity fraud, and protect personal privacy. HSPD-12 was signed by President George Bush in 2004 due to security concerns over the wide variations in the quality and the security of the identification used within the Federal Government to gain access to secure Federal facilities.  The goal of HSPD-12 was to eliminate these variations by establishing a mandatory, Government-wide standard for secure and reliable forms of identification issued by the Federal Government to its employees and contractors.  The HSPD-12 standard that will be utilized by all Federal departments and agencies includes the vetting of individuals and the issuance of identification (e.g., Smartcards) to enhance security, reduce identity fraud, and to protect personal privacy.

## What are somre NIST PIV requirements for PACS?

* PACS must be designed and configured to read and process the appropriate electronic identification information associated with an individual that is stored on a PIV Card.

*	PACS are required to be tested to ensure they meet the minimum security and interoperability requirements outlined in the NIST FIPS 201 PIV standard.

![Example PIV card](../img/PIV_card.png)

*	The PIV Card is the individual cardholders identity credential for accessing government buildings, facilities and computer networks.

* PIV PACS are required to access and validate the appropriate PIV certificate to meet the facilities security assurance level requirements.

* The assurance level required for each federal facility will determine which certificate stored on the PIV card will be needed for physical access into that facility.  A federal facillity may require:

  *Single Factor Authentication - Something you have (PIV Card) + visual check
  *Two Factor Authentication - something you have  (PIV Card) + something you know (PIN)
  *Three Factor Authentication - something you have (PIV Card) + something you know (PIN) + something you are (Biometric)

Note: Possession of a valid PIV Card as evidence by visual inspection of the card, reading a signed identity cert from the card, or performing challenge/response authentication with the card, provides one-factor authentication.  See examples below:  

*	PACS can perform a private key challenge/response using the Card Authentication Key (CAK) to validate the PIV Card is authentic or
*	PACS can perform a signature check of the Cardholder Unique Identifier (CHUID) to ensure it was signed by a trusted source and is unaltered and check the expiration date to ensure it’s still valid.

NIST FIPS 201 provided the opportunity to migrate building access systems from LITTLE OR NO confidence assurance levels to VERY HIGH confidence assurance levels.


## What are the benefits of PIV compliant PACS?

* PIV compliant PACS allow Federal employees and contractors to utilize the same PIV card for physical access into all Federal facilities for which they are authorized.

* Creates standardization and promotes interoperability within the Federal Government by Integrating several disparate PACSs into an enterprise system

* Provides a system that promotes trust and create efficiency by rapidly authenticating credentials electronically for entering and exiting Federal facilities

* Strengthens physical security within the Federal Government

* Capable of being implemented for federal facilities requiring high assurance personal identity verification

* Provides a stronger identification process than non-compliant PACS

* Maintain a system less susceptible to identity fraud, tampering, counterfeiting and terrorist exploitation

* Enables the PIV card to be centrally managed by the issuer, so that card loss or terminatioin results in disabling the card in any PACS database in which the card exists

## PACS Component Categories

PACS are classified in two “GSA Approved topologies” which consist of the latest and most utilized configurations within the federal government.  These topologies are listed as 13.01 and 13.02.  This document will focus on topology 13.01 and its components which are listed under categories.  These categories of PACS are defined as part of a whole PACS solution that can be tested end-to-end by the GSA's FIPS 201 Evaluation Program.

**Topology 13.01 consist of 3 main categories:**

*	PACS PIV Reader
*	PACS Validation System
*	PACS Infrastructure

## PACS Components (what they are and how they work)

### **PACS PIV Reader Category**
A PIV Reader (i.e., smartcard reader) is a device that provides the human interface, the PIV Card interface, and the communications to and from the PACS Validation System. PACS PIV Readers have 3 types:

*	Single Factor PIV Readers – Do not allow Two Factor authentication (No PIN Pad)
*	Two Factor PIV Readers – Has a Pin Pad but no Biometric Reader
* Three Factor PIV Readers – Has Pin Pad and Biometric Reader

Example of a PIV Reader in operation: Federal employees and contractors will present their PIV Card to the PIV reader to obtain entry into a controlled federal facility.  The PIV Reader reads the identifying information stored on the PIV Card that is associated with the individual PIV Card-holder.  It then communicates that information to the PACS Validation System.  The Validation System will validate the credentials of the individual stored on the PIV Card.  The information obtained from the PIV Card will determine if the individual will be granted physical access to the facility.   A PIV reader may be a wholly-integrated unit, or it may be an assembly of components including:

* Contact Reader (Core Component)

Communicates with the PIV smartcard using electrical signals via wires when touching (i.e., contacting) the PIV smartcard’s contact pad. 

* Contactless Reader

Communicates with the PIV smartcard wirelessly using Radio Frequency (RF) technology. 

* PIN Pad

Used in conjunction with the PIV Reader to provide two-factor authentication.  Personnel will present their PIV Card to the PIV Reader, and based on the level of security required for the facility, the system may require the PIV-card holder to enter their Personal Identification number (PIN).  This provides two-factor authentication to enter the facility (something you have (PIV Card) and something you know (PIN)).

* LCD Display

Provide PACS visual notifications to PIV Card-holders.  Visual notifications can include error messages; proceed or stop messages or some other type of notification to alert or direct an individual.

* LED lights

Similar to LCD displays in that they are used to provide a visual message to the PIV Card-holder.  LED lights can be used to display a green arrow to inform an individual to proceed through a gate/turnstile once a PIV Card-holder credentials have been validated and the individual is authorized and granted access to the facility.

*	Audio announcers

Used in PACS to provide audible alerts.

*	Fingerprint sensor

The fingerprint sensor can be used to access the on-card biometric data stored on the PIV Card to provide physical access to a federal facility.  A scan of the PIV Card-holders fingerprint is taken using the PACS fingerprint sensor and compared to the on-card biometric data stored on the card.

*	Other biometric modalities 

Other biometric methods (e.g., iris scan) can be utilized to access biometric data stored on the PIV Card to provide physical access to a federal facility.

*	Communications to a Validation System

The PIV Reader products communicates via wires, cables or by using wireless transmission (e.g., Wiegand, RS-485, secure wireless, Ethernet) to the Validation System and other PACS devices.

### **PACS Validation System**
The PACS Validation System provides the necessary functions to perform identification and authentication of the PIV Card-holder.   A Validation System is made up of several compatible and interoperable components that may include: 

*	Server-based Certificate Validation Protocol (SCVP) Server

Used to determine whether the PIV Card-holder’s digital identification (i.e., certificate) that is stored on a PIV Card can be linked back to a trusted issuer.

*	Online Certificate Status Protocol (OCSP) Responders

Used to check the status of a certificate stored on a PIV Card to ensure that the certificate is valid and has not expired.  An expired certificate is like an expired driver’s license; it cannot be used as a valid credential for physical access to a controlled federal facility.  The PIV-card holder will be denied access by the PACS.

*	Caching status proxy server

Used to cache PIV-Card holders data to optimize the performance of PACS.  It allows applications that continuously poll the controller for data to supply that data more rapidly, which is required to operate the PACS more efficiently when handling a lot of user traffic.

*	Secure Controllers

Devices located within a secure area that communicates with the PIV Card readers, door actuators (i.e., door locking mechanism), and the Head End System.  The Controller receives information about the PIV Card-holder from the PIV Card reader, which it uses to make access control decisions, such as to release the door locking mechanism to allow a PIV Card-holder access to a facility.  The Controller communicates to the Head End System to receive changes in the PIV Card-holder access permission.  All three of these devices work in concert to make physical access control decisions.

*	PKI validation software 

The validation software acts as an interface between the PIV Card reader and the door controller.  The software allows the PIV readers to communicate with the PACS Validation System.

*	PKI registration and management software

Used to manage PIV-Card-holders registered in the PACS database authorization requirements to a facility.

### **PACS Infrastructure**
The PACS Infrastructure is made up of many compatible and interoperable hardware and software components to include:

*	Controller (also called field panels or door controllers)

The Controller is a device that communicates with the PIV Card readers, door actuators (i.e., door locking mechanism), and the Head End System to make physical access control decisions.  The Controller receives information about the PIV Card-holder from the PIV Card reader, which it uses to make access control decisions, such as to release the door locking mechanism to allow a PIV Card-holder access to a facility.  The Controller communicates to the Head End System to receive changes in the PIV Card-holder access permission.  All three of these devices work in concert to make physical access control decisions.

*	PACS Application and Head End System (Access Control Server)

The Head End System is used to enroll an individual PIV Card-holder’s name into the database, create a unique ID number for each individual requiring physical access, and assign access privileges and an expiration date for these privileges.  The Head End server is used to maintain this information and refreshes the Controller with the latest changes.   

*	Database and Server 

The PACS Database Server, which is part of the Head End System, contains the names of the PIV Card-holders and their unique ID number and access authorization used to gain physical access to federal facilities.

* Workstation

Used with the Head End System for administration, and to register PIV Card-holder’s facility authorization into the PACS.

## FIPS 201 Compliance Testing for PACS

The GSA's FIPS 201 Evaluation Program performs compliance testing to ensure commercial products such as PACS meet federal security standards.  These standards must be met before federal agencies can purchase and implement commercial PACS within their infrastructure.  The FIPS 201 Evaluation Program test and certify PACS using third-party accredited testing labs, GSA managed testing labs, and National Institute of Standards and Technology (NIST) labs. The certification of PACS products is granted by either NIST or the Director of the FIPS 201 Evaluation Program after reviewing all materials and any testing results provided by the labs or product vendors. Once a product is certified, the product vendor is granted a letter of certification and the product information, version, date of certification, and any special considerations is placed on the GSA managed [Approved Products List (APL)](https://www.idmanagement.gov/IDM/IDMFicamProductSearchPage).  

Only PACS products listed on the APL are FIPS 201 PIV compliant and authorized for use within the federal government.  For information on how to buy approved PACS products that meet the FIPS 201 PIV standard visit [How to buy a PACS](//PACS-procurement.md)

The GSA support team also work with industry to certify engineers who have passed exams for installing and configuring physical access control systems to government requirements. The training and certification is managed by the Smart Card Alliance (non-profit).

* For additional information, please visit the Smart Card Alliance [Certified System Engineer ICAM PACS Training and Certification Program](https://www.smartcardalliance.org/activities-certified-system-engineer-icam-pacs-training-and-certification-program/).

GSA has tools available to help agencies and vendors test their products and implementations. See if there are [Product Testing Tools](https://www.idmanagement.gov/IDM/s/article_detail?link=product_testing_tools) that will help you - or contact us to suggest a useful tool that you would like.

## Resources

*Will update with reference links to info on FIPS compliance testing, PACS implementation guide, & policy docs*
