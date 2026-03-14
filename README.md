## Why implement CI/CD for Sprint releases?

After shifting from the **Waterfall model to the Agile Scrum methodology** to address the Dean’s new biometric requirement, the development team now works in **two-week sprint cycles**. Manually releasing an update after every sprint would be time-consuming and increases the chances of human error.

To make the release process more efficient and dependable, a **Continuous Integration and Continuous Deployment (CI/CD) pipeline** would be introduced. This automated pipeline ensures that each update of the **Smart-Attend** application is properly tested and delivered to students quickly and reliably.

Below are the main reasons why CI/CD is essential for this project.

---

### Continuous Integration (CI) helps prevent regression bugs

In **Sprint 2**, developers start working on the **Face ID authentication feature**. This feature modifies parts of the codebase that were completed earlier, including the **Geo-fencing attendance system** and the **University ID login** built during Sprint 1.

With CI in place, whenever a developer pushes code to the **GitHub repository**, an automated workflow (using tools such as **GitHub Actions** or **Jenkins**) will:

- Automatically build the application  
- Execute all predefined unit tests  

If any of the tests fail, the update is blocked from merging into the **main branch**. This ensures that newly added features do not accidentally break existing functionality and keeps the primary codebase stable.

---

### Continuous Deployment (CD) streamlines the release process

Without automation, releasing a new version would require the **university IT team** to manually prepare and distribute the application update, which could take several days.

With CD, once all CI checks pass:

- The pipeline automatically builds the **production version of the app (APK/IPA)**  
- The compiled build is then deployed to testing platforms such as **Google Play Beta** or **TestFlight**, or directly distributed to users  

This automated workflow enables the team to deliver updates smoothly at the end of each sprint, including **Sprint 1 (the MVP)** and **Sprint 2 (the biometric feature update)**.

---

### Faster feedback and quicker fixes

One of the key benefits of Agile development is the ability to collect **rapid user feedback**.

Because the CI/CD pipeline can deploy the **Sprint 1 MVP** immediately, students can begin using the geofencing attendance system in real-world scenarios. If users encounter a major issue—for example, **high battery consumption caused by GPS usage**—developers can quickly implement a fix and push the update through the pipeline.

The corrected version can then be delivered to users **within minutes**, instead of waiting for another large manual release cycle.
