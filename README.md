# VerifySearchResults
Created Test Case to verify URL was correct and started a search for a specific text.

Verified the following criteria:
1. Verify that search on PHP.net for "eval" is going to the right place.
2. Verify that the "eval" page warns the user they really shouldn't use
the function.

Goals
1. Change the user agent to match one from Chrome 60.
2. Visit http://www.php.net
3. Use the search box to search for "eval" and submit.
4. Verify that the browser was redirected to
http://php.net/manual/en/function.eval.php
5. Verify that there is atleast one "Caution" message on the page.
