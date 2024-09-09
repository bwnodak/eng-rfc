# Engineering RFC Repository

This repository is the single source of truth for engineering RFCs (Request for Comments) within our team. The purpose of this repository is to streamline the discussion, development, and approval of major engineering decisions and projects. Using GitHub's version control, templates, notifications, and comments, we aim to foster open participation and maintain clear records of discussions and decisions.

## What is an RFC?

An RFC is a proposal for significant changes or projects that affect our engineering workflow, architecture, or other technical decisions. They are used to outline an approach and gather feedback from the team before moving forward.

### Rules of Thumb: When to Create an RFC

Not every change or project needs an RFC, but here are some guidelines to help you decide when one is appropriate:

- **Significant Architectural Changes**: If a proposal involves changing how systems interact, introducing new technologies, or modifying the structure of core components, an RFC is recommended.
  
- **High-Risk or Large Projects**: If the change could have major impacts on stability, performance, or security, or if it involves a significant time or resource commitment, it's best to formalize it with an RFC.

- **Cross-Team Impact**: If the project or decision affects multiple teams, requires coordination across departments, or will change workflows for multiple stakeholders, an RFC should be written to ensure alignment.

- **New Frameworks, Libraries, or Tools**: Introducing new third-party dependencies or frameworks that will be widely adopted should go through the RFC process for evaluation.

- **Breaking Changes**: If your change will cause backward incompatibility with existing systems or APIs, it’s important to outline the risks and mitigation strategies in an RFC.

- **Key Infrastructure Updates**: Any modifications to critical infrastructure components (e.g., CI/CD pipelines, logging systems, or cloud configurations) should be proposed via RFC.

- **Unclear or Controversial Changes**: If the proposal is likely to generate a lot of debate or if there are multiple ways to approach the problem, an RFC helps structure the conversation and reach consensus.

- **New Processes or Standards**: Proposals that impact how the team works (coding guidelines, workflows, testing strategies) should be formalized in an RFC to ensure everyone is on board.

**When an RFC May Not Be Needed:**

- **Small or Low-Risk Changes**: Bug fixes, minor refactoring, or small feature additions that don’t significantly alter workflows or architecture generally don’t require an RFC.
  
- **Team-Specific Adjustments**: Changes that are contained to a single team or have no external dependencies may not require an RFC unless they impact others.
  
- **Routine Updates**: If the change is a routine update to documentation, configurations, or dependencies with no breaking changes, it can typically skip the RFC process.


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
   - Merging an RFC means that the project can begin implementation.
   - If approval state changes, the RFC should be reverted.

## Guidelines for RFCs

- **Keep it simple:** Only include as much detail as necessary. Save deep technical dives for high-risk or large projects.
- **Open collaboration:** Everyone should participate in discussions. Turn on notifications for this repo to stay informed.
- **Sponsorship:** Every RFC requires at least one Staff+ engineer sponsor for approval.
  
## Repository Structure

├── README.md                         # Overview of the repository 
├── rfcs/                             # Folder containing all RFCs 
│ └── yyyy-mm-dd-rfc-title.md         # Individual RFCs, named by date and short title 
└── .github/ 
  └── ISSUE_TEMPLATE.md               # Template for pre-RFC issue discussion 
  └── PULL_REQUEST_TEMPLATE.md        # Template for RFC pull requests
