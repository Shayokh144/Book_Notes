# Chapter 2 Planning Guidelines: Turning a Briefing Into a Strong Plan

This guide outlines key practices for mobile engineers when translating feature designs and briefings into robust development plans, based on Chapter 2 of *Mobile System Design: Resourceful Engineering*.

## Should Do

*   **Understand the problem deeply before you start writing any code.** Uncover hidden requirements early to prevent costly rewrites later. For example, ask if recurring tasks reset daily or weekly. [42]
*   **Sketch a technical landscape diagram early in your planning.** Map out all required components and domains as nodes. For example, mark unresolved dependencies with dashed outlines. [36, 42]
*   **Align early with backend developers on critical system integrations.** For example, discuss session timeouts and local login token retrieval. Also, negotiate consolidated network calls to support multiple platforms. [81, 83, 85]
*   **Request a worst-case scenario layout with poor content early on.** Verify how the screen holds up with very ugly data. For example, support extremely long labels and right-to-left text. [60]
*   **Identify pre-existing codebase components before writing any new code.** Ask your team if shared UI primitives are already available. For example, reuse an existing generic thumbnail and description view. [64, 65]

## Should Not Do

*   **Do not begin implementation by coding the UI right away.** Starting with visuals causes you to think too locally. For example, you might overlook critical backend authentication timeouts. [30, 31]
*   **Do not get bogged down in minor details.** Focus your energy on high-level system structures first. For example, defer adding custom drop shadows and animations. [40, 41]
*   **Avoid choosing a specific UI architecture too early.** Do not let a rigid pattern lock your app down. For example, do not force reactive programming onto simple screens. [37, 39]
*   **Do not accept a high-fidelity design as absolute law.** Use designs as communication tools to collaborate with your team. For example, challenge assumptions about a missing tablet layout. [58, 61]
*   **Avoid giving simple binary answers to difficult design requests.** Discuss consequences and alternatives in terms of time investments. For example, quantify a custom navigation bar as extra weeks. [73, 74]
