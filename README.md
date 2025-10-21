# Personal Dashboard Browser Extension

A beautiful and functional browser extension that transforms your new tab page into a personalized dashboard featuring real-time data and stunning background images.

## Features

- **Dynamic Background Images**: Beautiful nature photos from Unsplash that change on each new tab
- **Real-time Clock**: Live updating time display
- **Cryptocurrency Tracker**: Current Dogecoin price with 24h high/low data
- **Weather Information**: Current weather conditions based on your location
- **Responsive Design**: Clean, modern interface that works on all screen sizes

## Screenshots

The dashboard displays:
- A stunning nature background image with photographer attribution
- Current time in the center
- Dogecoin cryptocurrency data (price, 24h high/low)
- Local weather information with weather icons

## Installation

### For Development

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd browser-dashboard-ext
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Build the extension:
   ```bash
   npm run build
   ```

4. Load the extension in Chrome:
   - Open Chrome and go to `chrome://extensions/`
   - Enable "Developer mode"
   - Click "Load unpacked" and select the project directory
   - The extension will now replace your new tab page

### For Production

1. Build the extension:
   ```bash
   npm run build
   ```

2. Package the extension for distribution through the Chrome Web Store

## Usage

Once installed, simply open a new tab in Chrome and you'll see your personalized dashboard with:
- A beautiful background image
- Current time
- Cryptocurrency data
- Weather information for your location

## API Dependencies

This extension uses the following APIs:
- **Unsplash API**: For background images
- **CoinGecko API**: For cryptocurrency data
- **OpenWeatherMap API**: For weather information
- **Browser Geolocation API**: For location-based weather

## Development

### Project Structure

```
browser-dashboard-ext/
├── index.html          # Main HTML structure
├── index.css           # Styling and layout
├── index.js            # JavaScript functionality
├── manifest.json       # Extension configuration
├── icon.png           # Extension icon
├── package.json       # Dependencies and scripts
└── vite.config.js     # Build configuration
```

### Key Components

- **Background Images**: Fetches random nature images from Unsplash
- **Time Display**: Updates every second using `setInterval`
- **Crypto Data**: Fetches Dogecoin price information from CoinGecko
- **Weather**: Uses geolocation to get local weather data

### Customization

You can easily modify:
- **Cryptocurrency**: Change the coin by updating the API endpoint in `index.js`
- **Background Images**: Modify the search query in the Unsplash API call
- **Styling**: Update `index.css` for different visual themes
- **Layout**: Modify the HTML structure in `index.html`

## Browser Compatibility

- Chrome (manifest v3)
- Chromium-based browsers (Edge, Brave, etc.)

## Permissions

This extension requires:
- `activeTab`: To override the new tab page
- Geolocation: To provide location-based weather data

## Privacy

- No personal data is stored
- Location is only used for weather data
- All API calls are made directly from your browser

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Background images provided by [Unsplash](https://unsplash.com)
- Cryptocurrency data from [CoinGecko](https://coingecko.com)
- Weather data from [OpenWeatherMap](https://openweathermap.org)
- Built as part of the Scrimba Full Stack Developer course