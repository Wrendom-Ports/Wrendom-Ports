GHOST PORTS | Security Engineering Through a Production-Design Lens

Founder | Security & Infrastructure Engineer | Former Art Department Lead (Film & TV)
ISC2 C|C · EC-Council E|HE · CompTIA Security+ (In Progress)

The Throughline

I spent close to a decade in the Toronto and Vancouver film & TV industry (Fire Country, DC’s Legends of Tomorrow, and others) building physical environments convincing enough that no one watching could separate the real from the staged. That discipline — construct something “lived-in” enough to be indistinguishable from the genuine article — is the same instinct I now apply to defensive security architecture.

The Methodology: Wave Function Collapse

In quantum mechanics, a particle exists in superposition — every possible state at once — until it’s observed. The act of measurement is what collapses that superposition into one definite outcome. Ghost Ports applies this as a design principle, not a literal mechanism: the infrastructure an attacker is probing is never the thing they think they’re observing. Cross a defined threshold of recon, probing, or brute-force activity, and what’s being watched collapses into a decoy state — the attacker’s “measurement” resolves to a convincing fake, not the real system.

The connection to production design is deliberate, not incidental: the same design logic that makes a set believable is what makes a decoy convincing enough to gather real threat intelligence, because an attacker can’t tell they’ve been redirected. Unlike infrastructure built to disappear or leave no trace, everything in this framework is built to preserve full visibility and telemetry on the real side — deception is the tool, not an excuse to go dark. A system you can’t see is a system you can’t defend; the goal is misleading the attacker while watching every move they make.

Background

Decade+ in Toronto/Vancouver film & television production — set build-out, equipment logistics, and team coordination in high-pressure, fixed-deadline environments.
Honours Certificate in American Sign Language & Deaf Studies (George Brown College); ASL fluency applied through Hands United, volunteer technical tutoring for the Deaf and Hard of Hearing community.
ISC2 Certified in Cybersecurity; EC-Council Ethical Hacking Essentials; currently studying toward CompTIA Security+.

What I Build

Security & Detection Engineering

Deployed and maintain a Wazuh SIEM, including root-causing and fixing a rule-matching defect that was silently preventing custom detections from firing.
Built and operate an automated, API-driven threat-response pipeline using CrowdSec’s community threat-intelligence feed integrated with a Cloudflare Workers-based bouncer, operationalizing real-time IP-based enforcement at the edge without manual intervention.
Fixed real-IP attribution gaps across a multi-service Docker Compose deployment (custom Nginx and gunicorn logging) so SIEM correlation reflects actual client IPs rather than internal proxy addresses.

The Construct — a cybersecurity training platform (PWA) built end-to-end, including its flagship CMD+CTRL simulation for hands-on detection/incident-response practice.

In Development: Wave Function Collapse — Deception-Based Early-Warning Tier — currently building the Wave Function Collapse methodology into a sub-ban tier that redirects suspicious-but-not-yet-banned traffic to a decoy backend, gathering pure-signal threat intel while leaving existing hard-ban enforcement and full logging untouched. Explicitly marked not yet deployed.

Current Client Engagements — M.K. Bureautique (website build + ongoing SOC-style monitoring); prior IT support/hardening work (By The Blade, Apex Contracting).

Stack: Wazuh · CrowdSec · Cloudflare Workers/KV · WireGuard · Nginx · Python/PowerShell/Bash · Docker Compose · systemd · Linux
