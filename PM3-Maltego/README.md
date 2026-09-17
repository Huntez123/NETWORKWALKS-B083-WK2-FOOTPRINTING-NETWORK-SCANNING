PM3 — Footprinting with Maltego

Module Overview

This module focused on footprinting and reconnaissance using Maltego Graph.

The practical exercise required Maltego to be installed on a Windows computer and used to identify email addresses related to the authorized target organization domain.

**Target:** `networkwalks.com`

Task 1 — Maltego Installation

Maltego Graph was installed and configured on a Windows computer.

The installation and configuration process included:

- Installing Maltego Graph
- Completing the initial setup
- Creating and activating a Maltego ID
- Configuring the application
- Preparing Maltego to run transforms

Task 2 — Email Address Reconnaissance

A Domain entity was created in Maltego and configured with:

`networkwalks.com`

Email-related transforms were then executed against the Domain entity.

Transform 1

**Transform:** `[Utilities] To Emails @domain [Search Engine]`

The transform was executed successfully but did not return an Email Address entity in the current Maltego environment.

Transform 2

**Transform:** `[Utilities] To E-Mail Addresses [within Properties]`

The transform was also executed successfully but did not return an Email Address entity.

The results differed from the example shown in the Networkwalks training material. The practical documentation notes that reconnaissance results may vary depending on the tools, services, and information sources available at the time of testing.

Observed Result

The Maltego graph retained the `networkwalks.com` Domain entity after the email-related transforms completed.

No Email Address entity was returned by the two transforms used during the exercise.

The result was recorded as observed rather than reproducing or assuming the example result from the training material.

Evidence

Evidence was collected using screenshots of the Maltego Graph interface and transform execution results.

The evidence demonstrates:

- Maltego Graph running successfully
- `networkwalks.com` Domain entity
- Email-related transform execution
- Successful completion of the transforms
- No Email Address entity returned

Scope

**Authorized Training Target:** `networkwalks.com`

The activities were performed as part of the Networkwalks Cybersecurity Internship for educational and authorized reconnaissance training.

Responsible Use

Maltego is an OSINT and reconnaissance platform capable of collecting information from multiple sources.

The information gathered through reconnaissance should only be used within an authorized scope and for legitimate security research, education, assessment, and defensive purposes.

Module Status

**Completed**

Networkwalks Cybersecurity Internship

**Batch:** B083  
**Participant:** Dan Ngechu  
**Module:** W2-PM3  
**Activity:** Footprinting with Maltego
