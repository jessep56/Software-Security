# Software Security Project

This project demonstrates the development and deployment of a secure Java server application using best practices for encryption, secure communications, and vulnerability management.

It was developed as part of a course project for CS 305 - Software Security.

## 🔐 Project Objectives

- Implement secure communication protocols (SSL/TLS)
- Generate and use a self-signed SSL certificate
- Apply checksum verification for data integrity
- Use Advanced Encryption Standard (AES) for encryption
- Refactor code to eliminate identified security vulnerabilities
- Perform dependency vulnerability scanning using OWASP Dependency-Check

## 🛆 Project Structure

| Folder/File | Description |
| :--- | :--- |
| `/src` | Java source code for the server application |
| `pom.xml` | Maven configuration file (manages dependencies and build) |
| `selfsigned.cer` | Self-signed SSL certificate for HTTPS setup |
| `.mvn/` | Maven wrapper files for building the project |
| `dependency-check-report.html` (if generated) | Security report from OWASP Dependency-Check |
| `checksum.txt` | Checksum file for verifying data integrity |

## 🛠 Technologies Used

- Java 11
- Maven
- SSL/TLS (Secure Sockets Layer/Transport Layer Security)
- AES (Advanced Encryption Standard) 256-bit encryption
- SHA-256 checksum algorithm
- OWASP Dependency-Check

## 🚀 Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/jessep56/Software-Security.git
   cd Software-Security
   ```

2. **Build the project with Maven**:
   ```bash
   mvn clean install
   ```

3. **Run the server**:
   ```bash
   mvn exec:java -Dexec.mainClass="your.main.ClassName"
   ```
   *(replace `your.main.ClassName` with the actual server's main class)*

4. **Access the server** over HTTPS using the generated self-signed certificate.

> ⚠️ **Note**: Browsers may flag the self-signed certificate as untrusted — this is expected for testing purposes.

## 🧪 Testing and Validation

- **SSL Certificate**: Verified using browser access over HTTPS.
- **Checksum Verification**: Implemented SHA-256 checksum validation.
- **Functional Testing**: Server tested to ensure secure connections.
- **Dependency Analysis**: Vulnerabilities detected and mitigated using OWASP Dependency-Check.

## 🛡 Security Enhancements

- Enforced HTTPS-only communication
- Generated secure 2048-bit SSL certificate
- Integrated AES symmetric encryption
- Applied checksum verification to detect tampering
- Refactored code to meet OWASP secure coding standards

## 📄 Summary

This project integrates multiple layers of security to protect communications, data integrity, and dependency management. It demonstrates practical application of industry best practices in securing software and servers.

---

## 📚 References

- [OWASP Dependency-Check](https://owasp.org/www-project-dependency-check/)
- [Advanced Encryption Standard (AES)](https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.197.pdf)
- [SSL/TLS Concepts](https://www.ssl.com/faqs/faq-what-is-ssl-tls-https/)

---
