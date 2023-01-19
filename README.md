# securing-apis
Collection of notes &amp; techniques relating to API security

## Overview

## Why you *SHOULDN'T* implement security controls in your API code

Many organisations make the mistake of implementing security controls inside their API code. Here's a few reasons why this is the wrong approach to take:
- the percentage of developers who are also security experts is very low
- many developers frequently move between different organisations & industries
- organisation-level security requirements should be managed at an organisation level
- security requirements for APIs evolve over time

Your developers should be developing APIs on the assumption that adequate & appropriate security controls will be implemented outside of their code. In most cases, it's entirely appropriate for API developers to assume (unencrypted) https request traffic is all they need to deal with.

## Use API gateways & WAFs

## OWASP

### AWS WAF

### Kong + wallarm

### Kubernetes: policies & Gatekeeper

### modsecurity

## East-west vs north-south

## Traffic encryption

## Payload scanning & schema validation

## Authentication & authorisation

## It's not just *your* APIs that can hurt you

Many organisations consume 3rd party APIs as well as providing their own APIs. In many cases, servicing an incoming API request will require sending a request to a 3rd party API and processing the response, before responding to the original API request.

In these cases it's important to consider the risks involved in blindly accepting responses from 3rd party APIs.

## GraphQL is different

### References
- https://the-guild.dev/graphql/envelop/docs/guides/securing-your-graphql-api
- https://escape.tech/blog/9-graphql-security-best-practices/
- https://crashtest-security.com/graphql-security-vulnerabilities/
- https://brightsec.com/blog/graphql-security/
- https://www.fastly.com/blog/exploring-the-security-implications-of-graphql
- https://www.howtographql.com/advanced/4-security/

## Language-specific concerns

## Emerging trends
