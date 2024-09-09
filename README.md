# Engineering RFC Repository

This repository is the single source of truth for engineering RFCs (Request for Comments) within our team. The purpose of this repository is to streamline the discussion, development, and approval of major engineering decisions and projects. Using GitHub's version control, templates, notifications, and comments, we aim to foster open participation and maintain clear records of discussions and decisions.

## What is an RFC?

An RFC is a proposal for significant changes or projects that affect our engineering workflow, architecture, or other technical decisions. They are used to outline an approach and gather feedback from the team before moving forward. RFCs are an effective way for an engineering organization to manage both historical and planned changes.

1. Any person in the org can create an RFC
2. These RFCs should always choose "timely" over "perfect"

## Rules of Thumb 

**When to Create an RFC**

If your proposal includes:

- **Involves significant changes** to architecture, core components, or cross-team dependencies (e.g., introducing new frameworks or modifying infrastructure).
- **Carries high risk** (impact on stability, performance, or security) or requires a substantial resource/time commitment.
- **Introduces breaking changes** that affect existing systems or APIs, or alters processes or standards (e.g., new workflows, coding guidelines).

**When an RFC May Not Be Needed**:

- **Low-risk or routine updates**: Bug fixes, minor feature additions, team-specific changes, or routine updates that don’t impact others.

## Process Overview

1. **Pre-RFC Discussion:**
   - Begin with an [Issue](https://github.com/{org}/eng-rfc/issues) in this repository. Use the provided issue template to outline the initial problem or idea.
   - Engage in discussions. Everyone is encouraged to participate.

2. **Creating an RFC:**
   - If the issue gains traction, support, and backing from one or more Staff+ engineers, it can be converted into an RFC.
   - Create a pull request (PR) with the RFC document using the provided template.
   - The RFC will go through rounds of feedback in the PR comments before approval.

3. **Approval:**
   - An RFC must be approved by at least one Staff+ engineer before being merged to `main`, indicating that it is accepted and will move forward.
   - Merging an RFC means that the project has been ratified and can begin formal planning and implementation (in coordination with engineering management).
   - If approval state changes, the RFC should be reverted.

## Guidelines for RFCs

- **Keep it simple:** Only include as much detail as necessary. Save deep technical dives for high-risk or large projects.
- **Open collaboration:** Everyone should participate in discussions. Turn on notifications for this repo to stay informed.
- **Sponsorship:** Every RFC requires at least one Staff+ engineer sponsor for approval.
  
## Repository Structure
```
├── README.md                         # Overview of the repository 
├── rfcs/                             # Folder containing all RFCs 
│ └── yyyy-mm-dd-rfc-title.md         # Individual RFCs, named by date and short title 
└── .github/ 
  └── ISSUE_TEMPLATE.md               # Template for pre-RFC issue discussion 
  └── PULL_REQUEST_TEMPLATE.md        # Template for RFC pull requests
```
