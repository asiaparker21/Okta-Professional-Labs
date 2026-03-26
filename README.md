# Okta-Professional-Labs
Lab 1: Okta Org Setup
Steps Performed
Created developer org
Verified domain email
Logged into Admin Console

Screenshots
All screenshots for this lab 1 are in the screenshots folder or click on the link below to view each step visually:

View Screenshots

Phase 1: User Creation (Joiner)
This phase focuses on the initial onboarding of users into the Okta Directory and observing the lifecycle transition from Staged to Active.

1. Manual Provisioning & Staged Status
I initiated the Joiner process by manually creating two users via Directory → People. This allowed me to test different activation flows:

User A: Self-activation via email.

User B: Admin-set password for immediate access.

Observation: Before the first user interacted with their email, the account held a Staged status. This is a critical security state where the identity exists but cannot yet authenticate.

Phase2: Suspension (Temporary Access Restriction)
Suspended active user account.

Attempted login via incognito session.
(Insert screenshot here titled "Suspended users cannot log in but retain assignments").

IAM Insight: Suspension is used for temporary access restriction without removing entitlements

3. Deactivation (Leaver Phase)
Deactivated user account.

Verified:

Access revoked
Sessions terminated
Application access removed
IAM Insight:
Deactivation enforces complete access revocation and is used during employee offboarding.

(Insert screenshot here titled "Deactivation revoked access and terminated active sessions").

Expected Behavior/Result
User receives activation email
Access granted based on group membership
User successfully provisioned and able to authenticate
Suspended user authentication blocked while group and application assignments remained intact
Screenshots
(Insert all screenshots mentioned above)

What is User Lifecycle Management?
User Lifecycle Management (ULM) is the process of managing digital identities from account creation to deactivation, ensuring proper access control throughout the user’s relationship with the organization Proper lifecycle management:Prevents orphaned accounts, reduces insider risk, enforces least privilege and ensures timely access revocation Lifecycle Phases in IAM are- Joiner- Account creation and access provisioning Mover- Role change and access modification Leaver- Access revocation and account deactivation
