# GHOST PORTS | Security Engineering Through a Production-Design Lens

**Founder | Security & Infrastructure Engineer | ISC2 C|C · EC-Council E|HE · CompTIA Security+ (In Progress) | Former Art Department Lead (Film & TV)**

---

## The Throughline

For close to a decade, I was building two things at once. By day, in the Toronto and Vancouver film & TV industry (*Fire Country*, *DC's Legends of Tomorrow*, and others), I built physical environments convincing enough that no one watching could separate the real from the staged. In parallel, off set, I was doing the same restless work on my own systems — standing up networks, breaking them, rebuilding them, tearing down what didn't work and starting again. Ghost Ports isn't a pivot away from one discipline into another; it's the formalization of a track that was already running the whole time, now with the production-design instinct and the systems instinct fused into one practice.

---

## The Methodology: Wave Function Collapse

In quantum mechanics, a particle exists in superposition — every possible state at once — until it's observed. The act of measurement is what collapses that superposition into one definite outcome. Ghost Ports applies this as a design principle, not a literal mechanism: the infrastructure an attacker is probing is never the thing they think they're observing. Cross a defined threshold of recon, probing, or brute-force activity, and what's being watched collapses into a decoy state — the attacker's "measurement" resolves to a convincing fake, not the real system.

The connection to production design is deliberate, not incidental: the same design logic that makes a set believable is what makes a decoy convincing enough to gather real threat intelligence, because an attacker can't tell they've been redirected. Unlike infrastructure built to disappear or leave no trace, everything in this framework is built to **preserve full visibility and telemetry** on the real side — deception is the tool, not an excuse to go dark. A system you can't see is a system you can't defend; the goal is misleading the attacker while watching every move they make.

---

## Background

Decade+ in Toronto/Vancouver film & television production — set build-out, equipment logistics, and team coordination in high-pressure, fixed-deadline environments — run concurrently with a decade of hands-on systems work: building, breaking, and rebuilding networks and infrastructure on my own time. Honours Certificate in American Sign Language & Deaf Studies (George Brown College). Reaching fluency in a signed language means tracking grammar that lives in physical space — classifiers, spatial verb agreement, and multiple referents held and manipulated simultaneously in three-dimensional signing space. That's sustained, demanding practice at holding spatial and relational structures in your head, and it carries directly into visualizing network topology, multi-node architecture, and traffic flow. Applied through Hands United, volunteer technical tutoring for the Deaf and Hard of Hearing community. ISC2 Certified in Cybersecurity; EC-Council Ethical Hacking Essentials; currently studying toward CompTIA Security+.

---

## What I Build

### Security & Detection Engineering
- Operate a centralized Wazuh SIEM manager on a dedicated host, separate from the application servers it monitors, correlating logs across multiple production services — including root-causing a rule-matching defect that was silently preventing custom detections from firing.
- Configured real-time alerting from the SIEM into a dedicated incident channel, for immediate visibility into high-severity detections outside the console.
- Authored a formal incident response playbook codifying severity tiers mapped to SIEM rule levels, triage procedures, containment actions, and client notification SLAs.
- Built and operate an automated, API-driven threat-response pipeline using **CrowdSec**'s community threat-intelligence feed integrated with a **Cloudflare Workers**-based bouncer, operationalizing real-time IP-based enforcement at the edge without manual intervention.
- Fixed real-IP attribution gaps across a multi-service **Docker Compose** deployment so SIEM correlation reflects actual client IPs rather than internal proxy addresses.

### The Construct
Game Design & Principal Engineer on The Construct ([range.ghostports.com](https://range.ghostports.com), currently in open beta), a real-time, browser-based cyber-range platform spanning multiple simulation tracks — Linux, Windows forensics, and cloud/AWS investigation among them. CMD+CTRL, its flagship simulation, has players issue live commands against a simulated environment to work through a multi-node investigation, with a second detection-engine side watching how they play. Designed the platform's intrusion-detection system, modeling how a production SOC correlates multiple signal types — signature-based, volume/anomaly-based, and behavioral — into a single alerting pipeline, along with an anti-cheat and progression system so results can't be shared or faked, and tiered difficulty that deepens on the same content without a rebuild. Live sessions run through a Game Master console — a single screen controlling a full class or cohort in real time: instant roster provisioning, a moderated class-wide chat channel, and fully refereed Red vs. Blue Versus matches with real incident-response tradeoffs built into the available responses. 17 labs live as of this writing, including a complete SOC Analyst track, with new content added weekly.

### In Development: Wave Function Collapse — Deception-Based Early-Warning Tier
Building the methodology into a sub-ban tier that redirects suspicious-but-not-yet-banned traffic to a decoy backend, gathering pure-signal threat intel while leaving existing hard-ban enforcement and full logging untouched. Currently in design; not yet deployed.

### Current Client Engagements
- **M.K. Bureautique** — ongoing SOC-style security monitoring.
- Prior contract work in IT support and Windows systems hardening (By The Blade; Apex Contracting).

---

## Stack

| Domain | Technologies |
| :--- | :--- |
| **Detection & SIEM** | Wazuh |
| **Threat Intel & Edge Enforcement** | CrowdSec, Cloudflare Workers, Cloudflare KV |
| **Networking** | WireGuard, Nginx (reverse proxy, real-IP correlation) |
| **Automation & Scripting** | Python, PowerShell, Bash |
| **Platforms** | Docker, Docker Compose, systemd, Linux |

---

*© 2026 Ghost Ports*
