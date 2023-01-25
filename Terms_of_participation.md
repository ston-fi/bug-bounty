<h1 align="center">Terms of participation</h1>
<p align="center">This document describe how to participate</p>

These are the terms (the “Agreement”) governing your participation in the Bug Bounty program (hereafter referred to as the “Event”), organised by STON.FI ("[STON.fi](http://ston.fi/)", "STON", we). By participating for the Event you agree to these terms.

The program starts from the moment the article is published on official github account and ends when the STON informs about it by any means of its choice including update program description on github.

<h2 align="center">Participation process</h2>

The Event is free and without any purchase obligation but participation subject to the following minimum conditions:

* The vulnerability must meet the requirements for the type of vulnerability
* The report must be sent in the way described in the program
* Report must contain Proof of Concept

After submission, the report will be reviewed by a special judges. Review time is not regulated.

<h2 align="center">Modification, interruption and termination</h2>

STON reserves the right to shorten, extend, modify or terminate the Bug Bounty program for any reason without incurring liability from the participant as a result thereof. In such cases, we will provide notice thereof to the Participants by any means of its choice (including publication on this website, social media), and, if the need arises, will communicate to the Participants the new rules applicable, or the new ending date of the Bug Bounty program as the case may be.

<h2 align="center">Reports</h2>

If the bug or issue is already known to the project prior to the submission of the report, then they can close the bug report without providing a reward to the participant. The project can prove prior knowledge by providing:

- A reference to a previous bug report
- A Git PR
- An audit report
- A blog post
- A screenshot of an email with dates that clearly states the vulnerability and its impacts

<h3 align="center">Proof of Concept (PoC)</h3>

In the web3 world, a Proof of Concept (PoC) is runnable code that demonstrates that a bug/vulnerability and impact are real without actually exploiting the vulnerability in a live environment.

<h3 align="center">PoC Guidelines</h3>

- The smart contract PoC should always be made by forking the mainnet, but not by deploying and setting up the local off-chain contract state which doesn’t match with the on-chain state of the contract.
- The PoC should contain runnable code for the exploit demonstration. Screenshots of code are not acceptable. The participant can choose any framework or language to write a PoC. The participant should mention all the dependencies, configuration files, and environmental variables that are required in order to run that PoC, as any other requirements to run the test.
- PoCs should have clear print statements and or comments that detail each step of the attack and display relevant information.
- The participant can upload the PoC containing all the configuration files directly to Google Drive and share the link in the submission on the official communication channel.
- Alternatively, if the PoC is simple enough that it doesn’t require any configuration files, then it can be shared in the submission itself by pasting out the code.

If participant do not follow the guidelines, their reports may be closed.

<h3 align="center">PoC Rules</h3>

- Do not test on public testnet or mainnet.
- Do not submit a partial or incomplete PoC.

Violation of any of these rules will, in almost all cases, result in an immediate user ban in the STON Bug Bounty program.