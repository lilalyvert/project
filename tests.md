# Test Cases

## Valid Input
- Enter all required fields
- Expected: User summary and researcher record are displayed

## Missing Fields
- Leave one or more required fields empty
- Expected: Form prevents submission or prompts user

## Stress Classification
- Input: "exam stress"
- Expected: Category = Academic

## Severity Range
- Input values from 1–5
- Expected: Accepted
- Input values outside range
- Expected: Rejected or handled

## Output Display
- Submit form
- Expected: Output appears clearly in the output section

## Local Storage (if implemented)
- Submit entry
- Refresh page
- Expected: Data persists
