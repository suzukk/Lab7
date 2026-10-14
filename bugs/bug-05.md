# BUG-05: Duplicate books are accepted

**Severity:** Medium  
**Area:** Data integrity / UI

## Preconditions
- The application server is running.
- The book list is open in a browser.

## Steps to reproduce
1. Enter `Duplicate Test` as the title.
2. Enter `Tergel` as the author.
3. Enter `2020` as the year.
4. Click Add.
5. Enter the same title, author, and year again.
6. Click Add again.

## Actual result
Both identical books are added to the list.

## Expected result
The application should reject a duplicate book with the same title and author.

## Evidence
- Add a screenshot in `screenshots/` if captured.
