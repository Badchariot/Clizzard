# Clizzard Arcade

A tiny arcade for browser games dreamed up with AI. Static site, hosted on GitHub Pages, served at clizzard.com.

## Structure
```
index.html                     the arcade landing page (the "floor")
games/<id>/index.html          one self-contained game per folder
CNAME                          custom domain for GitHub Pages
```

## Add a new game
1. Drop the game's self-contained folder at `games/<id>/` with an `index.html`.
2. Open `index.html`, find the `GAMES` list near the bottom, and add one entry:
   ```js
   {
     id:"my-game",
     title:"My Game",
     pts:"Subtitle",
     blurb:"One or two sentences about it.",
     path:"games/my-game/index.html",
     tags:["Tag","1P"],
     accent:"#23e5db",
     status:"live",
     art:"soon"        // or add custom art in the art() function
   }
   ```
3. Commit and push. GitHub Pages redeploys in ~1 minute.

Games flagged `status:"soon"` render as empty "coming soon" cabinets.

## Current cabinets
- **Sky Invaders** — first-person ground-gunner take on Space Invaders.
