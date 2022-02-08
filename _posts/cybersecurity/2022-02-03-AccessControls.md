---
layout: post
title: Access controls (Chapter 5)
categories: cybersecurity
---

## AC Components

### Parts of AC

- Identification - who asks for the asset?
- Authentication - can the requestor be verified?
- Authorization - what can the requestor access?
- Accountability - how can we trace actions to an individual?

### Phases of AC

The above parts are divided into two phases:

- Policy definition
- Policy enforcement

### Types of AC

- Physical - keys, swipe card
- Logical - username, password
  - Roles kept in SK database, different objects for different users
  - Audit log is the **accountability piece**
  - Controls - biometrics, tokens, passwords, SSO (MFA)

### Security Kernel

![SK](https://i.imgur.com/L4VDtRV.png)

## AC Policies

A set of rules that allows certain users to perform certain actions on certain resources

### Four components

- Users
- Resources
- Actions - high level, 'what can you see, what can you do'
- Relationships - `+rwx`

# Authentication

## Types

- Knowledge - password, PIN, etc.
- Ownership - tokens, key
- Characteristics - retina
- Location
- Action

# ACL

- Discretionary (DAC) - owner deciedes permissions
- Mandatory (MAC) - determined by sensitivity of resource and security level of subject (military-level, strictest); this is a form of NAC 
- Nondiscretionary (NAC) - monitored by security administrator
- Rule-based - rules maintained by owner
- Role-based (RBAC) - based on the jobs a user is assigned
- Attribute-based (ABAC) - more understandable, in business terms, role-based ('executive', 'financial system' . . . )

# Centralized and Decentralized AC

Enforced through authentication, authorization and accounting (AAA) servers

## Centralized

## AAA servers

- RADIUS
- TACACS+
- DIAMETER
- SAML - XML based markup language for auth

## Decentralized

- Password AP (cleartext) and Challenge-Handshake Authentication Protocol (CHAP) (secure, hashed)
- OATH - ongoing reference for secure authentication