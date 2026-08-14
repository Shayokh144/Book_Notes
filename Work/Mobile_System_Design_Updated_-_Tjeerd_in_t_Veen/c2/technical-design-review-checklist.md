# Technical Design Review Checklist

This checklist is a practical tool compiled from Chapter 2 of *Mobile System Design: Resourceful Engineering* [3, 25]. Use it to guide technical briefings, structure system design reviews, and uncover hidden constraints before writing a single line of production code [26, 62].

---

## 1. Deconstructing the Briefing (The Technical Landscape)
- [ ] **Draw the component landscape first:** Before debating frameworks, architectures, or folder structures, sketch a high-level graph of all domains and components needed to solve the business requirement [50, 51, 56].
- [ ] **Define high-level domains as nodes:** Treat each node as its own independent domain (e.g., UI Library, Core Feature, Storage, Network API) to allow parallel work [110, 115].
- [ ] **Decompose pragmatically:** Decompose nodes only until you feel you understand the problem well enough to start implementation—avoid wasting time detailing components down to the lowest level [60].
- [ ] **Distinguish between clear and unclear requirements:** Use regular outlines for resolved components and dashed outlines for components with lingering known/unknown requirements [59, 61].
- [ ] **List the "known unknowns" and "unknown unknowns":** Explicitly map out everything you currently do not know (e.g., error behaviors, data sources, caching needs) [43].

## 2. Uncovering Secondary Requirements (Working with Designers)
- [ ] **Challenge the designs to find edge cases:** Act as a partner to the designer rather than blindly implementing high-fidelity blueprints, allowing the team to iteratively improve the product [66, 71, 101].
- [ ] **Test with a worst-case content scenario:** Ask the designer for a view containing minimal, missing, or extremely verbose real-world content to ensure the layout does not break under poor conditions [70, 101].
- [ ] **Verify pre-existing components:** Check with other engineers to see if similar components already exist in the codebase or UI library to avoid reinventing the wheel [74, 101].
- [ ] **Ask general UI robustness questions:**
  - [ ] Is the screen scrollable when content overflows [75]?
  - [ ] What is the empty state design [75]?
  - [ ] Does the UI handle large dynamic text/font sizes [76]?
  - [ ] Are landscape mode and tablet layouts supported [76]?
  - [ ] Are errors presented inline, or as alerts? What about partial loading errors [76]?
- [ ] **Ask feature-specific functionality questions:**
  - [ ] How does the UI behave if a network call fails while the app is backgrounded [78]?
  - [ ] For items like callout messages or labels, is there a character limit before truncating or expanding [78]?
- [ ] **Quantify and prioritize time investments:** Shift conversations from a binary "worth it or not" to quantifying the exact time/effort of custom layouts (e.g., custom navigation bars) so the team can prioritize the core features first [72, 81, 82].

## 3. Aligning with Backend Engineers (Integration Planning)
- [ ] **Align on sessions, tokens, and environments:** Clarify staging environment availability, token handling, login timeouts, and timeout error responses as early as possible [89, 90, 102].
- [ ] **Request consolidated network calls:** Steer toward single network calls to populate screens to avoid the complexity of multiple client-side requests and prevent heavy server usage [91, 102].
- [ ] **Standardize error-handling strategies:** Propose explicit error codes instead of relying on string-based backend error messages, allowing the client to handle localization and fallback UI [92, 102].
- [ ] **Establish a quick verification tool (e.g., cURL):** Set up cURL commands to test backend API responses in isolation from the client app to instantly narrow down bugs [90, 93].
- [ ] **Adjust plans for first-integrator overhead:** If you are the first client integrating a new backend API, double or triple your estimated integration time to account for beta-testing backend issues [94, 102].
- [ ] **Check for auxiliary features:** Discuss offline storage requirements (e.g., persistent Store), push notifications, local caching, and synchronization strategies [86, 95, 96, 102].
