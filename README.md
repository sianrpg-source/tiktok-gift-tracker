# 🎁 TikTok Live Gift Tracker

A beautiful, real-time gift tracking dashboard for TikTok live streams. Perfect for streamers who want to monitor gifts, track top contributors, and engage with their audience.

## ✨ Features

- **Real-time Gift Tracking**: Instantly see gifts as they come in during your live stream
- **Beautiful Animated Interface**: Modern glassmorphic design with floating emojis and smooth animations
- **Comprehensive Statistics**: Track total gifts, coin value, top gifters, and session time
- **WebSocket Connection**: Connect to TikTok live stream via WebSocket API
- **Mobile Responsive**: Works perfectly on desktop and mobile devices
- **Live Session Timer**: Track how long your streaming session has been active
- **Gift History**: See the last 50 gifts with sender details and timestamps

## 🚀 Quick Start

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/tiktok-gift-tracker.git
   cd tiktok-gift-tracker
   ```

2. **Open the tracker**:
   - Simply open `index.html` in your web browser
   - Or serve it using a local web server:
     ```bash
     python -m http.server 8000
     # Then visit http://localhost:8000
     ```

3. **Configure your connection**:
   - Enter your WebSocket server URL (default: `ws://localhost:3005/ws`)
   - Enter your API key
   - Click "Connect to Stream"

## 🔧 Configuration

### WebSocket Server
You'll need a TikTok Live WebSocket server that provides gift events. The tracker expects messages in this format:

```json
{
  "type": "tiktok_event",
  "name": "GiftEvent",
  "data": {
    "gift": {
      "name": "Rose",
      "id": 5655,
      "diamond_cost": 1
    },
    "user": {
      "nickname": "username",
      "unique_id": "uniqueid"
    },
    "count": 5
  }
}
```

### Connection Parameters
- **Server URL**: Your WebSocket server endpoint
- **API Key**: Authentication key for your WebSocket server
- **Unique ID**: The TikTok username to track (currently set to "sebsshoprblx")

## 📱 Usage

1. **Start Your Stream**: Begin your TikTok live stream
2. **Connect the Tracker**: Enter your server details and click connect
3. **Monitor in Real-time**: Watch as gifts appear instantly with beautiful animations
4. **Track Your Stats**: Monitor total gifts, earnings, and top contributors
5. **Engage Your Audience**: Use the information to thank top gifters and engage viewers

## 🎨 Interface Overview

### Header Section
- **Connection Status**: Shows if you're connected to the live stream
- **Connection Form**: Input fields for server URL and API key
- **Control Buttons**: Connect/disconnect and clear data buttons

### Statistics Dashboard
- **Total Gifts**: Count of all gifts received
- **Total Coins**: Total diamond/coin value of all gifts
- **Top Gifter**: The user who has sent the most valuable gifts
- **Session Time**: How long you've been connected to the stream

### Gift Feed
- **Real-time Updates**: New gifts appear instantly at the top
- **Gift Details**: Shows gift name, sender, count, value, and timestamp
- **Animated Entries**: Each gift slides in with smooth animations
- **Limited History**: Keeps the last 50 gifts to maintain performance

## 🛠️ Technical Details

### Built With
- **HTML5**: Structure and semantic markup
- **CSS3**: Modern styling with gradients, animations, and glassmorphism
- **Vanilla JavaScript**: Real-time WebSocket handling and DOM manipulation
- **WebSocket API**: Real-time connection to TikTok live stream data

### Browser Support
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Performance Features
- **Efficient DOM Updates**: Only updates changed elements
- **Memory Management**: Automatically limits gift history to 50 items
- **Optimized Animations**: Uses CSS transforms for smooth 60fps animations
- **Responsive Design**: Adapts to any screen size

## 🎭 Customization

### Changing the Streamer
To track a different TikTok user, modify line 298 in the JavaScript:
```javascript
const wsUrl = `${serverUrl}?unique_id=YOUR_USERNAME&api_key=${apiKey}`;
```

### Styling
The interface uses CSS custom properties. You can easily customize colors by modifying the gradient and color values in the CSS section.

### Gift Limit
To change the number of gifts stored in memory, modify line 369:
```javascript
if (this.gifts.length > 50) {  // Change 50 to your desired limit
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This tool is for educational and personal use only. Make sure you comply with TikTok's Terms of Service and API usage policies. The developers are not responsible for any violations or misuse of this software.

## 🙋‍♂️ Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/yourusername/tiktok-gift-tracker/issues) page
2. Create a new issue with detailed information about your problem
3. Include your browser version and console errors if applicable

## 🌟 Show Your Support

If this project helped you, please consider:
- ⭐ Starring the repository
- 🍴 Forking it to contribute
- 📢 Sharing it with other streamers

---

**Made with ❤️ for the TikTok streaming community**
