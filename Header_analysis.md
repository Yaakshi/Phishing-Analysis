# Analyse Email Headers

Phishing sample: https://github.com/rf-peixoto/phishing_pot/blob/main/email/sample-10.eml
![image](https://github.com/user-attachments/assets/39d6a028-114f-46dd-b172-3927a6896f6e)

Legitimate email from my Inbox:
![image](https://github.com/user-attachments/assets/ca9dffe3-e2bb-4329-986d-105d4b3a3f2c)

#### Analysing the Hyperlinks in the Emails

![image](https://github.com/user-attachments/assets/5e06d341-36a6-4fd0-9b45-38d03263ca0e)
(Used https://www.emlreader.com/ to view .eml files)

![image](https://github.com/user-attachments/assets/ff414402-c3a5-4d63-b5e4-55d0552bb462)
- The fraudulent email points to a random email whereas the legitimate email points to Microsoft URL.

#### Analysing email headers

Tool: https://mxtoolbox.com/EmailHeaders.aspx

1. Click the three dots at the top-right corner of the email --> Click Show Original to view email headers.
![image](https://github.com/user-attachments/assets/9e1b3046-30b4-4694-9fd6-d5bac83dd000)
2. Open the online header analyser tool and copy the headers for further analysis.

Fraudulent email:

![image](https://github.com/user-attachments/assets/b97cc278-d910-45a0-8b3c-b4aa9d90d11b)

Legitimate email:

![image](https://github.com/user-attachments/assets/dcd1ff6e-7e24-4833-9e54-994ea689de66)

### DMARC, SPF, DKIM
- Together, they help prevent spammers, phishers, and other unauthorized parties from sending emails on behalf of a domain they do not own.
- DomainKeys Identified Mail (DKIM) enables domain owners to automatically "sign" emails from their domain, just as the signature on a check helps confirm who wrote the check. The DKIM "signature" is a digital signature that uses cryptography to mathematically verify that the email came from the domain.
- Sender Policy Framework (SPF) is a way for a domain to list all the servers they send emails from. It lists all the IP addresses of all the servers that are allowed to send emails from the domain.
- Domain-based Message Authentication Reporting and Conformance (DMARC) tells a receiving email server what to do given the results after checking SPF and DKIM. 
