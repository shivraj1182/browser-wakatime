# browser-wakatime

Automatic time tracking for stats about your website debugging, research, documentation, etc.

Note: Activity from this browser extension will not display on leaderboards, so installing this extension may lower your rank.

## Installation

1. Install the extension:

[![Chrome](https://wakatime.com/static/img/chrome-web-store.png)](https://chrome.google.com/webstore/detail/wakatime/jnbbnacmeggbgdjgaoojpmhdlkkpblgi)

[![Firefox](https://wakatime.com/static/img/firefox-addon.png)](https://addons.mozilla.org/en-US/firefox/addon/wakatimes/)

[![Edge](https://wakatime.com/static/img/microsoft-extension.png)](https://microsoftedge.microsoft.com/addons/detail/wakatime/cdnpfnaadjmaplhghnlonephmabegadl)

2. Login to [WakaTime](https://wakatime.com/).

3. Use your browser like you normally do and your time will be tracked for you automatically.

4. Visit https://wakatime.com to see your logged time.

5. Use in conjunction with [other WakaTime plugins](https://wakatime.com/plugins).

6. ## Manual Installation in VS Code

To manually install the updated browser-wakatime extension in VS Code for enhanced activity tracking with dynamic stats display:

1. **Clone or Download the Repository:**
   ```
   git clone https://github.com/shivraj1182/browser-wakatime.git
   cd browser-wakatime
   ```

2. **Install Dependencies:**
   ```
   npm install --include=dev
   ```

3. **Build the Extension:**
   ```
   npm run build
   ```

4. **Load in Browser:**
   - **Chrome**: Go to `chrome://extensions`, enable "Developer mode", click "Load unpacked", and select the `dist` folder from this repository.
   - **Firefox**: Go to `about:debugging#/runtime/this-firefox`, click "Load Temporary Add-on", and select the `dist/manifest.json` file.
   - **Edge**: Go to `edge://extensions`, enable "Developer mode", click "Load unpacked", and select the `dist` folder.

5. **Access the Stats Display:**
   - Click the WakaTime extension icon in your browser toolbar
   - The popup will display your activity stats with the dynamic `statsDiv` component
   - Stats will update automatically as you browse

6. **Integration with VS Code:**
   - Install the official [WakaTime VS Code Extension](https://marketplace.visualstudio.com/items?itemName=WakaTime.vscode-wakatime) from the VS Code marketplace
   - This browser extension tracks browsing activity while the VS Code extension tracks your coding time
   - Both data sources are combined in your WakaTime dashboard

## Screenshots

![SC open](./screenshots/sc_6-green.png)

![SC open](./screenshots/sc_6-open.png)

## Development instructions

```
npm i --include=dev
npm run dev
```

Run tests:

```
npm test
```

### Troubleshooting

Check for errors by inspecting the extension.

![inspecting extension](./screenshots/wakatime-chrome-debug.gif)

The extension is going through a refactor, the new build [instructions are here](./DEVELOPMENT.md)
