## 🎬 **Obsidian DVD / Movie Collection Dashboard — Installation & Setup Guide**

This starter kit gives you a beautiful, interactive way to track your DVD/Blu-ray/movie collection inside Obsidian. It includes:

- **Movies/** — the folder where all your movie notes will be stored
- **Movie Collection - Dashboard** — browse, filter by genre/decade, search, toggle watched/unwatched, rate with stars, and more
- **Movie Collection - Add New Movie** — a simple form that creates new movie notes automatically

Everything runs on **DataviewJS** and core Obsidian features. No external scripts, no APIs, no complicated setup.

---

## 📁 Folder Contents

When you unzip the download, you’ll see:

```
Movies/   ← Folder where your movie notes will live
		2001 A Space Odysse.md   ← example movie
	Movie Collection - Add New Movie.md
	Movie Collection - Dashboard.md
	Readme.md
```

---

## 🎨 Theme and Appearance Settings to Match the Screenshots

These settings are optional, but they will make your vault look like the screenshots shown in this guide. They don’t affect functionality—only appearance and layout.

### **Theme**

The screenshots use the **Fancy A Story** theme with these style presets:

- **Board Game Dashboard:** _Art Deco — Light Silver_
- **Movie Dashboard:** _Art Deco — Dark Chocolate_

The dashboards work with any theme; these are just the ones used in the screenshots.

### **Appearance Settings**

These settings affect layout, spacing, and how clean the pages look:

- Appearance → Inline title → **Off**
- Editor → Readable line length → **Off**
- Editor → Properties in document → **Hidden**
- Core plugins → Page preview → **Off**

### **Editor Behavior**

These settings ensure the dashboard and forms open in the correct mode:

- Editor → Default view for new tabs → **Reading view**
- Editor → Default editing mode → **Source mode**

These match the environment used to create the screenshots and help the dashboards display cleanly and consistently.

---

## 🚀 Installation (2 minutes)

Follow these steps:

1. **Unzip the download.**
2. **Copy all three items into the root of your Obsidian vault** (the top level)
	You can skip copying the Readme.md if you’ve already read it or don’t need it in your vault.

```
Movies/   ← Folder where your movie notes will live
		2001 A Space Odysse.md   ← example movie
	Movie Collection - Add New Movie.md
	Movie Collection - Dashboard.md
```

3. Open Obsidian and make sure the plugin **Dataview** is installed and enabled.
    - Settings → Community Plugins → Browse → search “Dataview”
    - Install and enable **Dataview**
    - Settings → Dataview → **Enable JavaScript Queries** (very important — required for the form and dashboard to work)
4. Open **My Movie Dashboard** or **Add New Movie** and start using the system.

That’s it. No configuration, no renaming, no other plugins needed.

---

## 📝 How to Add a New Movie

1. Open **Add New Movie.md**
2. Fill out the form fields (title, year, director, poster URL, genres, synopsis, thoughts, etc.)
3. Click **➕ Create Movie Page**
4. A new note will appear inside the `Movies/` folder

Each note includes:
- Frontmatter (YAML) with all your data
- Poster image
- Sections for synopsis, thoughts/review, quotes, notes, and links

The dashboard reads everything automatically.

---

## 📊 Using the Dashboard

Open **My Movie Dashboard.md** to:

- Browse your entire collection
- Filter by genre or decade/year (including “TV Series”)
- Switch between Director and Actor(s) view
- Search by title or actor
- Toggle “Unwatched” to see only movies you haven’t watched yet
- Toggle “Show All” to see every movie without pagination
- Click **🎲 Surprise Me!** to open a random movie
- Check/uncheck “Watched” directly in the table (saves instantly)
- Click stars to rate 0–5 (saves instantly)
- Click posters to zoom in

The dashboard updates live as you add movies or change ratings/watched status.

---

## 🗂️ Customizing the System (Keep It Simple)

This kit is designed to be easy to use right away — and easy to tweak if you want.

**The safest & most common change: Rename the movies folder**  
If you’d rather call it “DVD Collection”, “Films”, “Media”, or anything else:

1. Open **Movie Collection - Add New Movie.md**  
   Find this line near the top:  
   const folder = "Movies";  
   Change "Movies" to your preferred name.

2. Open **Movie Collection - Dashboard.md**  
   Find this line:  
   const allMovies = dv.pages('"Movies"');  
   Change "Movies" to match exactly what you picked above.

3. (If you already added movies) Rename or move the “Movies” folder in your vault to the new name.

That’s all it takes — the form will save to the new location, and the dashboard will read from it.

**Want to do more?**  
You can safely edit labels, add/remove genres in the notes themselves, or experiment with the code. Everything is plain text — if something breaks, just replace the file from your backup. For bigger changes (like adding new fields), search online for “Obsidian Dataview frontmatter” or “DataviewJS tutorial” — there are tons of friendly guides.

---

## 🧩 Troubleshooting

**Dashboard is empty or form doesn’t work**  
- Make sure your movie notes are inside the `Movies/` folder  
- Make sure Dataview is enabled  
- Make sure **JavaScript Queries** are enabled in Dataview settings  

**Images not showing**  
- Check that your Poster URL is valid and ends in .jpg, .jpeg, .png, or .gif  
- Try a direct image link  

**Ratings or Watched status not saving**  
- Confirm JavaScript Queries are enabled  
- Make sure the note still has its frontmatter section at the top  

---

## 🎉 Enjoy Your Movie Collection Tracker

This system is designed to be simple, clean, and easy to extend. Track your DVDs, rate your favorites, rediscover old gems — all inside Obsidian.

Happy watching! 🍿