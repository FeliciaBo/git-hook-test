**Setup:**

**1. Setup git to use the ".githooks" folder:**

git config --local core.hooksPath .githooks

**2. Test that it works:**

git config --local core.hooksPath .githooks

Expected: Should show message ".githooks"


**How to use:**

**1. Stage changes as usual (example using "file.js":**
git add file.js

**2. Commit the file:**
git commit -m "insert message that won't be seen here"

Expected: Commit will be stopped and show the error message 
"Error: "file.js" is empty. Remove it or add content before comitting"

If the commit works while the file is empty, the hook doesn't work...



