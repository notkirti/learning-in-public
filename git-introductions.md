# quick intro to real env
## System Integration Testing (SIT), User Acceptance Testing (UAT) & Production (Prod)


Q: What is Alpha (SIT), and what is its purpose in the development lifecycle?
A: To check if the code that is being worked on can be integrated? To ensure that the new code is works with the existing code? (Environment where diff parts of the system r combined and tested together as a whole)

A: What kind of testing happens here?
Q: Functional testing - unit, integration, systems end-to-end and acceptance (sanity)

A: Who usually uses it?
Q: The developers, testers (technical crowd)

A: What is Beta (UAT), and why is it different from Alpha/SIT?
Q: To ensure that the code is working for the end-users. Different because the testing is done by the invited end-users. (Checks if the system complies w/ business requirements)

A: Who is responsible for testing in this stage?
Q: The invited end-users & stakeholders (business owners/users, product owners)

A: What kind of feedback is expected?
Q: How much the functionalities follows the expected deliverables and business rules? Bugs?

Q: What is the Production (Prod) environment, and why is it treated differently from all others?
A: The part that is actually shown to the users publicly? Treated diff because it affects the company's reputation, day-to-day use and privacy.

Q: What risks exist here?
A: Bugs? System incompatibility? Unknown issues arising? (Cost and reputation?)
  
Q: What rules should apply before changes reach Prod?
A: Testing? Code compliance? UAT approved? Rollback plan? System observerbility?
  
Q: What broader engineering umbrella do Alpha, Beta, and Prod fall under?
A: QA (doesnt compromise code quality), CI/CD (automated testing/deplyment), or Release Management (controls where, when & how the code will propagate through every statge and env.)?

Q: How do these concepts connect to deployment pipelines?
A: Enforces a step-by-step release with integrity confirmed throughout the entire deployment pipeline. Protects the functionality of the previous working system. It must all the tests prepared? 

Q: Why do companies separate environments instead of testing everything directly in Production?
A: To catch issues early on before it reaches the public users? (Reduces cost? Time 2 fix. Prevents rep loss? Damages user trust? Production data is irreversible)

Q: How do CI/CD pipelines control what moves from Alpha → Beta → Prod?
A: Automated deployment/testing? Branch rules? Environment/quality gates?