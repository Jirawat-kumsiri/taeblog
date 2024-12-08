---
title: Title of the post
description: 
date: 2024-11-06
tldr: 
draft: false
tags:
  - tag
  - names
toc: true
---
## SUMMARY
Guido and Frank discuss their lessons from implementing and improving test automation using Robot Framework over years, emphasizing best practices and conventions.

## IDEAS
- Effective automation starts with organizing test cases and separating reusable components into resource files.
- Avoid direct communication between test cases and the system; use intermediary resource files.
- Logical separation of files, such as screens, common actions, and shared functionality, enhances maintainability.
- Keep resource files compact, readable, and maintainable by splitting large functionalities into smaller files.
- Centralize locators within single-action keywords to minimize duplication and reduce locator management complexity.
- Composite keywords should check their completion status to ensure subsequent tests run without errors.
- Start each keyword with validation to confirm the proper context or screen before execution.
- Naming conventions for single-action keywords aid clarity and understanding in test suites.
- Separate technical details and business logic into distinct layers for clarity and stakeholder involvement.
- Stakeholder-friendly "business object" resource files should focus on functional, non-technical details.
- Technical details, like locators and logic, belong in "page object" resource files.
- "Assertion layer" ensures functional correctness without cluttering business objects.
- Prefix validation keywords with clear terms like "validate" to distinguish them in tests.
- Use directory-level test execution to organize and manage extensive end-to-end test setups.
- Split long end-to-end tests into modular test suites for flexibility and easier debugging.
- Keep setup and teardown logic outside test suites for clarity in specific test validations.
- Maintain stakeholder involvement by using their language in business layer test definitions.
- Utilize prefixes in resource file keywords to resolve ambiguous names and improve readability.
- Collaborate with developers to avoid the need for dynamic locators, simplifying automation.
- Domain language capture in the business layer facilitates alignment between testers and stakeholders.
- Modular testing ensures resilience against system changes by isolating specific functionalities.
- Define conventions for layer separation to enable maintainable and scalable test frameworks.
- Use consistent naming for validation steps to streamline debugging and stakeholder understanding.
- Dynamic fields can be handled with title-based locators or parametrized validations.
- JSON transfers between systems help align real-world application interactions and test automation.
- Modular test files ease switching components when applications are temporarily unavailable.

## INSIGHTS
- Separation of business logic and technical details builds frameworks readable for both testers and stakeholders.
- Modularization and logical resource file organization ensure long-term test maintainability and clarity.
- Collaboration with developers reduces automation complexity and improves locator stability.
- Business layer clarity fosters better communication and alignment between technical and non-technical teams.
- Validation at every step prevents silent failures and ensures more robust test outcomes.
- Prefixes in keyword naming avoid ambiguities and improve framework scalability.
- Layered architecture facilitates parallel test case development and system readiness checks.
- Assertions should be explicit and clearly identified to improve test integrity and results clarity.
- End-to-end tests should be modular, not monolithic, for resilience and easier maintenance.
- Stakeholder language integration in business layers builds trust and improves test case relevance.

## QUOTES
- "The fastest way to drop jaws is showing manual testers automated clicks."
- "Keywords must finish themselves to ensure the next ones won’t fail prematurely."
- "Keep resource files compact, readable, and maintainable by splitting larger functionalities."
- "The business object layer should only contain functional descriptions stakeholders understand."
- "Ambiguous keywords are a nightmare; use naming prefixes to resolve conflicts."
- "Validation steps must ensure system correctness without cluttering the business layer."
- "Stakeholders should not look at us like rabbits before an 18-ton truck."
- "Separate technical details from functionality to make test cases readable by stakeholders."
- "Test cases should end with validation keywords to confirm they achieved their purpose."
- "Dynamic locators should be avoided whenever possible through collaboration with developers."
- "Composite keywords must check if actions are complete before moving on."
- "Resource files must align with business layers for clarity and modularity."
- "Assertions are for testers, while business objects cater to stakeholder understanding."
- "Layer separation facilitates simultaneous test case creation and system readiness testing."
- "Organize long end-to-end tests into modular files for flexibility and clarity."

## HABITS
- Collaborate with developers early to simplify automation and avoid dynamic locators.
- Use clear naming conventions for single-action and composite keywords to improve clarity.
- Validate each test keyword’s context and outcome before advancing to the next step.
- Modularize tests into small, maintainable resource files for easier debugging and updates.
- Separate technical complexities into page objects to reduce stakeholder confusion.
- Use logical naming prefixes for keywords and files to resolve potential ambiguities.
- Align test terminology with stakeholder language to ensure mutual understanding.
- Create assertions as separate validation layers to confirm functional correctness.
- Modularize end-to-end tests into smaller test suites for scalability and resilience.
- Reserve test setup and teardown actions for designated files outside the core tests.
- Prefix assertion keywords with terms like “validate” for immediate recognition.
- Consolidate locator usage within keywords to reduce redundancy and errors.
- Develop tests incrementally to parallelize work on system readiness and test case creation.
- Utilize consistent conventions for page and business object layers to enhance readability.

## FACTS
- Robot Framework allows modularization through resource file organization for better test management.
- Test locators can often be simplified by avoiding dynamic parameters with developer collaboration.
- Stakeholders may find technical test scripts overwhelming without functional abstraction layers.
- Composite keywords must ensure their completion status before the next test step begins.
- Modular test frameworks enable switching out unavailable or incomplete system components.
- Validation steps are vital for ensuring test outcomes reflect real system behavior.
- JSON is often used for system-to-system data transfer in end-to-end tests.
- Consistent naming conventions in test frameworks improve scalability and reduce ambiguity.
- Modularized end-to-end testing eases debugging and reduces system interdependencies.
- Prefixes like "validate" distinguish validation steps from core test actions.

## REFERENCES
- Robot Framework documentation and best practices.
- JSON as a format for system-to-system communication.
- Giren language concepts for capturing stakeholder language in test layers.
- Page Object and Business Object design patterns in test automation.

## ONE-SENTENCE TAKEAWAY
Effective test automation frameworks rely on clear modularization, stakeholder alignment, and robust conventions for maintainability.

## RECOMMENDATIONS
- Modularize resource files to keep frameworks maintainable and scalable over time.
- Use clear prefixes in naming conventions to eliminate ambiguity in keywords.
- Validate every test case step to ensure accurate outcomes and prevent silent failures.
- Separate technical complexities from business logic for improved stakeholder readability.
- Engage stakeholders early to align test layers with domain language and requirements.
- Collaborate with developers to avoid using dynamic locators wherever possible.
- Split end-to-end tests into smaller suites for better debugging and flexibility.
- Organize tests logically to enable team-wide understanding and collaboration.
- Use assertion layers for validations without polluting business object layers.
- Document conventions for team consistency across test automation frameworks.
- Utilize titles or unique identifiers to manage dynamic elements in locators.
- Place setup and teardown actions outside core test suites for clarity.
- Develop tests incrementally to accommodate system readiness and parallel workflows.
- Incorporate domain-specific language into business objects for stakeholder clarity.
- Align test cases with stakeholder goals to enhance relevance and engagement.



https://youtu.be/v4gWC7GPxT4?si=_ScZLoAoEvh_ds3Y