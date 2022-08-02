---
title: Data Processing Policy
section: guides
layout: page
---

At Cleversteam we take the security of our partner's data very seriously and take strong measures to negate any potential risk.

This page outlines our general policy to protecting your data.

## Ownership of Data
Cleversteam has always assigned ownership of data to our partners. This is part of our long term relationship strategy that we have with the people that we work with. It allows our partners more freedom to use the data as they wish.

It is our partner's responsibility to ensure that the individual's rights are respected and implemented. It is Cleversteam's responsibility to work with our partners, and recommend best practices based on our experience.

## Locations of Data Storage
We currently store our partner's data in 3 locations:

* **Amazon Web Services** - Dublin (IE) and Frankfurt (EU) Data Centres
* **Rackspace** - London (GB) Data Centre
* **Brightbox** - Leeds (GB) Data Centre

Upon deployment of a new project, we inform our partners of which data centre we intend to use for their data storage. We also notify and seek agreement for any to change this location.

## Processing Records
Whenever data is processed through our web systems, we keep a log of the transaction. The log files contain the fundamental information that happened in each transaction but does not contain any personal data apart from the IP address from which the transaction originated.

See "backup data" within the "data retention" section for the retention period on log files.

## Data Retention
We categorise data retention in two ways. Live data and backup data.

### Live Data
Our policy is to retain data indefinitely unless one of the following circumstances is met:

* The data held has not been accessed for 6 months and is not required for a legal business purpose
* There is a local country legislation that states data must be held for a longer period
* Our partner has requested us to delete data

### Backup Data
We retain daily snapshots of our databases and file systems for 1 year.

## Data Breach
If our partners suspect a data breach of any kind, it should be reported immediately to [support@cleversteam.com](mailto:support@cleversteam.com)

If we become aware of a data breach, we will notify our partner primary contact immediately.

Our team will then follow our internal processes to patch the issue and deploy the fix to all relevant places. After this, we will work with our partner to notify the relevant authorities and impacted individuals.

Finally a full breakdown of what happened and how it has been resolved will be supplied to our partner.

## Encryption
All of our web services use SSL with 256 bit encryption meaning data in transit is secure.

Our databases, file systems and backups are also encrypted when the data is in transit and at rest where possible.

## GDPR
### General Information
It is our commitment to work with our partners to ensure that we build GDPR compliant systems.

We do this by providing mechanisms for data management, data portability, data erasure and many more aspects. This especially includes the data subjects access rights.

This is a key part of our [approach][approach] to building safe web and mobile systems.

### Cross Border Policy
Cleversteam is based within the EU but our partners are based world wide. For this reason, we are sometimes requested to transfer our partner's data outside of the EU. We will do this as long as the following circumstances are met:

* Our non EU partner is GDPR compliant
* Our non EU partner has informed the EU data subject that their data will be transferred out of the EU and where it will be transferred to

**We refuse to carry out any request from our partner that infringes the GDPR.**

[approach]: https://www.cleversteam.com/uk/approach

## Termination of Contract
In the event that we stop working with one of our partners, Cleversteam will return all data, then completely destroy any copy that we have. We maintain that the data belongs to our partners and we have no lawful basis to hold it after the contract has ended.

## Sub Processors
We use the following sub processors:

* **New Relic**
  * Used for: Application, browser, mobile and server infrastructure health and performance monitoring
  * Address: 9th Floor 107 Cheapside, London, United Kingdom, EC2V 6DN
* **GSuite (Google Apps)**
  * Used for: Office software (word processing, non critical file storage, spreadsheets, presentations etc)
  * Address: Belgrave House, 76 Buckingham Palace Road, London, SW1W 9TQ
* **GitHub**
  * Used for: Version control and backups for our code bases
  * Address: 88 Colin P Kelly Jr St, San Francisco, CA 94107, United States
* **Circle CI**
  * Used for: Continuous Integration (this continuously runs our automated tests against any new commits to our code bases)
  * Address: 201 Spear St. #1200 San Francisco, CA 94105
* **Adobe Creative Cloud**
  * Used for: Backups and data sync for our design work
  * Address: Adobe Systems, Inc. 345 Park Ave. San Jose, CA 95110-2704
* **Slack**
  * Used for: Internal instant messaging and file sharing
  * Slack Technologies, 500 Howard Street, San Francisco, CA 94105, USA
* **Stripe**
  * Used for: Payment processing
  * Address: Stripe, Inc. 185 Berry Street, Suite 550, San Francisco, CA 94107
* **Asana**
  * Used for: Project management and partner support
  * Address: Asana, Inc. 1550 Bryant St., 8th floor, San Francisco, CA 94103
* **Rollbar**
  * Used for: Application error tracking and alerts
  * Address: 51 Federal St, San Francisco, CA 94107, USA
* **Mailchimp**
  * Used for: Our applications send emails. To send them, we use Mailchimp
  * Address: The Rocket Science Group, LLC 675 Ponce de Leon Ave NE Suite 5000. Atlanta, GA 30308 USA
* **Message Bird**
  * Our applications send text messages. To send them, we use Message Bird
  * Address: 8th fl, 6 New Street Square, New Fetter Lane, London EC4A 3AQ, United Kingdom
* **Bugsnag**
  * Used for: Bug Tracking
  * Address: 110 Sutter Street, Suite 1000, San Francisco, CA

## Contractors and Remote Workers
At Cleversteam we regularly employ contractors and remote workers. Regardless of whether they're employed on a contract basis or a full time staff basis, all staff are required to adhere to the following [security protocol][securityprotocol]

[securityprotocol]: https://cleversteam.github.io/guides/security.html

## Updates To This Policy
This policy will change over time as we further advance our processes over time. It is Cleversteam's responsibility to keep this policy up to date, to inform our partners of any change and provide a means for our partner to reject an update.

## Appointed Data Protection Officer (DPO)
Cleversteam has an appointed DPO. This is communicated to all of our partners and anybody else who needs to know.
