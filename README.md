# SDLC Assignment - Nabajyoti Kalita

This repo contains my submission for the "Release Manager" Roleplay assignment for the SDLC & DevOps Fundamentals course. 

Files included:
- `Analysis.pdf`: My analysis on why the Waterfall model wouldn't work for this scenario.
- `Backlog.csv`: The Sprint 1 backlog with user stories.
- `README.md`: Explanation of why we'd use CI/CD.

## Why use CI/CD for pushing Sprint updates?

Since we switched to the Agile (Scrum) framework to deal with the Dean's new requirement, we are now working in short 2-week sprints. This means we have to release updates quickly and often. So we'd use Continuous Integration/Continuous Deployment (CI/CD) to make this process automatic.

Here's why CI/CD is really useful for our app:

1. **Testing the new Face ID code:** As we code the new Biometric stuff in Sprint 2, Continuous Integration (CI) will automatically run tests every time we commit our code. This makes sure that adding the Face ID doesn't accidentally break the login UI or the geo-fencing features we already built in Sprint 1.

2. **Automatic updates for students:** Continuous Deployment (CD) automatically pushes the completed app straight to the students' phones. At the end of Sprint 1, it pushes the MVP so students can start using the geo-fencing right away. Then, at the end of Sprint 2, it automatically updates their apps with the new Face ID feature without the school's IT department having to do it manually.

3. **Getting feedback faster:** Because we can push the Sprint 1 app automatically, students can try out the UI and the geo-fencing early on. If they complain that the geo-fencing radius is bad or the UI is confusing, we can quickly take that feedback and fix it in Sprint 2. If we didn't have CI/CD, pushing the app would take so long that we wouldn't get feedback in time.
