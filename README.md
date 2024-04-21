<p align="center">
  <img src="https://ondc.org/assets/theme/images/ecom/how-will-change-snap.svg?v=f86d4cd703" alt="ONDC Logo"/>
</p>

# Open Network for Digital Commerce (ONDC)

**ONDC** aims to democratize digital commerce by creating a decentralized network that connects buyer apps and seller apps through an interoperable protocol specification. This initiative supports a more inclusive digital commerce ecosystem.

## Overview

This guide is tailored for developers looking to integrate their digital commerce platforms with ONDC, facilitating seamless interoperability within a decentralized network. By integrating with ONDC, your platform can leverage a wider network, enabling more robust digital commerce transactions.

## 📚 Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Quick Start Guide](#quick-start-guide)
- [The Protocol](#the-protocol)
- [Subscription Process](#subscription-process)
- [Signing and Verification](#signing-and-verification)
- [Enabled Domains](#enabled-domains)
- [Reference Applications](#reference-applications)
- [Utilities](#utilities)

## 🌟 Introduction

The **Open Network for Digital Commerce (ONDC)** is an innovative project launched to promote open networks developed on open-sourced methodology, using open specifications and open network protocols, independent of any specific platform.

## 🚀 Getting Started

The first step is to create an account on the [**ONDC Web Portal**](https://portal.ondc.org/), a comprehensive self-service platform that facilitates the interaction between ONDC and its network participants throughout their integration lifecycle.

## 🌟 Quick Start Guide

Explore the [**ONDC Integration Guide**](https://docs.google.com/presentation/d/1HPRXk3lVYKmyAFcApgukZuwHhIZ_VlqR/edit#slide=id.g27b2e3e34a2_28_199), a detailed roadmap highlighting key resources and steps required for a smooth integration process.

## 🔗 The Protocol

ONDC utilizes the **Beckn Protocol**—an open standard that enables local businesses across various industries to connect with beckn-enabled applications for seamless commercial transactions.

## 📜 Subscription Process

Integration with ONDC involves several key stages, each requiring specific actions:

- **Staging Registry:** Begin by obtaining a subscriber ID and initiating the subscription process via the `/subscribe` API.The complete process is documented [**here**](https://github.com/ONDC-Official/developer-docs/blob/main/registry/Onboarding%20of%20Participants.md)
- **Pre-Production Registry:** After a successful demo, move to the pre-production stage as per the [**guidelines**](https://github.com/ONDC-Official/developer-docs/blob/main/registry/Onboarding%20of%20Participants.md).
- **Production Registry:** Upon passing functional testing, transition to the production environment.

## 🖋️ Signing and Verification

When communicating over HTTP using Beckn APIs, the subscribers need to authenticate themselves to perform transactions with other subscribers. Due to the commercial nature of the transactions, every request/callback pair is considered to be a **contract** between two parties. Therefore, all requests and callbacks must be digitally signed by the sender and subsequently verified by the receiver.

The complete process is documented[**HERE**](https://github.com/ONDC-Official/developer-docs/blob/main/registry/signing-verification.md).

## Enabled Domains 🔗

Below are links to the comprehensive developer guide and model implementations for the enabled domains.

### Retail 🛍️
This domain encompasses subcategories such as grocery, food and beverages, fashion, electronics, home & decor, beauty, and personal care, etc. It facilitates seamless transactions in both B2C and B2B modes, offering a comprehensive shopping experience for consumers and businesses alike.

- **B2C**
  - 📄 [v1.2](https://docs.google.com/document/d/1brvcltG_DagZ3kGr1ZZQk4hG4tze3zvcxmGV4NMTzr8/edit)
  - 🧪 [Test Case Scenarios - B2C](https://docs.google.com/spreadsheets/d/1JZV6ZQzXcHUsOwegGtArX3DdIXYIy3gxkhQ00q7kICc/edit#gid=1367601795)

- **B2B**
  - 📄 [v2.0.2](https://github.com/ONDC-Official/ONDC-RET-Specifications/tree/release-2.0.2)
  - 🧪 [Test Case Scenarios - B2B](https://docs.google.com/document/d/10ouiTKLY4dm1KnXCuhFwK38cYd9_aDQ30bklkqnPRkM/edit)

- 📘 [Retail Developer Guide](https://ondc-official.github.io/ONDC-RET-Specifications/)
  - For B2B, select version: [`release-2.0.2`](#)
  - For B2C, select version: [`draft-1.x`](#)

### Logistics 🚚
This domain streamlines the acquisition of on-network logistics services, providing logistics buyers with a variety of choices for flexible solutions that suit their specific needs.

- [v1.2](https://docs.google.com/document/d/1CkfxtqyLbSQccJZyNmf9BSGzJBH13gcLOk_tywV-LBk/edit)
- [B2B Logistics](https://github.com/ONDC-Official/ONDC-LOG-Specifications)
- 📘 [**Logistics Developer Guide**](https://ondc-official.github.io/ONDC-LOG-Specifications/)
  - For B2B Logistics, select version: [`draft-2.x`](#)
- 🧪 [Test Case Scenarios - Logistics](https://docs.google.com/spreadsheets/d/1JZV6ZQzXcHUsOwegGtArX3DdIXYIy3gxkhQ00q7kICc/edit#gid=1670900093)

### Financial Services 💰
Access a wide range of financial solutions effortlessly. This domain includes everything from loans to investment opportunities.

- 📘 [Financial Services Developer Guide](https://ondc-official.github.io/ONDC-FIS-Specifications/)
  - For Loans, select version: [`draft-loan`](#)
  - For Insurance, select version: [`draft-insurance`](#)
  - For Investments, select version: [`draft-mutual-funds`](#)
- 🎁 Gift Card

### Travel & Tourism ✈️
Enhance the travel experience with easy access to services like ride hailing and ticket booking for various modes of transport.

- 📘 [Mobility Specifications Developer Guide](https://ondc-official.github.io/mobility-specification/)
  - For On-demand Ride hailing, select version: [`draft-TRV10-2.0.0`](#)
  - For Unreserved Ticket Booking (metro and intracity bus), select version: [`draft-TRV11-2.0.0`](#)

- [Gift Card](https://docs.google.com/document/d/1iTCQd_jI3mRqgSiaeZBvxWL-G_wkE__xxW-Wua8arVE/edit)

### Services 🛠️
Empower individuals with a vast array of services at their fingertips, from home improvements to professional consultations.

- [v2.0.0](https://github.com/ONDC-Official/ONDC-SRV-Specifications/tree/draft-services)
- 📘 [Services Developer Guide](https://ondc-official.github.io/ONDC-SRV-Specifications/#)

### Ancillary Services 🌟
Support the ONDC network’s ecosystem with these essential services.

- **Issue & Grievance Management (IGM)**
  - [v1.0.0](https://docs.google.com/document/d/1UYGIo1fSOcA4ypnk5FuaCgUgNnu9dBQt/edit) - A critical mechanism for dispute resolution within the ONDC Network.
- **Reconciliation and Settlement Framework (RSF)**
  - [v1.0.0](https://docs.google.com/document/d/1ubUPAWpbbUJ4vG2h5TQ74srZBjYjrO0P/edit) - Ensures a transparent and accountable settlements system.
- **Rating**
  - [v1.2.0](https://docs.google.com/document/d/1VaafY8t47hjpoW6tdezGsPwLwxxaAaGc/edit) - Gauge the quality of network participants.
- **Score**
  - [v1.2.0](https://docs.google.com/document/d/126O1wFdA-IuwojiAuLzdpN36vjWfQg9KOA2zRd9-zTY/edit#heading=h.bifjra7hj5b0) - Assess the performance within the network.
  - [Test Case Scenarios (IGM & RSF)](https://docs.google.com/document/d/1tx86sypacIRXgL9nlNBdvHz7cYQjQoyC/edit)

### Reference Applications 📲

Network participants are required to perform end-to-end testing with ONDC reference applications to ensure seamless integration and functionality.

#### Staging Environment 🎭

- [**ONDC Reference Seller App**](https://ref-app-seller-staging-v2.ondc.org/sign-up) 
  - [![Github](https://github.com/ONDC-Official/seller-app-sdk/tree/master)](#)
  
- [**ONDC Reference Buyer App**](https://ref-app-buyer-staging-v2.ondc.org/login)
  - [![Github](https://github.com/ONDC-Official/ondc-sdk)](#)

- [**ONDC Reference Logistics Seller App**](https://ref-logistics-app-stage.ondc.org/) 
  - [![Github](https://github.com/ONDC-Official/ref-logistics-app-sdk/tree/main)](#)

#### Pre-Production Environment 🌐

- **ONDC Reference Seller App** 
  - [![Github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](#)
  
- **ONDC Reference Buyer App** 
  - [![Github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](#)

- **ONDC Reference Logistics Seller App** 
  - [![Github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](#)

### Utilities ⚙️

- **Signing and Verification**: 
  This tool supports ONDC Network Participants in creating their own cryptographic libraries, which are crucial for secure engagement with the ONDC Network. It includes key generation, signing, verification, encryption, and decryption tasks.
  - Java
  - [More info](#)



## 🛠️ Utilities

Enhance your integration with our array of utility tools designed for cryptographic operations, subscription management, and log verification.

## 🆘 Support

For queries or additional support, visit our [Help Center](#) or reach out to our support team.

