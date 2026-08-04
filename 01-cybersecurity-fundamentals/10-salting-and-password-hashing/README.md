# Salting and Password Hashing

## 📖 Overview

Password hashing and salting are essential techniques used to protect user passwords. Instead of storing passwords in plain text, organizations store hashed passwords. A unique salt is added before hashing to make passwords more resistant to attacks.

These techniques help improve the security of authentication systems and reduce the risk of password theft.

---

## 🎯 Learning Objectives

After completing this topic, you should be able to:

- Understand password hashing.
- Understand the purpose of salting.
- Explain why passwords should never be stored in plain text.
- Understand how salting improves password security.

---

# 🔑 Password Hashing

Password hashing is the process of converting a password into a fixed-length hash value using a hashing algorithm.

The original password cannot normally be recovered from the hash.

### Why Hash Passwords?

- Protect user passwords
- Prevent plain-text password storage
- Improve authentication security
- Verify passwords without storing the original password

---

# 🧂 What is Salting?

A salt is a random value added to a password before it is hashed.

Each user receives a different salt, even if two users choose the same password.

### Why Use Salting?

- Prevents identical passwords from producing identical hashes
- Protects against rainbow table attacks
- Makes password cracking more difficult
- Improves password security

---

# 🔄 Password Storage Process

1. User creates a password.
2. The system generates a unique random salt.
3. The password and salt are combined.
4. The combined value is hashed.
5. The hash and salt are stored in the database.

When the user logs in:

1. The entered password is combined with the stored salt.
2. A new hash is generated.
3. The new hash is compared with the stored hash.
4. If both hashes match, authentication succeeds.

---

# 🌍 Real-World Example

Suppose two users choose the same password:

```
Password123
```

Without salting:

```
User A → Same Hash
User B → Same Hash
```

With salting:

```
User A + Salt A → Different Hash
User B + Salt B → Different Hash
```

Even though the passwords are identical, the stored hashes are different because each user has a unique salt.

---

# 💡 Key Points

- Passwords should never be stored in plain text.
- Hashing protects passwords by converting them into fixed-length values.
- Salting adds randomness before hashing.
- Salting makes password attacks more difficult.
- Modern applications use secure password hashing algorithms.

---

# 📌 Summary

Password hashing and salting are fundamental techniques used to secure user authentication. Hashing protects passwords by storing only their hash values, while salting adds randomness to improve security and defend against common password attacks.

---

# ❓ Quick Review

1. What is password hashing?
2. What is a salt?
3. Why is salting important?
4. Why should passwords never be stored in plain text?
5. How does salting protect against password attacks?
