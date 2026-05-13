# IAM Architecture Diagram

```mermaid
flowchart TD
    A[HR System / User Profile Attributes] --> B[Okta User Profile]
    B --> C[Okta Group Rules]
    C --> D[Okta Groups / RBAC]
    D --> E[Application Assignments]

    E --> F[HR Portal]
    E --> G[Finance Portal]
    E --> H[IT Admin Portal]
    E --> I[Real SAML Test App]

    H --> J[MFA / App Sign-In Policy]
    I --> K[SAML 2.0 Federation]
    K --> L[Test Service Provider]

    M[Access Request] --> N[Manager Approval]
    N --> O[Application Owner Approval]
    O --> P[Temporary Access Group]
    P --> E

    Q[Access Review] --> D
    R[Leaver / Offboarding] --> S[Deactivate User]
    S --> T[Remove App Access]
```

## Summary

This diagram shows the workforce IAM flow used in the lab:

- User attributes drive group membership
- Groups control application access
- SAML enables federation to external apps
- MFA protects privileged access
- Access requests and reviews support governance
- Offboarding removes access
