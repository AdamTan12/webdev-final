# Frontend

A pet matchmaking app built with vanilla HTML, CSS, and JavaScript.

## Pages

| File | Description |
|---|---|
| `index.html` | Login / Register |
| `create-pet.html` | Create a pet profile (onboarding) |
| `discover.html` | Swipe on other pets |
| `matches.html` | View matches and chat |
| `profile.html` | Edit your pet's profile |

## Structure

```
index.html
create-pet.html
discover.html
matches.html
profile.html
css/
    base.css
    auth.css
    create-pet.css
    discover.css
    matches.css
    profile.css
js/
    store.js
    api.js
    auth.js
    create-pet.js
    discover.js
    matches.js
    profile.js
```

## API

The frontend talks to the backend via `js/api.js`. The base URL is set at the top of that file:

```js
const API_URL = "https://481-backend-production.up.railway.app";
```

Change this to `http://localhost:8000` to point at a local backend instance.

## Walkthrough

1. **Register** - create an account on the login page.
2. **Create a pet** - you'll be redirected to the pet creation flow automatically.
3. **Discover** - swipe right to like, left to pass. A match popup appears on mutual likes.
4. **Matches** - view all matches and open a chat with any of them.
5. **Profile** - edit your pet's details, add/remove photos and tags, or sign out.
