# Data Security, Encryption, Tokenization, and Version Control

## Main Idea

**Data security** means protecting data from unauthorized access or corruption by putting safety measures in place.

Data Analysts need to balance keeping data safe with being able to access and use it for timely analysis.

---

# What Is Data Security?

## Definition

**Data security** means protecting data from unauthorized access or corruption by adopting safety measures.

---

# Why Data Security Matters

Data security helps protect sensitive data from:

- unauthorized access
- unauthorized viewing
- corruption
- misuse
- theft
- accidental damage

---

# The Balance Between Security and Access

Companies must balance two needs:

1. **Protecting data**
2. **Allowing access to data for analysis**

---

# Why This Balance Can Be Difficult

Data Analysts need access to data so they can make meaningful and timely observations.

However, companies also need to keep data secure.

Too much restriction can slow analysis.

Too little restriction can create security risks.

---

# Security Measures

Two important data security measures are:

1. **Encryption**
2. **Tokenization**

---

# Encryption

## Definition

**Encryption** uses a unique algorithm to alter data and make it unusable by users and applications that do not know the algorithm.

---

# Encryption Key

The algorithm used for encryption is saved as a **key**.

The key can be used to reverse the encryption.

---

# How Encryption Works

Encryption changes data into a protected form.

Only users or applications with the correct key can return the data to its original form.

---

# Why Encryption Is Useful

Encryption protects data because unauthorized users cannot use the data without the key.

Even if someone accesses the encrypted data, they cannot understand it without the key.

---

# Tokenization

## Definition

**Tokenization** replaces protected data elements with randomly generated data called a **token**.

---

# How Tokenization Works

Tokenization replaces sensitive data with tokens.

The original data is stored in a separate location.

The original data is mapped to the tokens.

---

# Accessing Tokenized Data

To access the complete original data, a user or application needs permission to use:

- the tokenized data
- the token mapping

---

# Why Tokenization Is Useful

If tokenized data is hacked, the original data remains safe because it is stored separately.

This makes tokenization useful for protecting sensitive information.

---

# Encryption vs Tokenization

| Security Method | How It Protects Data |
|---|---|
| **Encryption** | Changes data using an algorithm and requires a key to reverse it |
| **Tokenization** | Replaces sensitive data with tokens and stores original data separately |

---

# Other Data Security Options

Encryption and tokenization are only two examples of data security methods.

Other options may include authentication devices and AI-related security technology.

---

# Junior Data Analyst Responsibility

As a junior Data Analyst, you probably will not be responsible for building full data security systems.

Many companies have:

- internal data security teams
- third-party data security providers
- specialized security systems

---

# Why Junior Analysts Still Need to Understand Security

Even if junior analysts do not build security systems, they should understand:

- why data security matters
- what protections may be used
- how to handle data responsibly
- how to balance security with analysis needs

---

# Company Responsibility

All companies have a responsibility to keep their data secure.

This is especially important when data includes sensitive or personal information.

---

# Version Control

## Definition

**Version control** enables collaborators within a file to track changes over time.

---

# What Version Control Tracks

Version control helps users understand:

- who made changes
- what changes were made
- when changes were made
- why changes were made

---

# Why Version Control Matters

Version control helps teams collaborate without losing work.

It prevents confusion and reduces the risk of people overwriting each other’s changes.

---

# Version Control Example

A project team may work together in the same set of files.

Each person may be responsible for a different part of the project.

Without version control, it would be hard to track who changed what and when.

This could lead to confusion or overwritten work.

---

# Benefits of Version Control

Version control helps Data Analysts:

- collaborate effectively
- track file changes
- experiment with new ideas
- avoid losing work
- understand file history
- recover earlier versions
- reduce confusion
- protect project progress

---

# Version Control and Data Security

Version control supports data security by making changes traceable.

It helps teams understand the history of a file and identify accidental or unauthorized changes.

---

# Big Lesson

Data security protects data, while version control helps protect the work being done with that data.

Both are important for responsible and efficient data analysis.

---

# Key Takeaways

- Data security protects data from unauthorized access or corruption.
- Data Analysts must balance data protection with analysis needs.
- Companies need to protect data while still allowing appropriate access.
- Encryption changes data using an algorithm.
- Encrypted data can only be restored with the correct key.
- Tokenization replaces sensitive data with randomly generated tokens.
- Tokenized original data is stored separately from the tokens.
- Tokenization keeps original data safer if the tokenized data is hacked.
- Junior analysts usually do not build data security systems.
- Companies may use internal security teams or third-party security providers.
- Analysts should still understand common security systems.
- Version control tracks changes over time.
- Version control records who changed a file, when, what changed, and why.
- Version control helps teams collaborate without overwriting each other’s work.
- Version control allows analysts to experiment without fear of losing work.

---

# Extra Important Notes

- Secure data is not useful if no authorized person can access it.
- Accessible data is risky if it is not protected.
- Good security balances protection and usability.
- Encryption depends on keeping the key secure.
- Tokenization depends on protecting the token mapping.
- Version control is one practical way analysts can support safe collaboration.
- Version control is especially useful when multiple people work in the same files.

---

# Final Summary

Data security means protecting data from unauthorized access or corruption by using safety measures. Companies must balance data security with the need for analysts to access data for timely analysis. Two common security methods are encryption and tokenization. Encryption changes data using an algorithm and requires a key to restore the original data. Tokenization replaces sensitive data with randomly generated tokens while storing the original data separately. Junior Data Analysts may not build these systems, but they should understand how companies protect data. One important practice analysts can use directly is version control, which tracks who made changes, what changes were made, when they happened, and why. The main lesson is that data security protects data, while version control protects collaborative work and helps prevent confusion, errors, and lost progress.
