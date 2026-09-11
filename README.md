# Academic Publications & Technical Reports

A collection of selected academic work, research papers, technical reports, and project documentation focused on **information retrieval**, **cybersecurity**, **container security**, and **software systems**.

## Contents

| Document | Type | Area | Summary |
| --- | --- | --- | --- |
| [RETRIX at CheckThat! 2026: Source Retrieval for Scientific Web Claims](./Clef26-RETRIX-5thPosition.pdf) | CLEF 2026 working paper | Information Retrieval / NLP | A multilingual scientific-source retrieval pipeline combining translation, query expansion, hybrid dense/sparse retrieval, ColBERT-style scoring, and neural reranking. The RETRIX system finished **5th** in the CheckThat! 2026 Task 1 ranking. |
| [Security Assessment and Attack Techniques in RFID Payment Technologies](./Padoan_Giancarlo_Bachelor_Thesis.pdf) | Bachelor's thesis | Cybersecurity / RFID | Practical security assessment of MIFARE Classic 1K payment technology using Proxmark3, including cloning, replay, and double-spending attacks and analysis of CRYPTO1 weaknesses. |
| [Hardening a Containerized Infrastructure on Proxmox: Docker Runtime Security with AppArmor and SELinux](./Hardening_a_Containerized_Infrastructure_on_Proxmox__Docker_Runtime_Security_with_AppArmor_and_SELinux%20%289%29.pdf) | Technical report | Container / Infrastructure Security | A security-focused study of hardening containerized workloads on Proxmox, with emphasis on Docker runtime controls and Linux Mandatory Access Control through AppArmor and SELinux. |
| [Software Platforms Project Documentation](./SOFTPLAT_DOCS%20%286%29.pdf) | Project documentation | Software Platforms | Documentation for a software-platform project involving containerized services, data ingestion, search/retrieval, and model-backed processing. |

## Featured Work

### RETRIX at CheckThat! 2026

**RETRIX at CheckThat! 2026: Source Retrieval for Scientific Web Claims**  
Fabio Baldan, Davide Donati, Alvise Garberino, **Giancarlo Padoan**, Marco Tessari, Nicola Ferro  
University of Padua — CLEF 2026 Working Notes

The paper addresses the problem of finding the scientific publication implicitly referenced by a short social-media claim. The system uses a multi-stage retrieval pipeline:

1. Translate French and German queries into English.
2. Expand queries using embedding-based pseudo-relevance feedback.
3. Retrieve candidates with **BGE-M3**, combining dense retrieval, sparse lexical matching, and ColBERT-style multi-vector scoring.
4. Rerank candidates with a fine-tuned **NVIDIA Llama Nemotron reranker**.

Reported aggregate test performance includes **0.7126 MRR@5** and **0.9240 Recall@100**. The team reports a **5th-place** finish in the task ranking.

[Read the paper](./Clef26-RETRIX-5thPosition.pdf)

---

### Security Assessment and Attack Techniques in RFID Payment Technologies

Bachelor's thesis, University of Padua, 2024/2025.

The thesis examines practical weaknesses in legacy RFID payment systems, focusing on **MIFARE Classic 1K**. Using a **Proxmark3**, it demonstrates a complete cloning workflow and evaluates attacks including replay and double spending. The work also discusses weaknesses in the proprietary **CRYPTO1** cipher and potential countermeasures for RFID-based payment deployments.

Official University of Padua record:  
https://hdl.handle.net/20.500.12608/89365

[Read the thesis](./Padoan_Giancarlo_Bachelor_Thesis.pdf)

## Topics

`Information Retrieval` · `NLP` · `Fact Checking` · `Cybersecurity` · `RFID Security` · `Docker` · `Proxmox` · `AppArmor` · `SELinux` · `Software Platforms`

## Repository Structure

```text
.
├── Clef26-RETRIX-5thPosition.pdf
├── Hardening_a_Containerized_Infrastructure_on_Proxmox__Docker_Runtime_Security_with_AppArmor_and_SELinux (9).pdf
├── Padoan_Giancarlo_Bachelor_Thesis.pdf
├── SOFTPLAT_DOCS (6).pdf
├── LICENSE
└── README.md
```

## License

This repository contains an MIT `LICENSE`, but individual academic documents may be subject to their own publication, institutional, or author-specific licensing terms.

In particular, the CLEF 2026 working paper is published under **CC BY 4.0** in the CLEF proceedings. For reuse or redistribution of any PDF, check the licensing information contained in the document or its official publication record.

## Author / Maintainer

GitHub: [@esspadoo](https://github.com/esspadoo)
