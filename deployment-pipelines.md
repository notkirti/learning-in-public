# Deployment Pipelines and Testing Stages
## System Integration Testing (SIT), User Acceptance Testing (UAT) & Production (Prod)

### System Integration Testing (SIT) or Alpha
Q: What is Alpha (SIT), and what is its purpose in the development lifecycle?
A: It is the environment where different parts of the system are combined and tested together as a whole. 

Q: What kind of testing happens here?
A: Functional testing - unit testing, integration testing, end-to-end system testing, and sanity checks.

Q: Who usually uses it?
A: The technical team (Developers and QA Testers).

### User Acceptance Testing (UAT) or Beta
Q: What is Beta (UAT), and why is it different from Alpha (SIT)?
A: It checks if the system complies w/ business requirements. It is different because the testing is done by the invited end-users as well as the stakeholders and not the technical team.

Q: Who is responsible for testing in this stage?
A: The invited end-users and the stakeholders (business owners/users &product owners).

Q: What kind of feedback is expected?
A: How much the functionalities follows the expected deliverables and business rules.

### Production (Prod)
Q: What is the Production (Prod) environment, and why is it treated differently from all others?
A: It is the enviroment that is shown to the users publicly. It is treated differently because it affects the company's reputation, day-to-day use and privacy.

Q: What risks exist here?
A: Bugs, system incompatibility and unknown issues arising that may lead to financial costs and reputation loss.
  
Q: What rules should apply before changes reach Prod?
A: It must pass all the reuqired testing, adhere to code compliance, ensure that is UAT approved and have a rollback plan and system observerbility set in place.

### Continuous Integration and Continuous Delivery/Deployment (CI/CD) & Release Management
Q: What broader engineering umbrella do Alpha, Beta, and Prod fall under?
A: It falls under Quality Assurance (QA) so that the code quality isnt compromised, CI/CD so that that the testing and the deployment is automated and Release Management which controls where, when and how the code will propagate through every stage and environment.

Q: How do these concepts connect to deployment pipelines?
A: It enforces a step-by-step release with integrity confirmed throughout the entire deployment pipeline and it protects the functionality of the previous working system.

Q: Why do companies separate environments instead of testing everything directly in Prod?
A: It is done to catch issues early on before it reaches the public user, protects prouduction data from irreversible changes, reduce costs, prevent reputation loss and damage to user trust.

Q: How do CI/CD pipelines control what moves from Alpha → Beta → Prod?
A: It does this through automated deployment/testing, branch protection rules and quality gates to ensure that the code will not move to the unless it passes the required tests.