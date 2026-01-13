# FilterGenie

FilterGenie is a browser extension that helps you kick off a more targeted LinkedIn job search from a simple popup. You type the kind of job you want, and FilterGenie uses the OpenAI API to suggest search filters and apply them on LinkedIn’s Jobs page.

> Formerly named **Slide-n-Seek** — this project has been renamed to **FilterGenie**.

---

## What it does

- **Popup UI input**: Click the extension icon and type the role you’re looking for (ex: “backend engineer new grad”).
- **AI-assisted filter suggestions**: Uses the OpenAI API to translate your text into structured job-search preferences.
- **LinkedIn Jobs integration**: Designed to work on LinkedIn’s job search experience without changing the page layout.

---

## How it works (high level)

1. You enter your desired role in the extension popup.
2. FilterGenie sends that text to the OpenAI API.
3. The extension interprets the response and applies the relevant filters/search actions on LinkedIn Jobs.

---

## Tech Stack

- JavaScript
- HTML / CSS
- Chrome Extension APIs (popup + content scripts)
- Webpack
- OpenAI API

---

## Installation (Local Development)

1. **Clone the repository**
   ```bash
   git clone https://github.com/TheRoadSurgeon/Filter-Genie.git
   cd Filter-Genie
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Create a `.env` file**
   In the project root, create a file named `.env` and add:
   ```env
   OPENAI_API_KEY="your_key_here"
   ```

4. **Build the extension**
   ```bash
   npm run build
   ```

5. **Load the extension in Chrome**
   - Open Chrome and go to `chrome://extensions/`
   - Enable **Developer mode** (top right)
   - Click **Load unpacked**
   - Select the **project folder** (the folder containing `manifest.json`)

6. **Use it**
   - Navigate to LinkedIn Jobs
   - Click the FilterGenie icon
   - Type the job you want and run the action

---

## Notes / Disclaimer

- This extension is intended for educational and hackathon/demo use.
- LinkedIn’s UI and behavior can change, which may require updates to selectors or automation logic.
- Be mindful of LinkedIn’s terms and automation policies when using browser automation tools.

---

## Credits

Built for **SparkHacks 2025**.

FilterGenie — search smarter, apply faster.
