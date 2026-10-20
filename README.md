# Gridiron Dynasty '09

A college football dynasty simulator that starts with the 2009 FBS season. Pick any of the 120 programs, recruit every week, set the depth chart, and sim through the BCS era, the four-team playoff (2014) and the twelve-team playoff (2024).

## Play it

Open `index.html` in a browser, or host it with GitHub Pages:

1. Create a new repository and upload `index.html`, `README.md` and the `samples` folder.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, and save.
4. After a minute your game is live at `https://<your-username>.github.io/<repo-name>/`. Add it to your phone's home screen to use it like an app.

## Saves

Saves are kept in the browser on that device (three slots). To move a dynasty to another device or back it up, use **More → Save & load → Download save file**, then **Import a save file** on the start screen.

## Uploading recruiting classes

Each season the game asks for the next year's class (the 2010 class while you play 2009). Go to **More → Upload recruits or rosters** and pick a CSV file. Only `name` and `position` are required:

```
name,position,stars,rating,rank,state,city,high_school,height,weight,juco,college
Ronald Powell,WDE,5,0.9999,1,CA,Moreno Valley,Rancho Verde,6-4,230,no,Florida
```

- Positions like OT, OG, DT, SDE, WDE, OLB, ILB, ATH, APB, PRO and DUAL map automatically.
- `rating` can be a 247-style composite (0.80–1.00) or a 0–100 score.
- `college` is where he signed in real life. It's shown on his profile; in your dynasty he can go anywhere.
- Uploaded recruits are mixed with generated ones so every school has a full pool to recruit from.

Roster files (`team,name,position,year,ovr`) can replace whole team rosters in the preseason. See `samples/`.

## Files

- `index.html` – the whole game in one file
- `icon.svg`, `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`, `manifest.webmanifest` – app icon for browser tabs and your phone's home screen
- `samples/recruits-2010.csv` – the real 2010 recruiting class (1,854 signees from 82 schools, 247Sports data)
- `samples/recruits-template.csv` – recruiting class layout
- `samples/rosters-template.csv` – roster layout
