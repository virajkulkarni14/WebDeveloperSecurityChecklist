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

# Web Traffic

# APIs

# Validation

# Cloud Configuration

# Infrastructure

# Operation

# Test

# Finally, have a plan
