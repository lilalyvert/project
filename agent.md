## Purpose

This agent is responsible for generating and maintaining a minimal browser-based stress tracking application using only:

HTML
CSS
Vanilla JavaScript

The goal is to build a simple, functional, and easy-to-understand app that allows users to input stress-related information and receive structured outputs for both personal and research use.

## Core Responsibilities

The agent must:

Generate a single-page web application
Implement:
One input form
One output display section
Process user input into:
A clean user-facing summary
A structured researcher-facing record
Ensure the app runs entirely in the browser (no backend)
## Required User Inputs

The application must collect:

User name or ID
Main stressor
Stress severity (scale 1–5)
Coping strategies used
Short open-text emotional description
## Required Outputs
## User-Facing Output

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
## Researcher-Facing Output

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
## Stress Classification Logic

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
## Technical Constraints

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
## Storage Rules

The agent should choose ONE of:

Store entries in localStorage
OR display structured data without persistence

Do NOT:

Build authentication
Connect to APIs
Use external storage
## UI & Design Principles

The interface must be:

Simple and readable
Clearly divided into:
Input section
Output section
Minimal styling (no over-design)
Easy to inspect in browser dev tools
## Constraints (Critical)

The agent must:

Prioritize clarity over complexity
Keep logic easy to follow and inspect
Avoid overengineering
Avoid unnecessary features
Avoid vague or ambiguous outputs
## Quality Standards

The generated app should:

Work immediately when opened in a browser
Have no console errors
Use clear variable names
Be logically organized
## Non-Goals

The agent should NOT:

Build a full product
Add advanced UI/UX features
Include analytics or tracking
Simulate real psychological evaluation
Overcomplicate classification logic
## Success Criteria

The app is successful if:

A user can input stress data
The app displays:
A clear summary
A categorized stress type
A structured record
Everything runs locally with no setup13. Permissions

The agent is allowed to:

Generate and modify HTML, CSS, and JavaScript files
Read and process user input from the form
Classify stressors using predefined logic
Create structured outputs for display
Store and retrieve data using browser localStorage (if implemented)

The agent must NOT:

Access external APIs
Send or receive data over the internet
Store data outside the browser environment
Execute system-level commands
Modify files outside the project scope
## Functional Requirements

The agent must ensure:

The application runs fully in a browser with no setup
All user inputs are captured correctly
A stress category is always assigned
Outputs are generated immediately after submission
No runtime errors occur in the browser console
## Behavioral Constraints

The agent must:

Be deterministic where possible (same input → same output)
Use simple, explainable logic
Avoid vague or inconsistent classifications
Keep responses concise and structured

The agent must NOT:

Guess missing data
Produce random or inconsistent outputs
Overcomplicate logic or introduce unnecessary abstraction
## Safety & Ethical Constraints

The agent must:

Avoid medical or psychological diagnosis
Avoid giving therapeutic or clinical advice
Keep feedback supportive but neutral
Respect user input without judgment

The agent must NOT:

Label users with conditions
Provide crisis or mental health treatment guidance
Make assumptions about the user’s identity or situation
## Error Handling

The agent should:

Handle empty or missing inputs gracefully
Prompt the user to complete required fields
Prevent submission if critical fields are missing

The agent must NOT:

Crash or break the UI
Display raw errors to the user
## Output Quality Standards

All outputs must be:

Clear and readable
Logically structured
Free of unnecessary technical jargon (for user-facing output)
Consistent in format across submissions
## Scope Limitations

This agent is intentionally limited to:

A single-page application
Local execution only
Basic stress classification

The agent will NOT:

Scale to multi-user systems
Store long-term datasets externally
Perform advanced analytics or predictions
## Determinism & Predictability

The agent should produce consistent outputs for the same inputs and avoid randomness unless explicitly required.
