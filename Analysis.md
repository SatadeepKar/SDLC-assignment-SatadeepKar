# Assignment: "Release Manager" Roleplay
**Student Name:** Nabajyoti Kalita

# Task 1: Why Waterfall Fails Here

In our scenario for the "Smart-Attend" app, we're halfway through making the app when the Dean suddenly asks for a big new feature: Biometric (Face ID) verification. If we were using the traditional Waterfall model for this project, adding this midway would be a huge disaster. Here are 3 reasons why:

1. It's too rigid
The whole point of Waterfall is that you do things one step at a time. First you gather all the requirements, then you design it, then you code it. Once you move past the requirements phase, you aren't supposed to go back. Since we are already halfway done with development, going all the way back to the start just to add the Face ID requirement breaks the whole Waterfall flow. It's just not flexible enough to handle sudden pivots like this.

2. High cost of making changes
When we started coding, we built the app's foundation and database based on the original plan (which only had Geo-fencing). Dropping a massive new feature like Face ID into the mix right now means we'd probably have to throw away a lot of the code and designs we've already spent time and money on. It would take way longer and cost a lot more because we'd basically have to start parts of it over from scratch.

3. Testing happens too late
In Waterfall, you only really start testing the app at the very end of the project, after all the coding is finished. If we try to just jam the Face ID stuff into what we have now, we won't actually test if the old Geo-fencing system and the new Face ID system work together until the very end of the 6 months. By then, if something is broken or they clash, it will be too late to fix it before the deadline.

# Task 2: The "Agile" Pivot (The Scrum Framework)

To handle the Dean's new requirement without failing, we should switch to the Agile Scrum framework. This lets us break the remaining work into two short, 2-week Sprints so we can deliver value quickly and adjust to feedback.

## Sprint 1 (MVP)
This first sprint is all about getting the "Minimum Viable Product" (MVP) out the door. We'll focus exclusively on:
* Building the basic UI.
* Setting up the User Login system.
* Implementing the core Geo-fencing logic so students can actually start marking attendance.

## Sprint 2 (The Update)
In the second sprint, we update the app with the new stuff. We will:
* Integrate the new Biometric (Face ID) logic to prevent proxy attendance.
* Refine and improve the reporting dashboard based on the early feedback we get from people using the Sprint 1 MVP.
