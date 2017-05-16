# Database

- [ ] Use encryption for data identifying users and sensitive data like access tokens, email addresses or billing details.
- [ ] If your database supports low cost encryption at rest (like AWS Aurora), then enable that to secure data on disk. Make sure all backups are stored encrypted as well.
- [ ] Use minimal privilege for the database access user account. Don’t use the database root account.
- [ ] Store and distribute secrets using a key store designed for the purpose. Don’t hard code in your applications.
- [ ] Fully prevent SQL injection by only using SQL prepared statements. For example: if using NPM, don’t use npm-mysql, use npm-mysql2 which supports prepared statements.

# Development

# Authentication

# Denial of Service Protection

# Web Traffic

# APIs

# Validation

# Cloud Configuration

# Infrastructure

# Operation

# Test

# Finally, have a plan
