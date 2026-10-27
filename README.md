# Safety in the Smart Home

**How insecure IoT devices turn digital exploits into physical risk, and a multi-layered defense model to stop it.**

📄 [Read the paper (Markdown)](paper.md) · [PDF](safety-in-the-smart-home.pdf)

## The problem

Smart locks, cameras, thermostats and voice assistants are now part of a home's critical infrastructure, but most were shipped with convenience ahead of security. In a traditional IT breach, the loss is data. In a smart-home breach, an unpatched lock firmware or exposed service port can become a physical entry point or an environmental hazard for the people living there.

## What this research covers

| Area | Questions examined |
|---|---|
| **Physical safety risk** | How smart-lock, camera and environmental-control weaknesses translate into occupant harm |
| **Device-level defenses** | Hardware root of trust, secure boot, cryptographically verified firmware updates, lightweight cryptography for constrained devices, patchable (FPGA-based) hardware |
| **Network-level defenses** | IoT intrusion detection using feature selection (PCA + Pearson correlation) feeding CNN classifiers; entropy-based multi-layer network security scoring |
| **Human factor** | Social engineering, MFA adoption, network segmentation and the convenience-security tradeoff that drives consumer behavior |

## Key findings

- **Security has to start at the silicon.** A hardware root of trust and verified firmware updates keep a device's integrity intact even after a network-level compromise.
- **Network monitoring is viable on home hardware.** Published PCA/PCC + CNN intrusion-detection models report >99% binary classification accuracy on the Edge-IIoTset benchmark while cutting training and inference time, which matters for resource-constrained residential networks.
- **Technical controls fail without the user.** Encryption and secure boot are undermined by weak credentials and flat networks; user education, MFA and segmentation form the last layer.
- **Proposed model:** a defense-in-depth architecture that links hardware integrity, network detection and user behavior, with concrete implications for manufacturers and consumers.

## Method

A structured literature review and synthesis of peer-reviewed research, ethical-hacking case studies (e.g., comparative analysis of smart-lock encryption implementations) and published intrusion-detection results. All figures cited in the paper are attributed to their original authors.

## Author

**Devante Metoyer** · [LinkedIn](https://linkedin.com/in/devantedmetoyer) · [GitHub](https://github.com/DDMetoyer)

## License

Text © Devante Metoyer, licensed under [CC BY 4.0](LICENSE).
