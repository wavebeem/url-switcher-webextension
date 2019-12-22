- [x] Test removing CSP
- [x] Test redirecting URLs
- [ ] Check if document URL matches
- [x] Keep counts of redirected URLs per tab
- [ ] Show if CSP was disabled per tab
- [ ] Make a real icon for the toolbar that isn't bad
- [ ] Make a settings page (Vue.js?)
- [ ] Make a match/replace engine

Given we only get 4 characters in a badge, I think a symbol to show if CSP was disabled is sufficient, as well as a count of blocked files, capping at 99+

So it would look like `*99+` if CSP was off _and_ over 99 URLs had been redirected.

This way the user remembers if it's on, so they can turn off the extension when they're done.

We can use `setTitle` to display the long form explanation, like `123 URLs switched (CSP disabled)`