# Architecture Review Board

## Purpose



## Scope



## SAD Tier Designations

Illustrative, not exhaustive...


SAD Tier | Tier Description
-----|------------
1 | Sufficiently broad and complex dependencies - with a high degree of risk - that it warrants a full ARB review/vote
2 | Limited/bounded scope - only requiring a subset of ARB participants (e.g., 3-5) to review/approve.
3 | TThe assigned EA authorized to review/approve
4 | TThe SA can review/approve
5 | Delivery team, with an attestation that they are compliant with all policies, standards, etc. - and that there are no (substantial) *new* technologies involved in the solution design - and that the solution utilizes approved integration patterns, etc.

For non-ARB organizations - a repository of Architecture Decision Records (ADRs) - used as the basis for recording key architecture decision outcomes. ADRs may be recorded by EAs, SAs, or the delivery team.


## Participant Roles
- ARB Chair
  + Voting member

- ARB Co-Chair
  + Voting member 
  + Facilitates meeting in the absence of the ARB Chair

- ARB Coordinator
  + Not a voting member 
  + Responsible for recording meeting minutes, votes, issues, follow-up actions
  + Point-of-Contact for ARB review meeting scheduling, agenda

- Key Voting Members:
  + ARB Enterprise Architecture representatives 
  + ARB Security Architecture representatives
  + ARB Domain Architecture representatives 
  + ARB Infrastructure Architecture representatives


## Selection/Entry Criteria

- Recommendation: Only Tier-1 and Tier-2 SADs should be scheduled for review/voting.

- SADs with Tier 3-5 *may* elect to request an ARB review session - for information purposes. 



## Frequency

- For large organizations, typically weekly. 



## Input Artifacts

- SAD prepared, submitted to ARB for internal review/feedback, two weeks prior (usually) to the scheduled ARB review date


## Output Artifacts

- ARB SAD Status
- ADRs (as appropriate) recorded in a central registry



## Possible ARB SAD Status Outcomes   

Review Status|Commentary
---|---
Approved| 
Approved with Modification| 
Approved with Exception| 
Reschedule, Rework Required| 
Reschedule, Additional Detail Required| 
Review Not Required| 
Not Reviewed|
Not Approved| 


