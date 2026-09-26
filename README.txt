# Personal Fitness Dashboard v3

## What's new
- Editable current diet: calories, protein, carbs, fat, meals.
- Editable current workout program: exercises, sets, rep ranges, RIR and rest.
- Historical dated logs are kept separately from current plan settings.
- Same localStorage key as the previous version for continuity.
- Automatic local backup before imports/writes.
- Backup/Restore + JSON export/import.
- PWA/offline assets included.

## iPhone
Keep this app at the SAME GitHub Pages URL. Replace the repository files with this version.
Then open Safari and refresh the site / installed Home Screen app.

## Important
localStorage belongs to the browser + exact website origin. Moving the app to a different URL/domain can create a separate storage area. Export a JSON backup before moving URLs or making major changes.

Future versions should preserve:
sid_fitness_dashboard_v1
and migrate the data object rather than replacing it.
