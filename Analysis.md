# Analysis: Why the Waterfall Model Would Fail in This Situation

## Task 1: Why Waterfall Fails Here

In the Smart-Attend app project, the development is already halfway complete when the Dean introduces a major new feature: biometric verification using Face ID to prevent proxy attendance. If this project were following the traditional Waterfall model, adding such a requirement at this stage would cause serious problems. Below are three main reasons why:

1. Lack of Flexibility (Sequential Phase Issue)

The Waterfall model follows a strict step-by-step process: Requirements → Design → Development → Testing → Deployment. Each stage must be fully completed and approved before moving forward.

Since development is already underway, introducing the Face ID feature would force the team to go back to the initial requirements stage. The Business Requirements Document (BRD) would need to be rewritten and approved again. This disrupts the linear process of Waterfall and delays the entire project schedule.

2. Expensive and Difficult Changes

In Waterfall projects, the system design and architecture are finalized early in the design phase. The current system for Smart-Attend was originally built only to handle GPS-based geo-fencing and simple student ID records.

Adding biometric authentication now would require major modifications. The database would need to support secure storage of biometric data, the application would need camera access and facial recognition functionality, and additional privacy and security compliance would have to be implemented. Making such large changes after development has started would significantly increase both cost and development time.

3. Late Testing Risks (Delayed Integration Testing)

Another weakness of Waterfall is that testing usually occurs near the end of the project. If the biometric system is forced into the current geo-fencing structure, the combined system may not be tested until the final months of the project.

For example, the Face ID module might consume a large amount of device memory, which could cause the background geo-fencing service to fail or crash. If such compatibility problems are discovered late in the process, the team may not have enough time to fix them before the release deadline, increasing the risk of a failed product launch.

## Task 2: Switching to an Agile Approach (Using Scrum)

To manage the Dean’s new request effectively, the team should move from the Waterfall model to the Agile Scrum framework. Scrum supports changing requirements by dividing work into short development cycles called Sprints, usually lasting two weeks. This allows the team to deliver small working versions of the product and continuously improve it based on feedback.

Sprint 1 – Minimum Viable Product (MVP)

The objective of the first sprint is to build a basic but functional version of the application as quickly as possible.

The Sprint Backlog will include:

Designing the main user interface and navigation structure.

Implementing a basic login system using the University ID.

Developing and testing the geo-fencing attendance mechanism so that students can automatically mark attendance when they are within the approved location.

At the end of Sprint 1, the team will have a working MVP that can be shown to stakeholders for early feedback.

Sprint 2 – Feature Enhancement

During the second sprint, the team will review the results of the MVP and begin implementing the Dean’s new requirement.

The focus will be on:

Adding Face ID biometric verification to the login process to prevent proxy attendance.

Improving the geo-fencing accuracy and attendance reporting dashboard based on feedback and issues discovered in Sprint 1.

By following this Agile process, the team can safely introduce the new biometric feature without disrupting the entire project, since each sprint builds upon the previous working version of the product.
