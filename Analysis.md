# Assignment: "Release Manager" Roleplay

**Student Name:** Satadeep Kar

# Task 1: Why Waterfall Fails Here

In our scenario for the "Smart-Attend" app, we are halfway through development when the Dean introduces a massive new requirement: Biometric (Face ID) verification to stop proxy attendance. If we were using the traditional Waterfall model for this project, trying to add this mid-way would completely derail it. Here are 3 specific reasons why:

1. It is too rigid (The Phase-Gate Problem)
   The Waterfall model works strictly in sequence—Requirements, Design, Implementation, Testing, and Deployment. Each phase must be signed off before the next begins. Because we are already halfway through development, getting the Face ID requirement means we are forced back to step one. We cannot simply "add" it; Waterfall's rigidity means we must rewrite the entire Business Requirements Document (BRD) and get it approved all over again, breaking the strict linear flow of the project.

2. High cost of making changes (The "Blueprint" Dilemma)
   In Waterfall, the system architecture (the "blueprint") is finalized during the Design phase. Our original database schema and backend were built exclusively to check GPS coordinates for Geo-fencing and log simple student IDs. Dropping Face ID in now means we have to drastically alter our database to securely store biometric data hashes, rewrite the app to request camera hardware permissions, and update our privacy compliance. Redesigning and rewriting these core components midway results in massive financial costs and major timeline delays.

3. Testing happens too late (The "Big Bang" Integration)
   Waterfall notoriously leaves the Testing phase to the very end of the project cycle. If we try to force the Biometric logic into the existing Geo-fencing code now, we won't actually test if they work together until month 5 or 6 out of the 6-month timeline. For example, what if the Face ID scanner takes up so much memory that it causes the background Geo-fencing tracker to crash? We wouldn't discover this critical conflict until it's far too late to fix before the deadline, leading to a catastrophic launch failure.

# Task 2: The "Agile" Pivot (The Scrum Framework)

To handle the Dean's new requirement without failing, we should drop Waterfall and switch to the Agile Scrum framework. Scrum allows us to embrace changing requirements by working in short, iterative 2-week cycles called "Sprints." This lets us deliver working software continuously and adapt based on feedback.

## Sprint 1 (MVP - Minimum Viable Product)

The goal of our first sprint is to get a usable version of the core product into the hands of users as fast as possible. Our Sprint Backlog will focus exclusively on:

- Developing the basic user interface (UI) and navigation.
- Setting up the standard User Login system (via University ID).
- Implementing and testing the core Geo-fencing logic so that students can start triggering automated attendance.
  By the end of this sprint, we will have a shippable MVP to demonstrate to stakeholders.

## Sprint 2 (The Update)

In the second sprint, we review the feedback from the MVP and tackle the Dean's new requirement. We will:

- Integrate the requested Biometric (Face ID) verification logic on top of the existing login flow to prevent proxy attendance.
- Refine the Geo-fencing radius and reporting dashboard based on any bugs or feedback discovered during the Sprint 1 review.
  Working this way ensures the new, complex feature is built safely on top of a stable MVP, rather than risking the whole project at once.
