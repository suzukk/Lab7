# BUG-02: Total book count is incorrect when the list is empty

**Severity:** Medium  
**Area:** Statistics / UI

## Preconditions
- The application server is running.
- The application is open in a browser.

## Steps to reproduce
1. Open the book list.
2. Delete every book.
3. Observe the table and total book count.

## Actual result
The table is empty, but the total book count displays `1`.

## Expected result
The total book count should display `0`.

## Evidence
- `screenshots/bug-02-count.png`
