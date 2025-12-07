---
layout: with_mermaid
title: "Cyber security landscape"
author: "Stratoclo"
mermaid: true
---


Modern hybrid estates expose dozens of seams where attackers can jump from anonymous infrastructure into crown-jewel workloads. The mermaid flow below captures the same whiteboard sequence—phishing to workstation, browser-token hijack, remote-access abuse, and deep-network pivoting—without relying on inline SVG artwork.

<div class="mermaid">
flowchart LR
  subgraph External["External attack surface"]
    APT["APT operator"]
    PH["Phishing email"]
    EP["Employee endpoint"]
  end

  subgraph Edge["Remote access edge"]
    TH["Transport hijack"]
    VPN["VPN / ZTNA gateway"]
  end

  subgraph Core["Corporate network core"]
    FW["Firewall / IDS"]
    WEB["Web & app tier"]
    ID["Identity & AD / SSO"]
    DB["Data lake / DB"]
  end

  APT --> PH --> EP --> TH --> VPN --> FW --> WEB --> ID --> DB
</div>

## Attack flow explained
1. **Campaign staging** - An APT operator automates browser-based phishing kits and spoofed infrastructure to deliver credible lures.
2. **Initial lure** - Victims interact with weaponized emails that mirror SaaS or HR communications, seeding credentials into attacker forms.
3. **Endpoint compromise** - Mac or Windows laptops run malicious extensions, payloads, or remote scripts that watch browser traffic.
4. **Transport hijack** - With cookies or OAuth tokens in hand, the attacker replays sessions or injects requests that inherit the victim identity.
5. **Remote access abuse** - The stolen session satisfies VPN or ZTNA policy, placing the adversary behind perimeter controls with analyst-grade visibility.
6. **East-west pivot** - Once inside, the attacker fans through app tiers, calling internal APIs, scraping logs, and harvesting identity systems for privilege.
7. **Data access** - The end game is database dumps or data-lake exports that can be monetized, extorted, or used for supply-chain attacks.

## Defensive imperatives
- **Tighten email and browser isolation**: Security keys, phishing-resistant MFA, and remote browser isolation blunt the first hop.
- **Continuously attest endpoints**: Device compliance, EDR, and posture-based policy keep hijacked laptops from meeting access rules.
- **Shorten token lifetimes**: Enforce proof-of-possession tokens and rapid refresh cycles to spoil replay attempts.
- **Observe VPN-to-app transitions**: Tag risky sessions at the gateway and require step-up approvals before they can reach AD or data tiers.
- **Segment data planes**: Treat identity stores and databases as separate blast domains with explicit, monitored access paths.

The landscape is messy, but visualizing each hop helps map detections, controls, and playbooks back to the exact places the attacker must touch.
