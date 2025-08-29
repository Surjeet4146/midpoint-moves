# Midpoint Moves - TradingView Pine Script Indicator

A dynamic support and resistance indicator that identifies key price levels based on streak midpoints and provides real-time target levels for trading decisions.

## 🚀 Features

- **Dynamic Support & Resistance**: Automatically calculates and displays support and resistance levels based on price streaks
- **Midpoint Calculation**: Creates horizontal lines at the midpoint between high and low ranges during price streaks
- **Real-time Labels**: Shows exact price values for the next key levels
- **Customizable Display**: Toggle visibility of different line types and customize colors
- **Performance Optimized**: Manages line objects efficiently with automatic cleanup
- **Multi-timeframe Ready**: Works across all timeframes

## 📊 How It Works

The indicator analyzes consecutive up/down bars (streaks) and:

1. **Detects Streak Ends**: Identifies when a series of up or down bars ends
2. **Calculates Midpoints**: Finds the midpoint between the highest high and lowest low during each streak
3. **Creates Dynamic Lines**: Draws horizontal support/resistance lines at these midpoints
4. **Updates Status**: Highlights the next key level to watch and removes broken levels
5. **Provides Midpoint**: Shows the middle point between current support and resistance

## 🔧 Installation

### Method 1: Copy & Paste
1. Open TradingView and go to Pine Editor
2. Create a new indicator
3. Copy the entire code from `midpoint_moves.pine`
4. Paste it into the editor
5. Click "Add to Chart"

### Method 2: Import from GitHub
1. Download the `midpoint_moves.pine` file
2. In TradingView Pine Editor, use the import function
3. Upload the downloaded file

## ⚙️ Settings

| Setting | Description | Default |
|---------|-------------|---------|
| **Next Level Line Color** | Color for the active target level | White (75% opacity) |
| **Show all active levels** | Toggle to show/hide non-target levels | Enabled |
| **Other Active Line Color** | Color for non-target active levels | White (25% opacity) |

## 📈 Visual Elements

### Lines
- **Solid White Lines**: Active support/resistance levels
- **Highlighted Line**: Next key level to watch (thicker, brighter)
- **Dotted Gray Lines**: Broken/historical levels
- **Dashed Line**: Midpoint between current support and resistance

### Labels
- **Price Labels**: Show exact values for next support/resistance levels
- **Info Table**: Displays current timeframe and number of active levels

## 🎯 Trading Applications

### Breakout Trading
- Watch for price breaks above resistance or below support
- Use the midpoint line as a potential reversal area

### Range Trading
- Trade between support and resistance levels
- Use labels for precise entry/exit points

### Target Setting
- Next level labels provide clear profit targets
- Midpoint serves as partial profit area

## 🔍 Technical Details

- **Max Lines**: 500 (configurable via max_lines_count)
- **Array Management**: Automatically limits to 20 active levels per direction
- **Memory Optimization**: Cleans up old lines to prevent memory issues
- **Bar Detection**: Uses close vs open comparison for streak identification

## 📋 Code Structure

```
midpoint_moves.pine
├── Input Settings
├── Variables & Arrays
├── Bar Detection Logic
├── Streak End Detection
├── Line Creation & Management
├── Support/Resistance Processing
├── Label Management
└── Info Display
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for:

- Bug fixes
- Performance improvements
- New features
- Documentation updates

### Development Setup
1. Fork this repository
2. Create a feature branch
3. Test changes on TradingView
4. Submit a pull request

## 📝 License

This Pine Script® code is subject to the terms of the [Mozilla Public License 2.0](https://mozilla.org/MPL/2.0/).

## ⚠️ Disclaimer

This indicator is for educational and informational purposes only. It should not be considered as financial advice. Always do your own research and consider your risk tolerance before making trading decisions.

## 📞 Support

- **Issues**: [GitHub Issues](../../issues)
- **Discussions**: [GitHub Discussions](../../discussions)
- **TradingView**: Search for "Midpoint Moves" by CraftyChaos

## 🏷️ Version History

### v1.0.0
- Initial release
- Basic midpoint calculation
- Dynamic support/resistance levels
- Customizable colors and visibility options

---

**Made with ❤️ for the TradingView community**
