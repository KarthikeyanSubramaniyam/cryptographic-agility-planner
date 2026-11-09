# Cryptographic Agility & Post-Quantum Migration Planner

<p align="center">
  <img src="https://img.shields.io/badge/Security-Defensive_Auditor-blue?style=flat" alt="Type">
  <img src="https://img.shields.io/badge/Status-Architectural_Showcase-success?style=flat" alt="Status">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
</p>

> 🔒 **Technical Showcase & Architecture Specification**  
> *This repository provides public architectural documentation, system specifications, and implementation summaries. Full production source code, internal test suites, and proprietary algorithms are maintained in a secure private repository.*

---

## 📌 Executive Summary

**Category**: Cryptography & Quantum Readiness  
**Tech Stack**: `Python 3.10+ · Cryptographic Architecture · NIST PQC Standards · Security Planning`  

Cryptographic inventory and readiness planner evaluating enterprise cipher suites, certificates, and algorithms for quantum-resistant migration.

---

## 🎯 The Problem It Solves

The advent of quantum computing threatens classical asymmetric encryption (RSA, ECC). Organizations must inventory algorithms now to achieve cryptographic agility and plan post-quantum migrations.

---

## ⚙️ How the Engine Works

1. **Algorithm Inventory Compilation**: Scans configuration files, TLS configurations, and codebases to compile an inventory of all active cryptographic algorithms.
2. **Vulnerability & Deprecation Classification**: Categorizes ciphers into DEPRECATED (DES, 3DES, MD5, SHA-1), LEGACY (RSA-1024, Diffie-Hellman < 2048), STANDARD (AES-256, RSA-3072, ECC), and POST-QUANTUM.
3. **Quantum Vulnerability Assessment**: Evaluates vulnerability to Shor's algorithm (breaking public-key cryptography) and Grover's algorithm (halving symmetric key security).
4. **Migration Path Synthesis**: Generates prioritized replacement recommendations mapping legacy algorithms to NIST-standardized Post-Quantum algorithms (ML-KEM, ML-DSA).
5. **Roadmap Output**: Emits phased migration roadmaps with risk scores and implementation timelines.

---

## 🚀 Key Capabilities

- Automated discovery of deprecated and quantum-vulnerable ciphers
- NIST Post-Quantum Cryptography (PQC) readiness scoring
- Prioritized migration path generation for certificates and encryption algorithms
- Cryptographic bill of materials (CBOM) generation

---

## 🏗️ System Data Flow & Architecture

```
+-----------------------------------+
|  Target Input / Configuration    |
|  (JSON Snapshots / Policies)      |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  1. Schema Normalization Engine   |
|  Validates types & formats        |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  2. Core Analytical Pipeline      |
|  Heuristic rule evaluation,       |
|  invariant checks & drift diffs   |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  3. Risk Classification           |
|  Assigns severity: INFO / HIGH    |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  4. Structured Findings & Report  |
|  Root cause, evidence &           |
|  actionable remediation steps     |
+-----------------------------------+
```

---

## 📄 Findings Output Structure

The engine generates structured, machine-parsable JSON reports adhering to this standard audit schema:

```json
{
  "results": [
    {
      "resource": "resource-identifier",
      "severity": "HIGH",
      "check": "CHECK_IDENTIFIER",
      "detail": "Descriptive analysis of the identified security posture issue.",
      "remediation": "Actionable step-by-step guidance to restore compliant state.",
      "evidence": {
        "observed_field": "value",
        "required_policy": "enforced_policy"
      }
    }
  ],
  "count": 1,
  "scope": "Comprehensive defensive security audit"
}
```

---

## 🔒 Source Code & Enterprise Inquiries

To protect proprietary intellectual property and client operational security:
* **Public Repository**: Contains comprehensive architecture specifications, schemas, and design overviews.
* **Private Repository**: Contains the complete production implementation, continuous integration pipelines, and full regression test suites.

For architectural questions or enterprise inquiries, connect via [LinkedIn](https://www.linkedin.com/in/karthikeyansubramaniam04/) or visit the [Portfolio Site](https://karthikeyansubramaniyam.github.io).
