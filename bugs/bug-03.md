# BUG-03: Book can be added with all required fields empty

**Severity:** Medium  
**Area:** Input validation / UI

## Preconditions
- The application server is running.
- The book list is open in a browser.

## Steps to reproduce
1. Leave the title field empty.
2. Leave the author field empty.
3. Leave the year field empty.
4. Click the Add button.

## Actual result
A book with empty fields is added to the list.

## Expected result
The application should reject the submission and display a useful validation message requiring the title, author, and year.

## Evidence
- Screenshot: `screenshots/bug-03-empty-fields.png` (if captured)
