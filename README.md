# Koel API Postman Collection

Postman collection for testing the Koel music player API (https://qa.koel.app).

## Overview
This collection covers core API endpoints used during a QA Automation internship, including authentication, song information, play count, recently played songs, and like/unlike functionality.

Tests include positive cases, negative cases (missing token, invalid data, wrong method), and checks against the API documentation. Several real bugs were found and reported (incorrect status codes, auth responses, non-existent resource handling, etc.).

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

## Notes
- Collection file: `API Koel.postman_collection (2).json`
- Tests follow the acceptance criteria from the internship user stories.
- Bugs found during execution were logged in Jira with steps, expected vs actual results, and screenshots.

## Author
Daniel Vasquez  
QA Automation Engineer
