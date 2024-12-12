# Aegis
Static analysis tool for payment logic verification.

## Contents
- [Overview](#overview)
- [Why Aegis?](#why-aegis)
- [Installation](#installation)
- [Usage](#usage)
- [Core Features](#core-features)
  - [Static Analysis Engine](#static-analysis-engine)
  - [Security Verification](#security-verification)
  - [Integration Pattern Analysis](#integration-pattern-analysis)
- [Implementation Details](#implementation-details)
- [Requirements](#requirements)

## Overview
Aegis is a static analysis tool for [Stripe's Node.js library](https://github.com/stripe/stripe-node) designed to detect common server-side implementation errors and security vulnerabilities. The system analyzes your TypeScript codebase to verify critical patterns such as proper error handling, webhook security, idempotency usage, and payment intent lifecycle management.

## Installation
Coming soon

## Usage
Coming soon

## Core Features

### Static Analysis Engine
- [ ] Parse TypeScript code using Stripe's SDK
- [ ] Track Stripe API method calls and usage patterns
- [ ] Verify proper async/await and Promise handling
- [ ] Detect common integration anti-patterns
- [ ] Analyze control flow for error handling completeness

### Security Verification
- [ ] Detect exposed API keys in source code
- [ ] Verify webhook signature validation
- [ ] Check for PCI compliance patterns
- [ ] Identify potential security vulnerabilities
- [ ] Monitor for sensitive data exposure

### Integration Pattern Analysis
- [ ] Verify proper PaymentIntent lifecycle handling
- [ ] Check for idempotency key usage
- [ ] Analyze webhook setup and handling
- [ ] Validate error handling patterns
- [ ] Monitor retry logic implementation

## Implementation Details
- **Written in Scala**
- **Nix for reproducibility**
    - Nix Flake provided for hermetic builds
    - [devenv](https://devenv.sh) for flexible and reproducible dev environments

## Requirements
- TypeScript codebase using `stripe-node`
- TypeScript >= 4.x
- Node.js >= 16.x 

> **Note**: Currently, Aegis is only planned to support TypeScript. JavaScript support may be added in a future release.
