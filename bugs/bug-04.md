# BUG-04: Non-numeric year is accepted

**Severity:** Medium  
**Area:** Input validation / UI

## Preconditions
- The application server is running.
- The book list is open in a browser.

## Steps to reproduce
1. Enter `Year Validation Test` as the title.
2. Enter `Tergel` as the author.
3. Enter `abc` as the year.
4. Click the Add button.

## Actual result
The application accepts the book with `abc` as its year.

## Expected result
The application should reject a non-numeric year and display a useful validation message.

## Evidence
- Add a screenshot in `screenshots/` if not already captured.
