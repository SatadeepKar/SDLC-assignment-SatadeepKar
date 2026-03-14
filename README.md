# SDLC Assignment - Satadeep Kar

This repository contains my submission for the "Release Manager" Roleplay assignment in the SDLC & DevOps Fundamentals course.

Files included:

- `Analysis.pdf` / `Analysis.md`: Detailed analysis of why the Waterfall model fails for changing requirements and how the Scrum framework solves this.
- `Backlog.csv`: The Sprint 1 backlog with user stories, estimated hours, and priorities.
- `README.md`: Explanation of why we would implement a CI/CD pipeline.

## Why use CI/CD for pushing Sprint updates?

Since we switched to the Agile (Scrum) framework to manage the Dean's mid-project pivot, we are now releasing software in iterative 2-week sprints. Releasing software manually every two weeks is prone to human error, slow, and tedious. To handle this, we would implement a **Continuous Integration and Continuous Deployment (CI/CD)** pipeline to automate the process of getting the app out to the university students.

This section explains why CI/CD is critical for the "Smart-Attend" app:

1. **Continuous Integration (CI) prevents regression bugs:**
   When the development team starts building the new Face ID feature in Sprint 2, they will be altering the codebase that was stabilized in Sprint 1. With CI, every time a developer commits code to GitHub, an automated pipeline (like GitHub Actions or Jenkins) immediately builds the app and runs automated unit tests. This ensures the new Face ID logic doesn't accidentally break the existing Geo-fencing system or the University ID login. If a test fails, the code is blocked from merging, keeping our main branch stable.

2. **Continuous Deployment (CD) automates distribution:**
   In a traditional setup, pushing an update requires the university IT team to manually package the app and distribute it, which takes days. With CD, once the code passes all CI tests, the pipeline automatically compiles the production app bundle (APK/IPA) and publishes it directly to testing environments (like TestFlight or Google Play Beta) or straight to the students' phones. This allows us to hit our 2-week Sprint release goals effortlessly at the end of Sprint 1 (the MVP) and Sprint 2 (the Biometric update).

3. **Faster Feedback Loops & Hotfixes:**
   Agile relies entirely on user feedback. Because CD allows us to safely push the Sprint 1 MVP automatically, students can test the geofencing in the real world immediately. If they discover a critical bug (for example, the GPS drains phone battery), the developers can write a fix, and the CI/CD pipeline can automatically push the patched version to all students within minutes, rather than waiting for another massive, manual release cycle.
