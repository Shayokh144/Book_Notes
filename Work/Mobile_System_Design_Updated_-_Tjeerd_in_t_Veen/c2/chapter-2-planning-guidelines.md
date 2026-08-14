# Chapter 2 Planning Guidelines: Turning a Briefing Into a Strong Plan

This guide outlines key practices for mobile engineers when translating feature designs and briefings into robust development plans, based on Chapter 2 of *Mobile System Design: Resourceful Engineering*.

## Should Do

*   **Try to understand the problem better before you start coding.** Ask questions to uncover hidden requirements. This step prevents major rewrites later. [42]
*   **Sketch a technical landscape diagram early in the planning phase.** Map out all required components and domains as nodes. Let your architecture grow organically over time. [36, 42]
*   **Align early with backend developers on critical systems.** Discuss session tokens, timeouts, and error codes. Propose consolidating multiple API calls into one. [81, 83, 85]
*   **Ask the designer for a worst-case scenario layout.** Real-world data is often ugly and missing. Ensure the design holds with poor content. [60]
*   **Identify pre-existing components before writing new code.** Talk to other mobile engineers on your team. Reusing existing views saves a lot of time. [64, 65]

## Should Not Do

*   **Do not start coding the UI right away.** This approach localizes your thinking too much. You might miss massive backend integration issues. [30, 31]
*   **Do not get bogged down in minor details.** Focus on high-level structures in the beginning. Defer styling and animations until much later. [40, 41]
*   **Avoid choosing a rigid UI architecture immediately.** Let your architecture evolve as you learn. A single pattern cannot solve every problem. [37, 39]
*   **Do not accept a design as absolute law.** Designs are tools used for team communication. Challenge assumptions to find critical edge cases. [58, 61]
*   **Do not give binary answers to difficult design requests.** Discuss tradeoffs in terms of time investments. Frame estimates as weeks of extra work. [73, 74]
