# Database

- [ ] Use encryption for data identifying users and sensitive data like access tokens, email addresses or billing details.
- [ ] If your database supports low cost encryption at rest (like AWS Aurora), then enable that to secure data on disk. Make sure all backups are stored encrypted as well.
- [ ] Use minimal privilege for the database access user account. Don’t use the database root account.
- [ ] Store and distribute secrets using a key store designed for the purpose. Don’t hard code in your applications.
- [ ] Fully prevent SQL injection by only using SQL prepared statements. For example: if using NPM, don’t use npm-mysql, use npm-mysql2 which supports prepared statements.

# Development

- [ ] Ensure that all components of your software are scanned for vulnerabilities for every version pushed to production. This means O/S, libraries and packages. This should be automated into the CI-CD process.
- [ ] Secure development systems with equal vigilance to what you use for production systems. Build the software from secured, isolated development systems.


# Authentication

- [ ] Ensure all passwords are hashed using appropriate crypto such as bcrypt. Never write your own crypto and correctly initialize crypto with good random data.
- [ ] Implement simple but adequate password rules that encourage users to have long, random passwords.
- [ ] Use multi-factor authentication for your logins to all your service providers.

# Denial of Service Protection

- [ ] Make sure that DOS attacks on your APIs won’t cripple your site. At a minimum, have rate limiters on your slower API paths like login and token generation routines.
- [ ] Enforce sanity limits on the size and structure of user submitted data and requests.
- [ ] Use Distributed Denial of Service (DDOS) mitigation via a global caching proxy service like CloudFlare. This can be turned on if you suffer a DDOS attack and otherwise function as your DNS lookup.

# Web Traffic

- [ ] Use TLS for the entire site, not just login forms and responses. Never use TLS for just the login form.
- [ ] Cookies must be httpOnly and secure and be scoped by path and domain.
- [ ] Use CSP without allowing unsafe-* backdoors. It is a pain to configure, but worthwhile.
- [ ] Use X-Frame-Option, X-XSS-Protection headers in client responses
- [ ] Use HSTS responses to force TLS only access. Redirect all HTTP request to HTTPS on the server as backup.
- [ ] Use CSRF tokens in all forms and use the new SameSite Cookie response header which fixes CSRF once and for all newer browsers.

# APIs

- [ ] Ensure that no resources are enumerable in your public APIs.
- [ ] Ensure that users are fully authenticated and authorized appropriately when using your APIs.

# Validation

- [ ] Do client-side input validation for quick user feedback, but never trust it.
- [ ] Validate every last bit of user input using white lists on the server. Never directly inject user content into responses. Never use user input in SQL statements.

# Cloud Configuration

# Infrastructure

# Operation

# Test

# Finally, have a plan
