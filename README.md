# DevOps_ManualTestingLab

A small login application used for a manual testing lab in a DevOps workflow.

## Application

A single-page login form (`index.html`) built with plain HTML, CSS and JavaScript. No server or build step is needed.

**Test user:** `admin` / `Pass@123`

## Run locally

1. Clone the repository.
2. Open `index.html` in any browser.

## Functional requirements

| ID | Requirement |
|---|---|
| FR01 | A user with valid credentials can log in and is shown the dashboard with a welcome message. |
| FR02 | A login with a wrong password or unknown username shows the error "Invalid username or password." |
| FR03 | Submitting empty fields shows a message saying the field is required. |
| FR04 | The Show/Hide button reveals and re-masks the password. |
| FR05 | After 3 consecutive failed logins the account is locked and further attempts are refused. |
| FR06 | Logging out returns the user to the login page and ends the session. |

## Lab workflow

1. Test cases are written from the requirements above (`test-cases` file).
2. Each test case is executed manually against the running app.
3. Every failed test case is logged as a GitHub Issue, linked to its Test Case ID.
4. Fixes are committed and the failed cases are re-tested.
