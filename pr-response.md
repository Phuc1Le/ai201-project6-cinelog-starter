# PR Response Doc — CineLog Watchlist Feature

## AI Usage
<!-- Fill in at the end — how you used AI tools during this project -->

## Comment 1 — Rename
**What I did:**
I renamed save_to_watchlist() to add_to_watchlist() in services/watchlist_service.py and update all call sites
**How I verified:**
I checked if there was any other function calls of save_to_watchlist() in the project and made sure there is none.
## Comment 2 — Deduplication
**What I did:**
I added deduplication logic in add_to_watchlist() by checking if the film is already in the user's watchlist before adding it.
**How I verified:**
I ran the app and tested the "watchlist/<user_id>/add" endpoint with an existing film. I also included it in the test_watchlist.py file.

## Comment 3 — Missing test
**What I did:**
I wrote the new test_collection.py file, following the test_collection.py file, but only with the first 3 tests (adding, deduplicating, nonexisting)
**How I verified:**
I ran the test file and confirm it worked.

## Comment 4 — Default visibility
**My position:**
**Reasoning:**
**Tradeoff acknowledged:**

## Comment 5 — Sort order
**My position:**
**Reasoning:**
**Engagement with reviewer's point:**

## Comment 6 — Rebase
**What conflicted:**
**How I resolved it:**
**How I verified no conflict remains:**

## PR Description
<!-- Written at the end — feature overview, design decisions, manual testing steps -->