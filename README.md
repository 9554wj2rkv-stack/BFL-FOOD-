<p align="center">
  <img src="logo.png" alt="Body Fuel Lab – Food Tracker logo" width="128" height="128">
</p>

<h1 align="center">Body Fuel Lab – Food Tracker</h1>

<p align="center">
  A simple, phone-first food tracker. It is the sister app to <b>Body Fuel Lab</b>.<br>
  The whole app is one HTML file. It works offline after the first load and keeps your data on your own phone.
</p>

---

## What it does

**Today**
- Shows the calories you have left and protein, carbs and fat against your daily target.
- Has one big "Log food or drink" button.
- "Again?" chips log your usual foods with one tap.
- Today's log is grouped by breakfast, lunch, dinner and snacks.
- Drinks count towards your fluids for the day.

**Foods**
- Search a built-in food list in English or Danish.
- Look up a product by its barcode number through Open Food Facts.
- Add your own foods from the values on a label.
- Mark foods as favourites.

**Teaspoons and tablespoons**
- Log ½ tsp, 1 tsp, ½ tbsp or 1 tbsp, and the app converts it to grams and calories.
- Weights for honey, olive oil, butter, mayonnaise and ghee come from USDA standard portions.
- For any other food, you weigh one tablespoon once and the app remembers it.

**Body Signals – My Food Detective**
- A food journal that takes about two minutes per entry. It answers seven questions: What did I eat? What happened? How did it affect me? Why did I eat it? Was it worth it? What was in it? Is it in or out for now?
- You can also mark "My body liked this", "Neutral / unsure" or "My body disliked this".
- History can be searched, filtered, edited and exported as a CSV file.
- Patterns appear after 5 entries and show how many observations each one is based on.

**Morning Body Check**
- "How do I feel today?" is a check-in that takes under a minute.
- It records symptoms with an optional strength, sleep, and optional details.
- You can link a food from the last 48 hours as a *suspected* association.
- Patterns can be viewed over 4 weeks, 3 months, 12 months or all time.
- There are no streaks, and skipped days are not counted.

**Notes**
- Free writing, saved on your phone.

**Me**
- Your plan: calories and macros for fat loss, maintenance or building muscle, worked out from your measurements, steps and workouts.
- Food profile: confirmed allergies always show a warning.
- Weekly weight trend.
- Appearance: **Light, Dark, Mint, Barbie** or System. Mint and Barbie match Body Fuel Lab.

> Body Signals and Morning Body Check are personal observations, not medical advice. The app never diagnoses allergies or intolerances, never claims a food caused a symptom, and never adds foods to an avoid list on its own.

---

## Files in this repository

| File | What it is |
|---|---|
| `index.html` | The whole app |
| `apple-touch-icon.png` | 180 × 180 home-screen icon for iPhone and iPad |
| `favicon.png` | Small browser-tab icon |
| `icon-192.png`, `icon-512.png` | App icons for Android and other browsers |
| `manifest.webmanifest` | App name and icons, so the app opens full-screen from the home screen |
| `logo.png`, `logo.svg` | The logo, for this README or anywhere else |
| `README.md` | This file |

All files sit in the top level of the repository, with no folders.

---

## Put it on GitHub Pages

1. On GitHub, click **New repository**. Name it, for example `bfl-food`, and choose **Public**. Free GitHub Pages needs a public repository.
2. Click **Add file → Upload files** and drag in every file listed above. Click **Commit changes**.
3. Go to **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then branch **main** and folder **/ (root)**. Click **Save**.
4. After a minute or two the app is live at:
   `https://YOUR-USERNAME.github.io/bfl-food/`

### Add it to your iPhone home screen

1. Open the link in **Safari**.
2. Tap **Share**, then **Add to Home Screen**.
3. The icon appears with the name **BFL Food** and opens full-screen like an app.

### Updating the app later

Upload the new `index.html` to the same repository; GitHub replaces the old one. Your logged data is not touched, because it lives on your phone, not on GitHub. If the old version still shows, close the app fully and open it again.

---

## Your data

- Everything is saved in the browser on your phone (`localStorage`). All keys start with `bflfood_`. The app never reads or changes Body Fuel Lab's data.
- Nothing is uploaded anywhere. The only outside connection is a barcode lookup, which asks Open Food Facts for that one product.
- **Important:** data belongs to one browser on one phone. If you clear Safari's website data or delete the home-screen app, your log goes with it.
- Use **Export CSV** in Body Signals → Food Detective and in Body Signals → Mornings to keep copies of your entries. On iPhone this opens the share sheet, so you can save the file to Files.

---

## Sources

- The built-in food list comes from Body Fuel Lab. The app never guesses missing values: if a value is unknown, it shows "n/a".
- Black coffee uses USDA FoodData Central, FDC 171890 (about 1 kcal per 100 ml).
- Spoon weights come from USDA FoodData Central standard portions.
- Barcode data comes from [Open Food Facts](https://world.openfoodfacts.org) (ODbL licence).

---

<p align="center"><sub>Body Fuel Lab – Food Tracker · sister app to Body Fuel Lab · made in Denmark</sub></p>
