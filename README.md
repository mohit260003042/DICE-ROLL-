# Dice Roll App

A simple, responsive dice-rolling web app built with **HTML, CSS, and JavaScript**. Choose how many dice to roll, watch them animate, see the total, and review your recent rolls.

## Features

- Roll between **1 and 6 dice** at a time.
- Animated dice rolling effect.
- Displays each die with a familiar 1–6 pip pattern.
- Highlights the single-dot face in red.
- Calculates and displays the total when rolling multiple dice.
- Keeps a history of the **last 10 rolls**.
- Saves roll history in the browser using `localStorage`, so it can remain available after refreshing or reopening the page.
- Clear the saved roll history with one click.
- Responsive layout for smaller screens.
- Respects the device's reduced-motion preference for the landing animation.
- Supports dark styling and a light color scheme based on the device preference.

## Project Files

```text
.
├── index.html   # Page structure and controls
├── style.css    # Layout, colors, dice appearance, and animations
├── script.js    # Dice logic, animation, totals, and roll history
└── README.md    # Project documentation
```

## Run Locally

No installation or build tools are required.

1. Download or clone this project.
2. Keep `index.html`, `style.css`, and `script.js` in the same folder.
3. Open `index.html` in a modern web browser.
4. Choose the number of dice and click **Roll dice**.

## How It Works

1. JavaScript generates a random value from **1 to 6** for each die.
2. The app animates changing dice faces for about two seconds.
3. It generates the final result and calculates the sum.
4. The result is shown on screen and added to the history list.
5. The most recent 10 rolls are saved in `localStorage`.
6. **Clear history** removes the saved history from the browser.

## Technologies Used

- **HTML5** — page structure and controls
- **CSS3** — responsive styling, dice layout, glow effects, and animations
- **JavaScript** — random rolls, event handling, totals, animation, and browser storage

## Notes

- Roll results are generated with JavaScript's `Math.random()`. This is suitable for a casual dice game, but it is not intended for cryptographic or security-sensitive randomness.
- Roll history is stored locally in the current browser. It is not synced across devices.
- If browser storage is unavailable, the app is designed to continue running, but history may not persist.

## License

No license has been specified for this project. Add a license file if you want to define how others may use, modify, or distribute it.
