# Joiner, Mover, Leaver Lifecycle

## Objective

The objective of this lab was to simulate the identity lifecycle process for onboarding, department transfer, and offboarding using Okta.

## JML Overview

JML stands for:

- Joiner: a new user joins the organization
- Mover: an existing user changes department or role
- Leaver: a user leaves the organization

## Joiner Scenario

A new user, Daniel Reed, was created as a Finance user.

Access flow:

```text
Daniel Reed → Finance-Team → Finance Portal
```

## Screenshot Evidence

![JML user status showing Daniel Reed deactivated](../screenshots/jml-user-status-deactivated.png)

This screenshot validates the leaver scenario by showing Daniel Reed’s account status as Deactivated after offboarding.

## Interview Summary

I simulated JML lifecycle workflows in Okta by creating a new user, assigning access through department-based groups, moving the user between departments, and deactivating the account during offboarding. I also configured group rules to automatically assign users based on department attributes, which mirrors HR-driven provisioning in enterprise IAM environments.
