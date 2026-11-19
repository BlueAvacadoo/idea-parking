# Idea Parking

A playful idea storage box where every idea is a car. Park your best ideas in a six-spot lot, return them to your collection when you need to rethink them, and sell them when they're done (or when you've decided to let them go).

## Features

- **Create ideas as cars**: name and describe each idea, then customize its body shape, colour, and up to 3 emoji stickers with a live preview.
- **Collection**: every idea you've created lives here until you park it.
- **Parking lot**: six numbered spots. Park up to six ideas at once. When the lot is full, parking is blocked until a spot frees up.
- **Two ways to sell**:
  - **Sell (completed)** from the lot: the idea was executed.
  - **Sell (never executed)** from the collection: the idea didn't make it.
- **Stats panel**: tracks ideas in the collection, cars parked, total lot changes (broken down by parked, returned, and sold), and sales by type.
- **Shift tracking**: each car records how many times it has moved between the collection and the lot.
- **Archive**: sold ideas are kept with their car appearance, sale type, and date.
- **Backup**: export and import all data as JSON.
- **Offline-friendly**: a single HTML file with no dependencies. Data is saved in your browser's `localStorage`.

## Demo

Once deployed, your app will be available at:

```
https://<your-username>.github.io/<repo-name>/
```

## Getting Started

### Run locally

No build step is needed. Either:

1. Double-click `index.html` to open it in your browser, or
2. Serve the folder with any static server, for example:
   ```bash
   npx serve .
   # or
   python -m http.server 8000
   ```

### Deploy to GitHub Pages

1. Create a new repository on GitHub (for example, `idea-parking`).
2. Upload `index.html` (and this `README.md`) to the repository's main branch.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose the **main** branch and the **/ (root)** folder, then save.
5. Wait a minute or two, then open the URL GitHub shows on the Pages settings page.

## Usage

| Action | How |
| --- | --- |
| Add an idea | Click **Add Idea**, fill in the name, description, shape, colour, and stickers, then save. |
| Edit an idea | Click its car in the collection or lot, then edit in the detail panel. |
| Park an idea | Select a car in the collection and click **Park** (or click an empty spot). |
| Return to collection | Open a parked car and click **Return to collection**. Its shift count is kept. |
| Sell from collection | Open a collection car and click **Sell (never executed)**. |
| Sell from lot | Open a parked car and click **Sell (completed)**. |
| Delete an idea | Open the idea and click **Delete**. Deleting is not counted as a sale. |
| Back up data | Use **Export** to save a JSON file, and **Import** to restore it. |
| Reset | Use **Reset all data** and confirm. This cannot be undone. |

## Data and Privacy

All data is stored locally in your browser's `localStorage`. Nothing is sent to a server. This means:

- Data is **per browser and per device**. Use Export/Import to move it between devices.
- Clearing your browser's site data will erase your ideas. Export regularly if you want a backup.

## Project Structure

```
idea-parking/
├── index.html   # The entire app (HTML, CSS, and JavaScript)
└── README.md    # This file
```

## Keyboard Accessibility

All buttons and interactive cars can be reached with the Tab key and activated with Enter or Space. Focus outlines are visible throughout.

## Browser Support

Any modern browser with ES6 and `localStorage` support, including recent versions of Chrome, Firefox, Safari, and Edge.

## Customizing

Predefined car options live at the top of the script in `index.html`:

- **Shapes**: Sedan, Hatchback, Coupe, SUV, Pickup, Convertible, Van
- **Colours**: Red, Blue, Green, Yellow, Black, White, Purple, Orange
- **Stickers**: 💡 🚀 🎨 🔧 📚 🌱 🎵 ⭐ 🔥 🧩 🏆 🌍

Edit these lists to change the options available to you.

## License

Add your preferred license here (for example, MIT).
