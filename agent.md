1. Purpose

This agent is responsible for generating and maintaining a minimal browser-based stress tracking application using only:

HTML
CSS
Vanilla JavaScript

The goal is to build a simple, functional, and easy-to-understand app that allows users to input stress-related information and receive structured outputs for both personal and research use.

2. Core Responsibilities

The agent must:

Generate a single-page web application
Implement:
One input form
One output display section
Process user input into:
A clean user-facing summary
A structured researcher-facing record
Ensure the app runs entirely in the browser (no backend)
3. Required User Inputs

The application must collect:

User name or ID
Main stressor
Stress severity (scale 1–5)
Coping strategies used
Short open-text emotional description
4. Required Outputs
4.1 User-Facing Output

Must:

Be short, clear, and supportive
Summarize the user’s input
Include:
Stress category
Severity level
Practical (non-clinical) feedback

Must NOT:

Provide medical, psychological, or diagnostic advice
Sound like therapy or counseling
4.2 Researcher-Facing Output

Must generate a structured object containing:

Timestamp
User name or ID
Stress category
Severity
Coping strategies
Original description

This can be:

Displayed on screen
Or stored in localStorage
5. Stress Classification Logic

The agent must classify the stressor into one of:

Academic
Social
Financial
Health
Other

Classification should be:

Keyword-based
Simple and transparent
Deterministic (same input → same output)
6. Technical Constraints

The agent MUST:

Use only:
HTML
CSS
Vanilla JavaScript
Avoid:
Frameworks (React, Vue, etc.)
External libraries (unless extremely minimal)
Backend systems
Databases
7. Storage Rules

The agent should choose ONE of:

Store entries in localStorage
OR display structured data without persistence

Do NOT:

Build authentication
Connect to APIs
Use external storage
8. UI & Design Principles

The interface must be:

Simple and readable
Clearly divided into:
Input section
Output section
Minimal styling (no over-design)
Easy to inspect in browser dev tools
9. Constraints (Critical)

The agent must:

Prioritize clarity over complexity
Keep logic easy to follow and inspect
Avoid overengineering
Avoid unnecessary features
Avoid vague or ambiguous outputs
10. Quality Standards

The generated app should:

Work immediately when opened in a browser
Have no console errors
Use clear variable names
Be logically organized
11. Non-Goals

The agent should NOT:

Build a full product
Add advanced UI/UX features
Include analytics or tracking
Simulate real psychological evaluation
Overcomplicate classification logic
12. Success Criteria

The app is successful if:

A user can input stress data
The app displays:
A clear summary
A categorized stress type
A structured record
Everything runs locally with no setup