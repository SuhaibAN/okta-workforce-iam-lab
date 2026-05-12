# Access Governance and Exception Access

## Objective

The objective of this lab was to simulate access governance activities, including access reviews, approval logic, and temporary exception access.

## Access Review Simulation

An access review matrix was created to validate:

- User
- Department
- Group membership
- Application access
- Access type
- Risk level
- Business justification
- Manager approval
- Review decision

## Example Access Review

| User | Department | Group | Application | Access Type | Risk Level | Review Decision |
|---|---|---|---|---|---|---|
| Omar Hassan | HR | HR-Team | HR Portal | Standard | Low | Keep |
| Sarah Miller | Finance | Finance-Team | Finance Portal | Standard | Low | Keep |
| Alex Chen | IT | IT-Admins | IT Admin Portal | Privileged | High | Keep with review |
| Mark Wilson | Contractor | Contractors | Contractor Portal | Limited | Medium | Remove when contract ends |

## Privileged Access Review

Alex Chen was assigned to the IT-Admins group and had access to the IT Admin Portal.

Control requirements:

- Manager approval
- MFA enforcement
- Quarterly access review
- Least privilege validation

## Contractor Access Review

Mark Wilson was assigned to the Contractors group.

Control requirements:

- Limited access
- Time-bound access
- Removal at contract end date
- Periodic review

## Exception Access Workflow

Daniel Reed needed temporary Finance Portal access while his standard role was HR.

Temporary access flow:

```text
Daniel Reed → Finance-Portal-Temporary-Access → Finance Portal
