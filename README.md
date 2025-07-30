# PassiveBot Config Viewer

**Live Tool**: [https://majedpro.github.io/pbview/](https://majedpro.github.io/pbview/)

A comprehensive web-based viewer for PassiveBot trading configuration files. This tool provides an intuitive interface to analyze and visualize all aspects of your PassiveBot configurations.

![PassiveBot Config Viewer](https://img.shields.io/badge/PassiveBot-Config%20Viewer-00d4ff?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## 🚀 Features

### 📊 **Performance Analysis**
- **Core Metrics**: Total Gain, ADG, Sharpe Ratio, Omega Ratio, Max Drawdown, Loss/Profit Ratio
- **Advanced Ratios**: Calmar Ratio, Sortino Ratio, Sterling Ratio
- **Weighted Metrics**: ADG, Sharpe, Omega, and Calmar weighted calculations
- **Position Statistics**: Hold times, positions per day, and trading frequency analysis
- **Visual Progress Bars**: Color-coded performance indicators

### 🔧 **Bot Configuration**
- **Comprehensive Parameter Display**: 20+ parameters per long/short side
- **Entry Settings**: Grid spacing, quantity percentages, EMA distances
- **Close Settings**: Markup ranges, quantity percentages, trailing parameters
- **Risk Management**: Unstuck thresholds, loss allowances, exposure limits
- **Filter Settings**: Volume clips, rolling windows, and market conditions

### 📈 **Backtest Configuration**
- **Flexible Symbol Handling**: Supports both array and object formats
- **Exchange Management**: Multi-exchange trading configurations
- **Date Ranges**: Start/end dates with balance information
- **Advanced Settings**: OHLCVS combining, cache compression, gap tolerance

### ⚡ **Live Trading Settings**
- **Execution Parameters**: Delays, batch limits, market orders
- **Risk Controls**: Coin age requirements, restart limits, price thresholds
- **Approved Coins**: Flexible long/short or unified coin lists
- **Performance Monitoring**: PnL lookback, OHLCVS updates

### 🎯 **Optimization Analysis**
- **Algorithm Settings**: Iterations, population size, CPU usage
- **Genetic Parameters**: Crossover and mutation probabilities
- **Parameter Bounds**: Visual range displays for optimization limits
- **Scoring Methods**: Multi-objective optimization criteria

### 🎨 **User Experience**
- **Dark Theme**: Professional, eye-friendly interface
- **Drag & Drop**: Seamless file loading with visual feedback
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Auto-Expansion**: All sections expanded by default for quick overview
- **Global File Reload**: Drop new configs anywhere on the page
- **Progress Indicators**: Real-time loading animations

## 🛠️ Usage

### Quick Start
1. **Download**: Save `config-viewer.html` to your computer
2. **Open**: Double-click the file or open in any modern web browser
3. **Load Config**: Drag and drop your `config.json` file or click to browse
4. **Analyze**: Explore all sections of your configuration data

### Supported File Formats
- ✅ **Standard PassiveBot Configs**: Full analysis with performance data
- ✅ **Basic Bot Configs**: Configuration-only files (like BTCUSDT.json)
- ✅ **Mixed Formats**: Handles both object and array structures seamlessly

### File Structure Examples
```json
// Standard format with analysis
{
  "analysis": { "adg": 0.009, "sharpe_ratio": 0.139, ... },
  "backtest": { "symbols": {"binance": ["BTCUSDT"], ...} },
  "bot": { "long": {...}, "short": {...} },
  "live": { "approved_coins": {"long": [...], "short": [...]} },
  ...
}

// Simple format without analysis
{
  "backtest": { "symbols": ["BTCUSDT"] },
  "live": { "approved_coins": ["BTCUSDT"] },
  ...
}
```

## 📋 System Requirements

- **Modern Web Browser**: Chrome 80+, Firefox 75+, Safari 13+, Edge 80+
- **JavaScript**: Must be enabled
- **File Access**: Local file reading capability
- **No Installation**: Runs entirely in the browser

## 🔒 Privacy & Security

- **100% Client-Side**: No data is sent to any server
- **Local Processing**: All analysis happens in your browser
- **No Dependencies**: Self-contained HTML file with embedded resources
- **Offline Capable**: Works without internet connection

## 🎨 Visual Features

### Color Coding
- 🟢 **Green**: Good performance metrics and positive values
- 🟡 **Orange**: Medium performance metrics
- 🔴 **Red**: Poor performance metrics and negative values
- 🔵 **Blue**: Neutral information and section headers

### Responsive Grid Layout
- **Auto-fit Columns**: Adapts to screen size automatically
- **Minimum Widths**: Ensures readability on all devices
- **Flexible Spacing**: Optimized for both desktop and mobile viewing

## 📊 Metrics Interpretation

### Performance Thresholds
| Metric | Good | Medium | Poor |
|--------|------|--------|------|
| Sharpe Ratio | > 1.0 | 0.5-1.0 | < 0.5 |
| Omega Ratio | > 2.0 | 1.5-2.0 | < 1.5 |
| ADG | > 0.5% | 0.2-0.5% | < 0.2% |
| Max Drawdown | < 20% | 20-50% | > 50% |
| Loss/Profit Ratio | < 0.4 | 0.4-0.6 | > 0.6 |

## 🚧 Browser Compatibility

| Browser | Minimum Version | Status |
|---------|----------------|---------|
| Chrome | 80+ | ✅ Fully Supported |
| Firefox | 75+ | ✅ Fully Supported |
| Safari | 13+ | ✅ Fully Supported |
| Edge | 80+ | ✅ Fully Supported |
| Internet Explorer | - | ❌ Not Supported |

## 🐛 Troubleshooting

### Common Issues
1. **File Won't Load**
   - Ensure the file is valid JSON
   - Check that JavaScript is enabled
   - Try refreshing the page

2. **Missing Data**
   - Some sections may not appear if data is missing from config
   - This is normal for basic configuration files


## 🤝 Contributing

This is a single-file application designed for simplicity and portability. To contribute:

1. **Fork** the repository
2. **Modify** the `config-viewer.html` file
3. **Test** with various PassiveBot configuration files
4. **Submit** a pull request with your improvements

### Development Guidelines
- Maintain the single-file architecture
- Ensure backward compatibility with existing config formats
- Test with both analysis and non-analysis configurations
- Keep the dark theme consistent
- Ensure mobile responsiveness

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **PassiveBot Community**: For providing the configuration formats and use cases

---

**Made with ❤️ for the PassiveBot community**

For questions, issues, or feature requests, please open an issue on GitHub.
