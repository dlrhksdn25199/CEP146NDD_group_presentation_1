# CEP146NDD Group Presentation 1: Mass Credential Exposure: Apple, Google, Facebook Case Study 

### note: Speaker copy, "Script:" part is the one you speak first, and then talk about "-". If you have any questions about the script | pptx call either one.

### Slide 1 – Title 
Mass Credential Exposure: Apple, Google, Facebook Case Study
Group Presentation – CEP146NDD
Script:
Welcome everyone. Today, our group will be presenting a case study on one of the largest credential exposures in recent history — involving over 16 billion login credentials. While Apple, Google, and Facebook weren’t directly breached, their users’ data appeared in massive compilations on the dark web. Let’s dive into what happened, why it matters, and how the industry is responding.

### Slide 2 – Objective
Script:
Our goal is to examine this major event in software development — the 16-billion credential leak — and understand its broader implications. We’ll explore the risks it poses to users and organizations, the lessons developers can take away, and how the industry is shifting toward passwordless authentication to prevent future incidents.

### Slide 3 – What Happened
Script:
In June 2025, researchers uncovered a massive trove of login credentials — over 16 billion — spread across roughly 30 datasets on the dark web. Importantly, this wasn’t a single hack. Instead, it was a compilation of stolen data from infostealer malware and older breaches.
About 85% came from malware that harvested credentials from infected devices, and 15% from historical breaches.
Even though platforms like Apple, Google, and Facebook weren’t directly compromised, their users’ credentials were found in these datasets — often in structured formats like this:

- https://facebook.com : jsmith@example.com : Databr3achFUd!

This format makes it easy for attackers to automate credential stuffing attacks.

### Slide 4 – Risks & Implications
Script:
The exposure of billions of credentials creates serious risks:
- First, credential stuffing — attackers use stolen credentials to try logging into other accounts, especially when users reuse passwords.
- Second, identity theft and fraud — personal data can be exploited for financial gain.
- Third, phishing campaigns — attackers craft convincing emails using leaked info.
- Companies also face operational costs for investigations, compliance, and user notifications.
- And finally, even if a company wasn’t breached, the appearance of its users’ data can lead to loss of trust and reputational damage.

### Slide 5 – Developer & Design Lessons
Script:
So what can developers do?
- Never store passwords in plain text. Use strong hashing algorithms like bcrypt or Argon2, with unique salts.
- Enforce multi-factor authentication to add layers of security.
- Integrate breach-detection APIs like Have I Been Pwned to alert users if their credentials are compromised.
- Encourage the use of password managers to generate and store strong, unique passwords.
- Apply secure coding practices — validate input, encrypt data, limit login attempts, and secure sessions.
- And finally, educate users through intuitive design that promotes secure behavior by default.

### Slide 6 – Passwordless / Passkeys
Script:
The industry is moving beyond passwords.
- Companies like Microsoft and Google are promoting passwordless sign-ins that resist phishing.
- Bitwarden reported a 550% increase in passkey creation in 2024 — showing strong adoption.
- Passkeys are more secure and user-friendly than traditional one-time passwords.
- There are two types:
- Device-bound passkeys offer stronger security.
- Synced passkeys improve convenience across devices.
Organizations must balance these trade-offs as they transition to passwordless systems.

### Slide 7 – Criticism & Balanced View
Script:
Some experts caution that the 16-billion figure may be inflated — many credentials are duplicates or recycled from older breaches.
But even if the numbers are overstated, the leak still exposes systemic weaknesses in password-based security.
It highlights poor user habits like password reuse and the need for transparent reporting and ongoing user education.
Ultimately, it’s a wake-up call for the entire industry.

### Slide 8 – Summary
Script:
To wrap up:
- Over 16 billion credentials were exposed — mostly from malware and past breaches.
- The risks include credential stuffing, identity theft, phishing, and loss of trust.
- Developers must adopt secure storage, MFA, passkeys, and breach detection.
- And as we’ve seen, passwordless authentication is emerging as the future — offering better security and user experience.
Thank you!


