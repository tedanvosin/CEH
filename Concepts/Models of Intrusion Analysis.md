# Models of Intrusion Analysis
**Models of Intrusion Analysis** are structured methodologies used to detect, analyze, and respond to security breaches.

The various models are:

## Cyber Kill Chain

The **Cyber Kill Chain**, developed by Lockheed Martin, is a sequential model that outlines the stages of a cyber attack. It is used to break down the attack process and identify potential points of interruption.

### Stages of the Cyber Kill Chain

- **Reconnaissance:**  
  Gathering information about the target, such as network details, employee information, and technology used.
- **Weaponization:**  
  Crafting a payload or exploit based on the gathered intelligence.
- **Delivery:**  
  Transmitting the malicious payload to the target via email, websites, or other delivery vectors.
- **Exploitation:**  
  Triggering the payload to exploit a vulnerability in the target system.
- **Installation:**  
  Installing malware or backdoors on the compromised system to maintain persistence.
- **Command and Control (C2):**  
  Establishing a covert channel to remotely control the compromised system.
- **Actions on Objectives:**  
  Executing the final stage of the attack, such as data exfiltration, system disruption, or further lateral movement.

### Application

By understanding each phase, defenders can implement countermeasures at various stages to disrupt the attacker’s progression, making it a powerful tool for both prevention and incident response.

---

## Diamond Model of Intrusion Analysis

The **Diamond Model** offers an analytical approach that centers on four core features, allowing for a relational view of an intrusion event.

### Core Elements

- **Adversary:**  
  The individual or group responsible for the attack. This node helps in understanding motives, capabilities, and historical behavior.
- **Capability:**  
  The tools, techniques, and procedures (TTPs) employed by the adversary. This element explains what the attacker can do.
- **Infrastructure:**  
  The hardware and software assets used in the attack, such as command and control servers, exploit kits, or compromised domains.
- **Victim:**  
  The target of the attack. This component is crucial for understanding the impact and context of the intrusion.

### Application

The model emphasizes the relationships between these elements, allowing analysts to correlate events, identify patterns, and link separate intrusion incidents to a common adversary.

---

## MITRE ATT&CK Framework

The **MITRE ATT&CK Framework** is a comprehensive knowledge base of adversary tactics and techniques based on real-world observations.

### Structure

- **Tactics:**  
  The high-level objectives or goals of an adversary (e.g., initial access, execution, persistence, privilege escalation).
- **Techniques:**  
  The specific methods employed to achieve these tactics (e.g., phishing for initial access, use of scheduled tasks for persistence).

### Application

Security professionals can map observed behaviors to the framework, identify gaps in their defenses, and prioritize mitigation strategies. Although it is not a sequential model like the Kill Chain, it provides a detailed taxonomy that enhances understanding of adversary behavior.

---

## Pyramid of Pain

The **Pyramid of Pain** is a conceptual model that categorizes indicators of compromise (IOCs) based on the difficulty for adversaries to change them.

### Levels of the Pyramid

- **Hash Values:**  
  The simplest indicators; easily changed by an attacker with minimal effort.
- **IP Addresses and Domain Names:**  
  Slightly more disruptive to change, yet still relatively easy.
- **Network/Host Artifacts:**  
  More challenging to modify, providing a moderate level of "pain" for attackers.
- **Tools:**  
  The attacker’s custom or widely used tools, which are harder to change without significant effort.
- **Tactics, Techniques, and Procedures (TTPs):**  
  The highest level on the pyramid, representing the adversary’s core operational methods. Changing these would require a complete overhaul of the attacker’s strategy.

### Application

By prioritizing IOCs at the higher end of the pyramid, defenders can focus on elements that impose the most significant burden on an attacker when disrupted, thereby improving long-term defensive efficacy.

---

## Model-Based Intrusion Detection Approaches

These approaches use statistical models and machine learning techniques to define normal behavior and then detect anomalies that might indicate an intrusion.

### Categories of Detection Methods

- **Signature-Based Detection:**  
  Compares incoming data against known signatures of malicious activity. While effective for known threats, it may miss novel or obfuscated attacks.
- **Anomaly-Based Detection:**  
  Establishes a baseline of normal network or system behavior and flags deviations from this baseline. This method can detect unknown threats but may have higher false positives.
- **Hybrid Approaches:**  
  Combine elements of signature-based and anomaly-based methods to enhance detection accuracy and reduce false positives.

### Application

Model-based detection systems help automate the process of intrusion detection and are vital in environments where constant monitoring and rapid response are required. They must be finely tuned to balance sensitivity and specificity.
