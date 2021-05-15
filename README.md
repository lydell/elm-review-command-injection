# elm-review command injection

1. Clone this repo
2. `npm ci`
3. `npx elm-review --fix`

Result: 

elm-review offers to remove an unused variable. When you answer yes, elm-review keeps asking about the same fix. If you exit elm-review, you’ll notice that a file called `pwned` has been created (and also another Main.elm for some reason).

Expected:

elm-review applies the fix and exits.
