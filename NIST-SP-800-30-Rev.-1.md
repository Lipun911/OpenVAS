**NIST SP 800-30 Rev. 1** 

## **Guide to assessing risk** 

NIST SP 800-30 is a publication that provides guidance on performing risk assessments. It outlines strategies for identifying, analyzing, and remediating risks. Organizations use NIST SP 800-30 to gain insights into the potential likelihood and severity of risks—helping them make informed decisions about allocating resources, implementing controls, and prioritizing remediation efforts. 

This four page document is adapted from NIST SP 800-30 Rev. 1. The term "Rev. 1" signifies that it is the first updated version of this publication. NIST occasionally revises its documents to incorporate new information, reflect changes in technology and regulatory requirements, or address feedback. 

**Note:** NIST's Computer Security Resources Center contains more information on SP 800-30 Rev. 1. 

## **Threat sources** 

NIST SP 800-30 defines and categorizes threat sources as entities or circumstances that can negatively impact an organization's information systems. This information is useful for identifying and assessing potential risks. When referencing it, consider the intent/capabilities of either internal and external threat sources. 

**Note:** The following table lists a few possible _threat sources_ that could compromise a publicly accessible database server. 

|**Type**|**Examples**|**Description**|
|:---:|---|---|
|Human|_Standard user_<br>&emsp; ●Employee<br>&emsp; ●Customer<br>_Privileged user_<br>&emsp; ●System administrator &emsp; Group<br>&emsp; ●Competitor<br>&emsp; ●Supplier<br>&emsp; ●Business partner<br>&emsp; ●Nation state<br>_Outsider_<br>&emsp; ●Hacker<br>&emsp; ●Hacktivist<br>&emsp; ●Advanced persistent threat<br>(APT)|Threats arising from individuals or groups who might<br>purposefully or accidentally exploit cyber resources. For example, they might alter data in a way that<br>negatively impacts the company. Alternatively, they might intentionally steal data and damage business equipment.|
|Technological|_Hardware_<br>&emsp; ●Storage<br>&emsp; ●Processing<br>&emsp; ●Communications<br>_Software_<br>&emsp; ●Operating system(s)<br>&emsp; ●Networking<br>&emsp; ●Malicious software<br>|Threats that originate from non-human factors. For example, failures of equipment due to aging, resource depletion, or other circumstances.|
|Enviromental|_Operational environment_<br>&emsp; ●Temperature controls<br>&emsp; ●Humidity controls<br>&emsp; ●Faulty power supplies<br>_Natural hazards_<br>&emsp; ●Power outages<br>&emsp; ●Extreme weather events<br>|Threats that arise from accidental, non-human factors. For example, equipment failures caused by the operational environment.|



## **Threat events** 

NIST SP 800-30 defines and categorizes threat events as actual instances where a threat source exploits a vulnerability and causes damage or harm to an organization's information systems. This information is useful for gaining insights into the types of risks that assets face. More effective controls and countermeasures can be identified by understanding possible threat events, 

**Note:** The following table lists just a few possible _threat events_ that could compromise a publicly accessible database server. 

|**Examples**|**Description**|
|---|---|
|Perform reconnaissance and surveillance of organization|Threat source examines and assesses the company's vulnerabilities over time using various<br>tools (e.g., scanning, physical observation).|
|Obtain sensitive information via exfltration|Threat source installs malicious sofware on organizational systems to locate and acquire sensitive information.|
|Alter/Delete critical information|Threat source alters or deletes data that is<br>critical to day-to-day business operations.|
|Craft counterfeit certifcates.|Threat source compromises a certifcate authority to make their connections appear<br>legitimate.|
|Install persistent and targeted network sniffers on organizational information systems.|Threat source installs sofware designed to<br>collect (sniff) network traffic over a continued period of time.|
|Conduct Denial of Service (DoS) attacks.|Threat source sends automated, excessive requests to overwhelm the system's operating capabilities.|
|Disrupt mission-critical operations.|Threat source compromises the integrity of<br>information in such a way that prevents the<br>business from carrying out critical operations.|
|Obfuscate future atacks.|Threat source takes actions to inhibit the effectiveness of the intrusion detection systems or auditing capabilities at the company.|
|Conduct "man-in-the-middle" atacks.|Threat source eavesdrops on sessions between<br>internal and external systems. Later, they relay<br>messages between organizational and external systems that make them believe they're talking directly to each other over a private connection.|



## **Likelihood of a threat event** 

In general, the _likelihood_ of a threat event should be a score based on a combination of factors. For example, any available evidence that you have, prior experience, and your expert judgment. 

Consider the intent/capabilities of a threat source and potential threat events when producing a likelihood score.  


|**Qualitative values**|**Quantitative values**|**Description**|
|:---:|:---:|---|
|High|3|Threat source is almost certain to initiate a security event. An event could have multiple, severe, or catastrophic effects on business operations and<br>assets.|
|Moderate|2|Threat source is somewhat likely to initiate a security event. An event could significantly reduce the functionality of organizational operations and<br>assets.|
|Low|1|Threat source is highly unlikely to initiate a security event. An event could have minor, negligible effects on business operations and assets.|



## **Severity of a threat event** 

In general, the _severity_ of a threat event is a measure of its potential impact to business operations. For example, would the event cause a business function to stop entirely? Might it temporarily disrupt a business process and go unnoticed? 

Consider the business impact of _threat events_ when producing a severity score. 

|**Qualitative values**|**Quantitative values**|**Description**|
|:---:|:---:|---|
|High|3|Threat source is almost certain to initiate a security event. An event could have multiple, severe, or catastrophic effects on business operations and assets.|
|Moderate|2|Threat source is somewhat likely to initiate a security event. An event could signifcantly reduce the functionality of organizational operations and assets.|
|Low|1|Threat source is highly unlikely to initiate a security event. An event could have minor, negligible effects on business operations and assets.|



4 

