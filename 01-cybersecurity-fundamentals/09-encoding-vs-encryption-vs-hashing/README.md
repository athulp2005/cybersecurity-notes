# Encoding vs Encryption vs Hashing

## 📖 Overview

Encoding, Encryption, and Hashing are three different techniques used in computing and cybersecurity. Although they may appear similar, each serves a different purpose.

Understanding the differences between these concepts is essential for anyone beginning a cybersecurity journey.

---

## 🎯 Learning Objectives

After completing this topic, you should be able to:

- Understand the purpose of Encoding.
- Understand the purpose of Encryption.
- Understand the purpose of Hashing.
- Compare Encoding, Encryption, and Hashing.
- Identify common real-world applications.

---

# 📄 Encoding

Encoding is the process of converting data from one format into another so that different systems can correctly store or transmit the data.

### Purpose

- Improve compatibility
- Support data transmission
- Standardize data formats

### Common Examples

- Base64
- ASCII
- Unicode
- URL Encoding

> **Note:** Encoding is **not** intended to provide security.

---

# 🔐 Encryption

Encryption converts readable data (plaintext) into unreadable data (ciphertext) using an encryption algorithm and a key.

Only someone with the correct key can decrypt the data back into its original form.

### Purpose

- Protect confidential information
- Secure communication
- Prevent unauthorized access

### Common Uses

- HTTPS
- VPN
- Secure messaging
- Online banking

---

# 🔑 Hashing

Hashing converts data into a fixed-length value called a **hash**.

Unlike encryption, hashing is a **one-way process**, meaning the original data cannot normally be recovered from the hash.

### Purpose

- Verify data integrity
- Store passwords securely
- Detect file modifications

### Common Algorithms

- SHA-256
- SHA-512
- bcrypt
- Argon2

---

# 📊 Comparison

| Feature | Encoding | Encryption | Hashing |
|---------|----------|------------|----------|
| Purpose | Data formatting | Data protection | Data integrity |
| Reversible | Yes | Yes (with key) | No |
| Uses a Key | No | Yes | No |
| Security | No | Yes | No (integrity only) |
| Common Example | Base64 | AES | SHA-256 |

---

# 🌍 Real-World Examples

### Encoding

A web application converts binary data into Base64 so it can be transmitted safely in text format.

---

### Encryption

An online banking website encrypts customer information before transmitting it over the internet.

---

### Hashing

A website stores a hash of a user's password instead of storing the actual password.

---

# 💡 Key Points

- Encoding changes the format of data.
- Encryption protects confidential information.
- Hashing verifies integrity and securely stores passwords.
- These techniques have different purposes and should not be confused.

---

# 📌 Summary

Encoding, Encryption, and Hashing are important concepts in cybersecurity. Encoding improves compatibility, Encryption protects sensitive information, and Hashing verifies data integrity and supports secure password storage.

---

# ❓ Quick Review

1. What is Encoding?
2. What is Encryption?
3. What is Hashing?
4. Which technique uses a key?
5. Which technique is one-way?
6. Give one real-world example of each.
