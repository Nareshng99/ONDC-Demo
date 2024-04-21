# ONDC - Open Network for Digital Commerce 🌐

ONDC is an ambitious initiative to democratize digital commerce by creating a decentralized network of buyer apps and seller apps through an interoperable protocol specification.

## Overview 📖

This comprehensive guide is designed to walk you through the process of integrating your digital commerce platform with the Open Network for Digital Commerce (ONDC). By following these steps, you'll enable seamless interoperability with the decentralized network, allowing your platform to leverage the benefits of ONDC.

## Table of Contents 📑

1. [Getting Started](#getting-started)
2. [Quick Start Guide](#quick-start-guide)
3. [The Protocol](#the-protocol)
4. [Subscription Process](#subscription-process)
5. [Signing and Verification](#signing-and-verification)
6. [Enabled Domains](#enabled-domains)
7. [Reference Applications](#reference-applications)
8. [Utilities](#utilities)

### Getting Started 🚀

The ONDC Web Portal serves as a self-service platform that streamlines interaction between ONDC and its network participants across their entire lifecycle. "Network player" encompasses network participants, ecosystem partners, and other entities engaged with ONDC. The portal provides access to a range of services for network players, such as self-service onboarding, self-monitored compliance, and self-monitored operations. Creating an account on [ONDC Web Portal](#) is necessary for starting your integration with ONDC.

### Quick Start Guide 🛣️

ONDC Integration Guide is a roadmap designed to illuminate key resources and navigate through the integration journey.

### The Protocol 📜

Beckn is an open protocol that allows local businesses across any industry to be discovered and engaged by any beckn-enabled application. Beckn protocol is a collection of open specifications consisting of protocol APIs, message formats, network design, and reference architectures to allow any two entities to execute commercial transactions without being on the same platform.

ONDC has provided the network extension layer over the Beckn Protocol (base layer). Over the base layer, the network extension layer comprises model specifications customized to the ONDC context that have been adopted to facilitate transactions over the network.

### Subscription Process 📝

To enroll in the ONDC network, Network Participants (NP) must be added to the registry. The steps for an NP to onboard onto the ONDC Registry (Staging, Pre Production, Production) are outlined as follows:

#### Staging Registry

- Obtain whitelisting for the subscriber ID.
- Initiate the subscription process by calling the `/subscribe` API. [The complete process is documented here](#).

#### Pre-Production Registry

- After presenting a demo and receiving approval from the relevant team, follow the outlined process to be added to the Pre-Prod registry.

#### Production Registry

- Upon successfully completing functional testing and satisfying the final checklist in Pre-Production, an NP can transition to the the Production environment.

### Signing and Verification 🔒

When communicating over HTTP using Beckn APIs, the subscribers need to authenticate themselves to perform transactions with other subscribers. Due to the commercial nature of the transactions, every request/callback pair is considered to be a "contract" between two parties. Therefore, it is imperative that all requests and callbacks are digitally signed by the sender and subsequently verified by the receiver.

[The complete process is documented here](#)

### Enabled Domains 🌍

Below are links to the comprehensive developer guide and model implementations for the enabled domains.

- **Retail** - This domain encompasses subcategories such as grocery, food and beverages, fashion, electronics, home & decor, beauty, and personal care, etc. It facilitates seamless transactions in both B2C and B2B modes, offering a comprehensive shopping experience for consumers and businesses alike.
  - [Retail Developer Guide](#)
  - [Test Case Scenarios - B2C](#)
  - [Test Case Scenarios - B2B](#)

- **Logistics** - This domain streamlines the acquisition of on-network logistics services, providing logistics buyers with a variety of choices for flexible solutions that suit their specific needs.
  - [Logistics Developer Guide](#)
  - [Test Case Scenarios - Logistics](#)

- **Financial Services** - This domain facilitates easy access to a spectrum of financial solutions, covering loans, insurance, investments.
  - [Financial Services Developer Guide](#)

- **Travel & Tourism** - This domain enables easy access to a range of travel-related services, covering On-demand Ride hailing with various transport modes, ticket booking without designated seat.
  - [Mobility Specifications Developer Guide](#)

- **Services** - This domain empowers individuals to effortlessly access a diverse array of services, covering home services like painting and consultations, etc.
  - [Services Developer Guide](#)

### Reference Applications 📲

The network participants need to complete the end-to-end testing with ONDC reference applications.

- **Staging Environment**
  - [ONDC Reference Seller App](#)
  - [ONDC Reference Buyer App](#)
  - [ONDC Reference Logistics Seller App](#)

### Utilities 🔧

- **Signing and Verification**: This tool is designed to support and aid ONDC Network Participants in constructing their own cryptocurrency libraries essential for engaging with the ONDC Network. It encompasses tasks such as key generation, signing, verification, encryption, and decryption.
  - [Java](#)
  - [NodeJS](#)
  - [Python](#)
  - [GoLang](#)

- **Subscription process**: This tool aids ONDC Network Participants during the subscription process for the registry (Staging, Pre Prod, Prod). It includes the implementation of the `/on_subscribe` API in both NodeJS and Python.
  - [NodeJS](#)
  - [Python](#)

- **Retail/IGM Log Verification**: This tool is designed for ONDC Network Participants to verify their transaction logs related to the Retail and IGM use cases on their end, ensuring accuracy before submission to the ONDC team for technical clearance.
  - [Log Verification Tool](#)

- **B2B/Logistics Log Verification**: This tool is designed for ONDC Network Participants to verify their transaction logs related to the B2B and Logistics use cases on their end, ensuring accuracy before submission to the ONDC team for technical clearance.
  - [Log Verification Tool](#)

- **vlookup**: This tool is developed to perform a registry lookup and retrieve details related to Network Participants (NP).
  - [RSF Mock Server](#): The RSF Mock Server is a tool specifically designed to test network integration for Reconcillation and Settlement Framework (RSF), based on ONDC model implementation.
