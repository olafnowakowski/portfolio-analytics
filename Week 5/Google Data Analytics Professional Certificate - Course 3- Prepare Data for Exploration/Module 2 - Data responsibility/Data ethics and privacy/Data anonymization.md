# Data Anonymization

## Main Idea

**Data anonymization** is the process of protecting people’s private or sensitive data by removing or hiding information that could identify them.

It is an important part of data privacy and responsible data use.

---

# What Is Personally Identifiable Information?

## Definition

**Personally identifiable information**, or **PII**, is information that can be used by itself or with other data to identify a person.

---

## Simple Explanation

PII is any information that could help someone figure out who a person is.

---

## Examples of PII

PII can include:

- names
- telephone numbers
- email addresses
- social security numbers
- account numbers
- IP addresses
- license plate numbers
- license numbers
- medical records
- photographs

---

# What Is Data Anonymization?

## Definition

**Data anonymization** is the process of protecting people’s private or sensitive data by eliminating or hiding personally identifiable information.

---

# Why Data Anonymization Matters

Data anonymization helps protect people’s privacy.

It prevents sensitive information from being used to identify, track, or harm individuals.

### Important Lesson

Data anonymization helps keep data private and secure.

---

# How Data Anonymization Works

Data anonymization usually involves methods such as:

- blanking
- hashing
- masking
- using fixed-length codes
- replacing data with altered values

---

# 1. Blanking

## Definition

**Blanking** removes sensitive information by leaving the data field empty.

### Example

A phone number field might be replaced with a blank value.

---

# 2. Hashing

## Definition

**Hashing** converts data into a fixed-length code.

The original data is hidden and replaced with a coded version.

### Example

A customer ID or email address might be changed into a long code that does not reveal the original value.

---

# 3. Masking

## Definition

**Masking** hides part of the data while leaving some of it visible.

### Example

A credit card number may appear as:

**** **** **** 1234

The full number is hidden, but the last four digits remain visible.

---

# 4. Fixed-Length Codes

Fixed-length codes can be used to represent data columns without showing the actual personal information.

### Example

Instead of showing a person’s name, a dataset might show:

USER0001

---

# 5. Altered Values

Data can also be hidden by replacing real values with changed values.

### Example

A real birthdate may be replaced with a general age range.

---

# Your Role in Data Anonymization

Organizations are responsible for protecting their data and any personal information inside it.

As a Data Analyst, you may need to understand:

- what data should be anonymized
- why certain data is sensitive
- how anonymized data protects privacy
- when anonymization may be required

---

# Are Data Analysts Usually Responsible for Anonymization?

Usually, junior Data Analysts are not responsible for performing data anonymization themselves.

However, they should understand the basics.

---

# When a Data Analyst Might Need to Anonymize Data

A Data Analyst might need to anonymize data when working with a copy of data for:

- testing
- development
- practice
- system checks
- training environments

In these cases, the analyst may need to anonymize the data before working with it.

---

# What Types of Data Should Be Anonymized?

Sensitive and personally identifiable data should be anonymized.

This is especially important in industries like:

- healthcare
- finance

---

# Healthcare Data

Healthcare data is highly sensitive because it may include private medical information.

Examples:

- medical records
- patient names
- diagnosis information
- treatment history
- insurance information

---

# Financial Data

Financial data is highly sensitive because it may include private money-related information.

Examples:

- account numbers
- credit card information
- loan records
- financial transactions
- social security numbers

---

# De-Identification

## Definition

**De-identification** is the process of removing all personally identifying information from data.

---

# Why De-Identification Is Important

Healthcare and financial industries often use de-identification because the risks are high.

If this data is exposed, it can harm people’s:

- privacy
- safety
- finances
- identity security
- trust in organizations

---

# Data Often Anonymized

The following types of data are often anonymized:

- telephone numbers
- names
- license plates
- license numbers
- social security numbers
- IP addresses
- medical records
- email addresses
- photographs
- account numbers

---

# Why Specificity Matters

Some people naturally understand that sensitive data should be anonymized.

Others may need clear rules about what counts as sensitive information.

That is why organizations must be specific about what data needs protection.

---

# Why Anonymization Protects Safety

Imagine a world where everyone had access to each other’s:

- addresses
- account numbers
- medical records
- phone numbers
- photographs
- identifying information

This would invade privacy and make people less safe.

### Important Lesson

Data anonymization protects both privacy and safety.

---

# Data Anonymization in Every Industry

Data anonymization is used in many industries, not just healthcare and finance.

It may be used anywhere personal or sensitive data is collected.

Examples:

- education
- retail
- government
- technology
- insurance
- marketing
- transportation

---

# Data Anonymization and Data Privacy

Data anonymization supports data privacy by reducing the risk that individuals can be identified.

It helps organizations use data while still protecting the people behind the data.

---

# Summary Table

| Term | Meaning |
|---|---|
| **PII** | Information that can identify a person by itself or with other data |
| **Data anonymization** | Process of removing or hiding private identifying information |
| **Blanking** | Removing sensitive information by leaving fields empty |
| **Hashing** | Converting data into a fixed-length code |
| **Masking** | Hiding part of the data |
| **De-identification** | Removing all personally identifying information from data |

---

# Big Lesson

Data anonymization protects people by removing or hiding information that could identify them.

It allows organizations to use data while reducing privacy and security risks.

---

# Key Takeaways

- Personally identifiable information is information that can identify a person.
- PII can identify someone by itself or when combined with other data.
- Data anonymization protects private or sensitive data.
- Anonymization can involve blanking, hashing, masking, fixed-length codes, or altered values.
- Organizations are responsible for protecting personal information in their data.
- Data Analysts should understand what data needs to be anonymized.
- Junior Data Analysts usually do not perform anonymization themselves.
- Analysts may need to anonymize copied data used for testing or development.
- Healthcare and financial data are especially sensitive.
- De-identification removes personally identifying information from data.
- Names, phone numbers, email addresses, social security numbers, medical records, photographs, IP addresses, and account numbers are often anonymized.
- Data anonymization helps keep data private and secure.

---

# Extra Important Notes

- Data anonymization is part of responsible data use.
- The goal is to protect people, not just protect datasets.
- Sensitive data should be handled carefully even if it seems harmless.
- Data can sometimes identify a person when combined with other information.
- Anonymization helps reduce the risk of privacy violations.
- Healthcare and finance have high stakes because their data can deeply affect people’s lives.
- Analysts should always be aware of privacy risks when working with personal data.

---

# Final Summary

Data anonymization is the process of protecting people’s private or sensitive data by removing or hiding personally identifiable information. Personally identifiable information, or PII, is information that can identify a person on its own or when combined with other data. Common anonymization methods include blanking, hashing, masking, using fixed-length codes, and replacing real values with altered values. Healthcare and financial data are especially sensitive and often go through de-identification, which removes personally identifying information. Data that is often anonymized includes names, phone numbers, email addresses, social security numbers, medical records, photographs, IP addresses, license numbers, and account numbers. The main lesson is that data anonymization helps protect privacy, improve security, and keep people safe when organizations use data.
