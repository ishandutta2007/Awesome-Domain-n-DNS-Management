# Awesome-Domain-n-DNS-Management

# Top Domain & DNS Management Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Authoritative DNS, Zone Automation & DNS-as-Code Workflows*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Domain & DNS Management**. These tools manage authoritative DNS zones, record automation, DNSSEC signing, and multi-provider DNS orchestration for enterprises, agencies, and developers.

**Examples** include Cloudflare DNS, DNS Made Easy, NS1, Amazon Route 53, Google Cloud DNS, Azure DNS, EasyDNS, ClouDNS, Dyn Managed DNS, and UltraDNS (the category leaders).

**Open-source emphasis**: This section is expanded with active projects for self-hosting, multi-provider DNS automation, and transparent zone management — ideal for infrastructure teams, developers, and organizations building vendor-independent DNS workflows. The open-source ecosystem is anchored by **DNSControl** (multi-provider DNS-as-code) and **Technitium DNS Server** (recursive + authoritative with web UI), with strong coverage in IPAM-integrated DDI platforms.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Cloudflare DNS](https://www.cloudflare.com/dns/)**  
  The most widely used managed DNS service, offering free and enterprise tiers with anycast network, DNSSEC, and integrated DDoS protection. API-first design makes it a popular target for DNS-as-code automation tools .

- **[DNS Made Easy](https://dnsmadeeasy.com/)**  
  Enterprise-grade managed DNS with 100% uptime SLA, global anycast network, and advanced monitoring. Offers DNS Failover and granular record management .

- **[NS1](https://ns1.com/)**  
  Modern DNS platform with intelligent traffic management, real-time analytics, and API-first architecture. Popular for high-scale, latency-sensitive applications.

- **[Amazon Route 53](https://aws.amazon.com/route53/)**  
  AWS's highly available and scalable DNS web service with domain registration, health checks, and traffic flow policies. Deep integration with AWS services .

- **[Google Cloud DNS](https://cloud.google.com/dns)**  
  Google's managed DNS service running on the same infrastructure as Google's own DNS, with global anycast and 100% uptime SLA.

- **[Azure DNS](https://azure.microsoft.com/en-us/services/dns/)**  
  Microsoft Azure's DNS hosting service for public and private zones, with role-based access control and Azure resource integration.

- **[EasyDNS](https://easydns.com/)**  
  Managed DNS provider offering domain registration, DNS hosting, and dynamic DNS with a focus on reliability and customer support.

- **[ClouDNS](https://www.cloudns.net/)**  
  Managed DNS and DDNS provider with anycast network, DNSSEC, and flexible pricing across multiple global locations.

- **[Dyn Managed DNS](https://dyn.com/)**  
  Enterprise DNS service (now part of Oracle Cloud) with global anycast, traffic management, and advanced failover capabilities.

- **[UltraDNS](https://www.ultradns.com/)**  
  Enterprise-grade DNS platform (now part of Vercara) with 100% uptime SLA, DNSSEC, and advanced security features for large organizations.

## Open-Source GitHub Projects

- **[DNSControl](https://github.com/StackExchange/dnscontrol)**  
  The most mature open-source multi-provider DNS-as-code tool, used by Stack Overflow to manage hundreds of domains across multiple registrars and providers. A domain-specific language (DSL) describes DNS zones and pushes them to 50+ supported providers including Cloudflare, Route 53, Azure DNS, Google DNS, NS1, DNS Made Easy, and PowerDNS. Supports preview/apply workflow, CI/CD integration, and multi-provider redundancy. Runs on any platform Go supports. **This is the de-facto standard for GitOps-driven DNS management** .

- **[Technitium DNS Server](https://github.com/TechnitiumSoftware/DnsServer)**  
  Self-hosted DNS server with web console, working as both authoritative and recursive resolver. Features block lists for ad/malware blocking, DNS-over-TLS/HTTPS/QUIC support, DNSSEC validation, persistent caching, clustering, and SSO with OpenID Connect. Serves over 100,000 requests per second on commodity hardware. Docker image available. **The most feature-complete self-hosted DNS server for privacy-conscious organizations** .

- **[deSEC](https://github.com/desec-io)**  
  Free secure DNS hosting service with an open-source backbone (desec-stack). Provides authoritative DNS with DNSSEC, REST API, and automation tools. The stack is MIT-licensed and available for self-hosting. Includes certbot integration for Let's Encrypt certificates. **A production-grade open-source DNS hosting platform** .

- **[dnsctl](https://github.com/dhivijit/dnsctl)**  
  Secure, version-controlled DNS management tool for Cloudflare with CLI and GUI. Brings Git-backed state, drift detection, and plan/apply workflow to DNS record management. Features AES-256-GCM encrypted token storage, session locking, multi-account support, and protected records requiring explicit override. **Ideal for teams wanting GitOps for Cloudflare DNS specifically** .

- **[NicTool](https://github.com/nictool)**  
  Open-source DNS management system with a Node.js server, web configurator, and nameserver supervisor. Supports multiple DNS engines (BIND, Knot, NSD, PowerDNS, TinyDNS, MaraDNS) with export engines and DNSSEC signing. MySQL or file-based TOML storage. **A full DNS management suite for organizations running their own nameservers** .

- **[Bind9 Web Manager](https://github.com/bugfishtm/Bind9-Web-Manager)**  
  Web-based management interface for BIND9 DNS servers. Simplifies zone management, replication, and user administration with a GUI. Installation via manual, Docker, or automated script. **Brings modern web UI to legacy BIND9 deployments** .

- **[MoeDNS](https://github.com/phoenixlzx/moedns)**  
  DNS management app using Node.js and MongoDB, designed for use with PowerDNS/MySQL or MiniMoeDNS/MySQL. 87+ stars on GitHub. **A lightweight web UI for PowerDNS backends** .

- **[routedns](https://github.com/folbricht/routedns)**  
  Configurable DNS proxy and router written in Go. Supports DNS-over-TLS, DNS-over-HTTPS, DNS-over-QUIC, and Oblivious DoH. Features DNSSEC validation, query logging, blocklists, client blocklists, DNS64, and advanced routing based on query name/type. **A powerful self-hosted DNS forwarding and filtering solution** .

### Additional Strong Open-Source Options

- **SpatiumDDI** — Open-source DDI platform unifying DNS, DHCP, and IPAM. Runs its own BIND9/PowerDNS/Kea service containers with FastAPI control plane and React UI. Features RBAC, LDAP/OIDC/SAML auth, TOTP MFA, and scoped API tokens for Terraform credentials .
- **NSoT** — Network Source of Truth (IPAM) from Dropbox, now API-first with Django 5.2 and Python 3.10+ support. Tracks IP addresses, network devices, and interfaces via REST API .
- **teemIP** — Open-source web-based IPAM and DDI solution built on iTop framework. Features IPv4/IPv6 management, subnet hierarchy, DNS/DHCP integration, VLAN management, and capacity planning .
- **Rackd** — Lightweight IPAM and device inventory in Go with SQLite. Features DNS management with Cloudflare/Route53/PowerDNS sync, RBAC, audit trail, and MCP server for AI/automation .
- **jt-ipam** — Self-hosted, integration-focused IPAM with deep DNS server integration (BIND, PowerDNS, Windows DNS), LibreNMS, OPNsense, and Proxmox VE. Python/FastAPI/Vue stack with local LLM support .
- **phpIPAM** — Mature open-source IP address management with DNS integration, section/subnet hierarchy, and API. Widely deployed for network infrastructure management .
- **NetBox** — Premier source of truth for network automation with IPAM, DCIM, and DNS management. Apache 2.0 licensed with large community .

**Frameworks for building custom DNS management solutions**: Combine **DNSControl** for multi-provider DNS-as-code with GitOps workflows . Use **Technitium DNS Server** for self-hosted authoritative and recursive DNS with web UI and block lists . Deploy **deSEC** for a full open-source DNS hosting stack with DNSSEC . For Cloudflare-specific GitOps, **dnsctl** provides plan/apply with drift detection . Integrate **SpatiumDDI** or **teemIP** for unified DNS+DHCP+IPAM management . Note that true enterprise managed DNS with global anycast, 100% uptime SLA, and advanced traffic management remains primarily commercial territory; open-source stacks provide strong self-hosted authoritative DNS, multi-provider automation, and DDI foundations.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- DNS management tools must comply with ICANN policies, registry requirements, and applicable laws regarding domain registration and DNS operations.
- Self-hosted open-source solutions require proper infrastructure, DNSSEC key management, and ongoing maintenance. DNS is a critical service — high availability and disaster recovery planning are essential.
- The open-source ecosystem provides strong self-hosted DNS servers, multi-provider automation, and DDI platforms, but global anycast networks with 100% uptime SLAs remain primarily a commercial offering.

---

**Made for network engineers, DevOps teams, infrastructure architects, and domain administrators.**  
Let's make DNS management more open, transparent, and automated.
