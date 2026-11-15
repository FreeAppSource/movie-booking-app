# Movie Booking App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Richard Yang** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `movie-booking-ui-richardyang.sketch` by **Richard Yang**: one route per artboard, with the artboard's layout, colours, images and text.

![Movie Booking App screens](./showcase.jpg)

## 📱 Screens (4 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **1** · start screen | `src/app/s-1.jsx` | 360 × 640 | 5 |
| 2 | **2** | `src/app/s-2.jsx` | 360 × 640 | 4 |
| 3 | **1.1** | `src/app/s-1-1.jsx` | 360 × 760 | 5 |
| 4 | **2.1** | `src/app/s-2-1.jsx` | 360 × 760 | 4 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Inter, Montserrat), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/movie-booking-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Movie Tickets and Booking App** design by **Richard Yang**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Richard Yang](https://www.sketchappsources.com/contributor/richardyang) |
| Original design | [Movie Tickets and Booking App](https://dribbble.com/shots/11378695-Android-Movie-Booking-Experiment) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4417-movie-booking-ui-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/richardyang> |
| Website | <https://origamiui.com/> |
| Original file | `movie-booking-ui-richardyang.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Movie Tickets and Booking App" by Richard Yang (https://dribbble.com/shots/11378695-Android-Movie-Booking-Experiment), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4417-movie-booking-ui-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
