# BUG-01: Invalid JSON returns HTTP 200 instead of HTTP 400

**Severity:** Medium  
**Area:** API — `POST /api/books`

## Preconditions
- The application server is running at `http://localhost:3000`.

## Steps to reproduce
1. Send a POST request to `/api/books`.
2. Set `Content-Type: application/json`.
3. Use the invalid JSON body `буруу оролт`.

## Actual result
The server returns HTTP 200 OK with response body `{"result":"OK"}`.

## Expected result
The server should return HTTP 400 Bad Request for invalid JSON.

## Evidence
- `evidence/bug-api-curl.txt`
