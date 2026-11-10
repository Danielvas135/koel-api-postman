# Koel API Postman Collection

Postman collection for testing the Koel music player API (https://qa.koel.app).

## Overview
This collection covers core API endpoints used during a QA Automation internship, including authentication, song information, play count, recently played songs, and like/unlike functionality.

Tests include positive cases, negative cases (missing token, invalid data, wrong method), and checks against the API documentation.

## What’s Included
- Login / authentication
- Get song info
- Increase play count
- Get recently played songs
- Like / Unlike multiple songs (batch endpoints)
- Negative and edge cases for each

## How to Use
1. Import the collection JSON into Postman.
2. Set up an environment with:
   - `baseURL` = `https://qa.koel.app`
   - Valid credentials
3. Run the collection or individual requests.
4. Review the Tests tab for assertions.

## Bugs Found
- Batch like endpoint returned 204 No Content instead of the documented 200 OK with response body.
- Requests with missing or invalid auth token returned an HTML error page instead of a 401 Unauthorized JSON response.
- Requesting a non-existent song ID returned 204 instead of 404 Not Found.

## Notes
- Collection file: `API Koel.postman_collection (2).json` (consider renaming to `koel-api.postman_collection.json`)
- Tests follow the acceptance criteria from the internship user stories.
- Bugs were logged in Jira with steps, expected vs actual results, and screenshots.

## Author
Daniel Vasquez  
QA Tester transitioning to automation
