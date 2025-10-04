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

- (https://www.facebook.com/:jsmith@example.com:Databr3achFUd!)
- (https://www.bank.com/login.php:jsmith:SkyIsFa11ing#)
- (https://x.com/i/flow/login:jsmith@example.com:StayCalmCarryOn)

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

### 4. The Transition to Passwordless / Passkeys

The widespread exposure of credentials has highlighted the weaknesses of traditional password-based authentication. In response, both tech companies and academic research are advocating for more secure alternatives:

- **Industry Adoption of Passwordless Sign-In:** Microsoft and other technology companies are promoting *phishing-resistant, passwordless sign-in methods*. These approaches reduce reliance on traditional passwords, which are vulnerable to leaks and attacks.

- **Surge in Passkey Usage:** Bitwarden, a popular password manager, reported a *550% increase in passkey creation* in late 2024. This reflects the growing adoption of passwordless authentication among users and organizations.

- **Organizational Shift Towards Passwordless Authentication:** Organizations are adopting passwordless solutions due to *increasing cyber threats, regulatory pressure, and the risks associated with managing passwords*. This trend helps improve security and user experience.

- **Academic Insights on Passkey Security:** Research shows passkeys are *more secure and user-friendly than traditional Time-Based One-Time Passwords (TOTP)*. Passkeys resist phishing attacks and credential reuse, addressing common vulnerabilities in password-based systems.

- **Implementation Considerations:** Passkeys can be *device-bound* (tied to a single device) or *synced across devices*. Device-bound passkeys offer stronger security, while synced passkeys improve usability. Organizations must balance these trade-offs.

*Sources:*  
- [Microsoft Blog](https://blogs.microsoft.com/blog/2025/05/15/passwordless/)  
- [AuthSignal Blog](https://authsignal.com/blog/passkey-adoption)  
- [arXiv Paper on Passkey Implementation](https://arxiv.org/abs/2508.11928)

### 5. Balanced View & Criticism

While the 16-billion-credential leak has drawn widespread attention, several experts urge a cautious interpretation of the scale:

- **Inflated Numbers:** Some cybersecurity analysts argue that the *16 billion figure is exaggerated* because many of the credentials are duplicates or recycled from older breaches. Therefore, the total number of unique compromised accounts may be lower than initially reported.

- **Data from Older Breaches:** According to BleepingComputer, much of the leaked data does not represent a new breach. Instead, it mostly consists of credentials that have already appeared in previous leaks and are circulating in various combo lists or dark web marketplaces.

- **Demonstrates Systemic Weakness:** Even with possible inflation, the leak highlights the *inherent weaknesses of password-based security*. User behavior, such as password reuse and weak passwords, continues to pose a serious risk, emphasizing the need for stronger authentication methods.

- **Awareness and Response:** The debate around the exact number also underscores the importance of transparency, responsible reporting, and proactive security measures by both companies and end-users. It serves as a reminder for organizations to continuously monitor and improve their security practices.

*Sources:*  
- [BleepingComputer Article](https://www.bleepingcomputer.com/news/security/16-billion-passwords-leaked/)  
- [Cybernews Report](https://www.cybernews.com/news/massive-password-leak/)

### 📘 Summary: 16-Billion Credential Leak & Passwordless Authentication

In June 2025, over **16 billion login credentials** were exposed across ~30 datasets on the dark web, mainly from **infostealer malware** and **historical data breaches**. Major platforms like **Apple, Google, and Facebook** were not directly breached, but their user credentials were found in aggregated datasets.  

### Key Risks:
- **Credential Stuffing Attacks:** Using leaked credentials to access multiple accounts.  
- **Identity Theft & Fraud:** Personal data may be exploited for financial or identity crimes.  
- **Phishing Campaigns:** More convincing phishing attempts using exposed data.  
- **Operational Costs:** Expenses for investigations, compliance, notifications, and compensation.  
- **Public Trust & Reputation:** Organizations may lose user trust even without a direct breach.  

### Developer & Software Implications:
- Store passwords securely (hashing with bcrypt/Argon2 + salts).  
- Implement **MFA** and encourage password managers.  
- Adopt **passwordless/passkey technologies** for improved security.  
- Apply secure coding practices: input validation, session security, encryption.  
- Educate users on strong credentials and intuitive flows.  

### Passwordless / Passkeys Adoption:
- Companies like **Microsoft** promote phishing-resistant, passwordless sign-ins.  
- **Bitwarden** reported a 550% increase in passkey creation in 2024.  
- Research shows passkeys are more secure and user-friendly than TOTP.  
- Consider trade-offs: device-bound vs synced passkeys.  

### Criticism & Balanced View:
- Some experts argue the **16-billion figure** is inflated due to duplicates.  
- Most data comes from **older breaches**, but it highlights password-based security weaknesses.  
- Emphasizes the need for proactive security, monitoring, and user education.  

---

### references
- [Forbes](https://www.forbes.com/sites/daveywinder/2025/06/20/16-billion-apple-facebook-google-passwords-leaked---change-yours-now/)  
- [Malwarebytes](https://www.malwarebytes.com/blog/news/2025/06/billions-of-logins-for-apple-google-facebook-telegram-and-more-found-exposed-online)  
- [The Guardian](https://www.theguardian.com/technology/2025/jun/21/internet-users-advised-to-change-passwords-after-16bn-logins-exposed)  
- [Microsoft Blog](https://blogs.microsoft.com/blog/2021/10/28/america-faces-a-cybersecurity-skills-crisis-microsoft-launches-national-campaign-to-help-community-colleges-expand-the-cybersecurity-workforce/)  
- [AuthSignal Blog](https://authsignal.com/blog/articles/world-passkey-day-the-state-of-passkeys-in-2025)  
- [arXiv Paper on Passkey Implementation](https://arxiv.org/abs/2508.11928)  
- [BleepingComputer](https://www.bleepingcomputer.com/news/security/16-billion-passwords-leaked/)  
- [Cybernews Report](https://www.cybernews.com/news/massive-password-leak/)
