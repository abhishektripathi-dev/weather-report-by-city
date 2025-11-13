# Weather App by Abhishek Tripathi

A small, client-side weather lookup app that fetches current weather by city using the OpenWeatherMap API.

**Status:** Live demo deployed on Netlify (see Live Demo below). Replace the API key before publishing code.

**Live Demo**

- Deployed site: https://weather-report-by-city-name.netlify.app/

**Contents:**
- `index.html` : Main UI and JavaScript for fetching weather data.
- `style.css` : Styles for the app.
- `images/` : Weather and UI icons used by the app.

**Features**
- Search weather by city name.
- Displays temperature (°C), humidity, wind speed, and an icon representing weather.

**Quick Start**

1. Get an OpenWeatherMap API key:
   - Sign up at https://openweathermap.org/ and obtain a free API key.

2. Add your API key to the project:
   - Open `index.html` and find the line:

```js
const apiKey = ""
```

   - Replace the value with your own API key, for example:

```js
const apiKey = "YOUR_API_KEY_HERE"
```

   - Important: Do not commit private API keys to public repositories. For client-side apps the key is visible in the browser — consider using a server-side proxy if you need to keep the key secret.

3. Run the app locally:
   - The easiest way is to open `index.html` in your browser directly.
   - For a simple local server (recommended for consistent behavior), run one of the commands below from the project root:

```bash
# Python 3 built-in server
python -m http.server 8000

# If you have Node.js installed, you can use 'serve' (install with `npm i -g serve`)
serve . -l 5000
```

   - Then open `http://localhost:8000` (or the port you chose) in your browser.

4. Use the app:
   - Type a city name in the search box and click the search button.
   - The app will show current temperature, humidity, wind speed and a weather icon.

**Deployment (Netlify)**

- Quick deploy: Drag-and-drop the project folder to Netlify Drop (https://app.netlify.com/drop) or connect your GitHub repo and enable continuous deploy.
- Netlify environment variables: If you want to avoid committing keys, set a variable like `OPENWEATHER_API_KEY` in Netlify's Site settings and use a build step to inject it into the client files. Note: a simple static client will still expose the key to users; to fully protect a key, use a server-side API proxy.
- Netlify docs: https://docs.netlify.com/

**Files to check**
- `index.html` — Update `apiKey` and optionally tweak UI text or placeholders.
- `style.css` — Modify styling.
- `images/` — Add or replace icon images used by the app.

**Troubleshooting**
- If nothing appears after searching, open the browser DevTools console (F12) to see any API or JS errors.
- Ensure your API key is valid and that you are not exceeding the OpenWeatherMap free tier limits.

**Contribution & License**
- Feel free to open issues or submit pull requests to improve the UI or add features (e.g., search suggestions, forecasts).
- This repository does not include a license file. Add one if you intend to open-source it. A common choice is the MIT license.

