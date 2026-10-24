# azure landing zone
A production style Azure Landing Zone built with Terraform, management group hierarchy, platform and workload subscriptions, and policy-driven guardrails for governance, security, and networking at scale.

## Overview 
This project demonstrates an enterprise-grade Azure foundation following Microsoft’s Cloud Adoption Framework principles. It separates platform services, connectivity, identity, management, from workload landing zones — corp and online — with Azure Policy enforcing guardrails across the hierarchy.

## Architecture 
 - Management Groups: Tenant Root to Org to Platform, which splits into Connectivity, Identy, and Management, and Landing Zones, which splits into corp  and online, plus Sandbox and Decommissioned.
 - Platform subscriptions: Hub VNet, Azure Firewall, Bastion, Log Analytics, Defender for CLoud.
 - Landing Zone Subscription: Spoke VNets peered to the hub, workload resources.
 - Policy-driven guardrails: Allowed locations, required tags, Networkrestrictions, auto-enabled diagnostics and defender, assigned via policy initiatives at management group scope. 

## Tech Stack
   - Terraform.
   - Azure Policy, initatives and assignments.
   - GitHub Actions for CI/CD, plan on pull request, apply on merge.
   - Checkov or tfsec for security scanning.

## Getting started
     Coming soon as the project is built out.
     
## status 
    Work in progress — built step by step as a learning and portfolio project.
