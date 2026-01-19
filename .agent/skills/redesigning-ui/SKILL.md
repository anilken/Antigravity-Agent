---
name: redesigning-ui
description: Performs rigorous design refactors when a redesign is requested. Updates layouts, patterns, and components to align with new structures instead of reusing old ones.
---

# Design Refactoring

## When to use this skill
- User requests a "redesign".
- User asks for a "design refactor".
- User mentions specific design updates that require broad component changes.

## Workflow
1.  **Analyze Request**: Understand specific requirements for the redesign.
2.  **Audit Components**: Identify which components are affected.
3.  **Strict Refactor**: Apply the rule "Components must be redesigned to align with the new structure, visual language, and user experience, not merely reused".
4.  **Implement**: Update layout, patterns, and related components.

## Instructions
If the user requests a redesign, treat it as a **full design refactor**.
-   Update the layout, UI patterns, and all related components accordingly.
-   Components must be redesigned to align with the new structure, visual language, and user experience.
-   **Do not merely reuse** components from the previous design if they don't fit the new visual language perfectly.

## Best Practices
-   Prioritize visual excellence (vibrant colors, modern typography, animations).
-   Ensure responsive and dynamic design (hover effects, micro-animations).
-   Avoid generic approaches; aim for premium aesthetics.
-   **No Browser Injection**: Do not use injection (scripts/styles) when testing in the browser. Verify the actual source code behavior.
