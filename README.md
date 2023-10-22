# CS305
Software Security

The client for this project, Artemis Financial needs a web application with security features that are adequate for protecting sensitive customer and business data. 

There were several vulnerable dependencies found in a static test of the program. Additionally, the lack of encryption and client/server validation posed a significant risk to the company. The third major risk uncovered was the lack of input validation on the HTTPs request. Poor security could be very costly to a company, particularly a financial institution which has a legal obligation to their customers to protect their data. Through improving security, Artemis Financial is protecting themselves and their customers from malicious actors. 

The most difficult part of the vulnerability assessment for me was the mitigation plan for resolving vulnerabilities in the dependency report. There were several recommended resolutions I found that I did not know how to implement. In future work, more should be done to address some of these vulnerable dependencies. 

To increase the layers of security, I first encrypted the data that was being transmitted in the get request. I also implemented a security certificate to protect the site from unauthorized users. Both the data encryption and the certificate used asymmetric encryption algorithms, which provide verification of the data’s integrity in addition to concealment from bad actors. The next layer of security I added was input validation. This will help prevent code injection by limiting the length and characters accepted in the get request. 

To ensure the software was secure, I ran a second static test and verified that no new vulnerable dependencies were introduced. I completed a manual review of the program and tested the program by testing the HTTPS request with invalid authorization and input. 

