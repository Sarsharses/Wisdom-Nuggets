# Refactoring

- Whenever refactoring a URL (or anything else for that matter) you should take careful note of where that gets used. Oftentimes it's a great investment to take a minute checking that out. If you forget this it might come back at you eventually in places you didn't think of at the time.

# Requests

- Only use GET requests for getting (get it?) stuff from the back and POST or PUT for storing stuff. In some cases you might want to use DELETE instead of POST or PUT to signal the end of life for that specific record. GETs should never change the server state. The risk might be small but the damage can be huge.

# Routing

- When creating routes, always double-check if nothing shares a name. Things tend to break if two routes are called the same.
