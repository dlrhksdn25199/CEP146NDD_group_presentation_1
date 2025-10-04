## hi we need it edit this

## GitHub Best Practices for the Project

- Create a `README.md` file with:
  - Project title, team members name and student number
  - Topic summary
  - Link to YouTube video
  - Final question
- Use GitHub Issues to track tasks (e.g., script writing, editing, voiceover).
- Assign roles clearly and document contributions.
- Commit regularly – avoid a single last-minute upload.
- Create branches and use pull requests if possible.

topic will be this https://www.forbes.com/sites/daveywinder/2025/06/20/16-billion-apple-facebook-google-passwords-leaked---change-yours-now/


## team roles
- Video Presentation   : Mateo
- Research & summary   : Timothy, Vansh
- make README.md       : Vansh
- Summary & script     : Vipishan
- Build PPTX & script  : Taishi

i put names on team roles but we need to help each other out for this. we dont have a lot of time

# CEP146NDD Group Presentation 1: Mass Credential Exposure: Apple, Google, Facebook Case Study

## Objective

The goal of this project is to research and present a current event in software development: a massive leak of 16 billion usernames and passwords affecting platforms like Apple, Google, and Facebook.  
We aim to understand the risks, implications for users and developers, and the transition toward password less authentication.

### 1. The 16-Billion Credential Leak: What Happened

In June 2025, researchers uncovered a massive compilation of over **16 billion login credentials**, including usernames and passwords, exposed across approximately 30 datasets on the dark web. These datasets predominantly originated from **infostealer malware** and **historical data breaches**. Notably, major platforms like **Apple, Google, and Facebook** were not directly breached; instead, their user credentials were found in these aggregated datasets.

The data was briefly accessible due to misconfigured servers but was promptly removed upon discovery. Despite the brief exposure, the sheer volume of compromised credentials poses significant risks to users and organizations alike. multiple cybersecurity teams reported that 16 billion usernames and passwords surfaced across ~30 exposed datasets on the dark web.  The leak is **not a single hack** but a compilation of past breaches, malware theft, and credential stuffing combo lists.  

Some reports cast doubt on the full scale; BleepingComputer notes that the figure may be inflated due to duplicates, but even partial exposure is significant.  
Sources: [Forbes](https://www.forbes.com/sites/daveywinder/2025/06/20/16-billion-apple-facebook-google-passwords-leaked---change-yours-now/), [Malwarebytes](https://www.malwarebytes.com/blog/news/2025/06/billions-of-logins-for-apple-google-facebook-telegram-and-more-found-exposed-online), [The Guardian](https://www.theguardian.com/technology/2025/jun/21/internet-users-advised-to-change-passwords-after-16bn-logins-exposed)
The compromised datasets were primarily composed of:

- **85% from infostealer malware**: Malicious software designed to harvest login credentials and other sensitive information from infected devices.

- **15% from historical data breaches**: Credentials leaked from past security incidents involving various platforms.

These credentials were typically stored in a structured format, such as:

(https://www.facebook.com/:jsmith@example.com:Databr3achFUd!)
(https://www.bank.com/login.php:jsmith:SkyIsFa11ing#)
(https://x.com/i/flow/login:jsmith@example.com:StayCalmCarryOn)

This structured format facilitates automated attacks, such as credential stuffing, where attackers use stolen credentials to gain unauthorized access to multiple accounts across different platforms.

### 2. Risks & Implications

The exposure of such a vast number of credentials presents several critical risks:

- **Credential Stuffing Attacks:** Attackers can use the compromised credentials to attempt unauthorized logins across multiple platforms, taking advantage of users who reuse passwords.  

- **Identity Theft and Fraud:** Access to personal data can enable identity theft, financial fraud, and other malicious activities.  

- **Phishing Campaigns:** Cybercriminals may craft highly convincing phishing emails using the exposed data, increasing the likelihood of successful attacks.  

- **Operational Costs:** Companies face significant expenses for breach investigations, regulatory compliance, notifying affected users, and potential compensations.  

- **Public Trust & Reputational Damage:** Even if not directly breached, organizations whose users’ credentials are exposed may lose user trust and face long-term reputational harm.  

### 3. Developer & Software Design Implications

- *Never store passwords in plain text*; always use strong hashing (bcrypt, Argon2) with unique salts.  

- *Implement Multi-Factor Authentication (MFA):* Require users to verify their identity with two or more factors (e.g., authenticator apps, SMS codes, hardware tokens).  

- *Adopt passwordless / passkey technologies:* Transition to authentication methods such as biometrics or cryptographic keys, reducing risks from stolen passwords.  

- *Encourage password managers:* Help users generate and securely store strong, unique credentials for every account.  

- *Use breach-detection APIs:* Integrate services like *Have I Been Pwned* to detect compromised credentials and prompt users to reset them.  

- *Apply secure coding practices:* Validate input, limit login attempts, monitor suspicious activity, secure sessions, and encrypt data both in transit and at rest. 
 
- *Prioritize user education & UX:* Provide guidance toward strong credentials, make secure options the default, and build intuitive flows that don’t frustrate users.  

By proactively implementing these design principles, developers can significantly reduce the impact of credential leaks and strengthen overall system resilience.
