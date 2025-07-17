# RENEC Solarpunk Standards Explorer

A beautiful, interactive web application for exploring renewable energy competency standards with a solarpunk aesthetic. Built with modern web technologies and featuring neumorphic design principles.

## 🌱 Overview

The RENEC Solarpunk Standards Explorer is a curated collection of competency standards designed to empower builders, dreamers, and communities working toward sustainable futures. This tool provides foundational skills for fostering renewable energy, strengthening community bonds, and practicing regenerative methods.

## ✨ Features

### 🎨 Design & UX
- **Neumorphic Design**: Modern, tactile interface with soft shadows and depth
- **Responsive Layout**: Works seamlessly across desktop, tablet, and mobile devices
- **Dark/Light/Auto Themes**: Automatic system theme detection with manual override options
- **Smooth Animations**: Subtle hover effects and transitions for enhanced user experience

### 🌍 Internationalization
- **Bilingual Support**: English and Spanish language options
- **Real-time Translation**: Instant language switching without page reload
- **Persistent Language**: Remembers user's language preference

### 🔍 Advanced Filtering
- **Text Search**: Search across titles, committees, and sectors
- **Multi-level Filtering**: Filter by rank, sector, committee, and tags
- **Interactive Tag System**: Click to toggle multiple tags simultaneously
- **Real-time Results**: Instant filtering with live result counts
- **Clear All Filters**: One-click reset functionality

### 📊 Data Organization
- **Rank-based Priority**: High/Medium/Low ranking system with color coding
- **Sector Classification**: Organized by productive sectors
- **Committee Structure**: Standards grouped by responsible committees
- **Tag System**: Flexible categorization with visual tag indicators

## 🛠️ Technical Stack

- **Frontend**: Vanilla JavaScript (ES6+)
- **Styling**: Tailwind CSS with custom CSS variables
- **Fonts**: Google Fonts (Inter)
- **Icons**: Heroicons (SVG)
- **Data Format**: JSON
- **Theme System**: CSS custom properties with localStorage persistence

## 📁 Project Structure

```
renec-solarpunk-standards/
├── index.html              # Main application file
├── renec_solarpunk.json    # Standards data (required)
├── README.md              # This file
└── assets/                # Optional assets directory
```

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- Local web server (for development)

### Installation

1. **Clone or download** the project files
2. **Ensure data file exists**: Place `renec_solarpunk.json` in the same directory as `index.html`
3. **Serve locally**: Use a local web server to avoid CORS issues:

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

4. **Open in browser**: Navigate to `http://localhost:8000`

### Data Format

The application expects a JSON file named `renec_solarpunk.json` with the following structure:

```json
[
  {
    "Código": "Standard code",
    "Título": "Standard title",
    "Nivel": "Level description",
    "Comité": "Committee name",
    "Sector Productivo": "Productive sector",
    "solarpunk-rank": "High|Medium|Low",
    "solarpunk-alignment": "Description of alignment",
    "solarpunk-tags": ["tag1", "tag2", "tag3"]
  }
]
```

## 🎯 Usage

### Basic Navigation
- **Search**: Use the search bar to find standards by title, committee, or sector
- **Filter**: Apply filters using the dropdown menus and tag buttons
- **Language**: Switch between English and Spanish using the language toggle
- **Theme**: Choose light, dark, or auto theme using the theme switcher

### Advanced Features
- **Multiple Tag Selection**: Click multiple tags to filter by all selected tags
- **Sticky Controls**: Filter controls remain accessible while scrolling
- **Responsive Design**: Optimized for all screen sizes
- **Keyboard Navigation**: Full keyboard accessibility support

## 🎨 Customization

### Themes
The application supports easy theme customization through CSS custom properties:

```css
:root {
  --bg-color: #e0e5ec;
  --text-color: #374151;
  --accent-color: #10b981;
  /* ... more variables */
}
```

### Adding Languages
To add new languages, extend the `translations` object in the JavaScript:

```javascript
const translations = {
  en: { /* English translations */ },
  es: { /* Spanish translations */ },
  fr: { /* French translations */ }
};
```

### Styling
The neumorphic design system uses consistent CSS classes:
- `.neumorphic-outset`: Raised elements
- `.neumorphic-inset`: Depressed elements
- `.neumorphic-card`: Content cards with hover effects
- `.neumorphic-button`: Interactive buttons

## 🔧 Configuration

### Local Storage
The application uses localStorage for:
- Theme preference (`solarpunk_theme`)
- Language preference (planned feature)

### Performance
- Efficient filtering algorithms for large datasets
- Lazy loading of non-critical resources
- Optimized CSS for smooth animations

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Bug Reports**: Open an issue with detailed reproduction steps
2. **Feature Requests**: Suggest new features or improvements
3. **Translations**: Add support for additional languages
4. **Documentation**: Improve documentation and examples

### Development Guidelines
- Follow existing code style and conventions
- Test across multiple browsers and devices
- Ensure accessibility standards are maintained
- Keep the neumorphic design system consistent

## 🌟 About

This project is a gift from **Innovaciones MADFAM** to the global community of builders, dreamers, and sustainable development practitioners. It represents a commitment to open knowledge sharing and collaborative learning in the renewable energy sector.

## 📄 License

This project is released under an open-source license. Please refer to the LICENSE file for details.

## 🔮 Future Enhancements

- **Export Functionality**: PDF/CSV export of filtered results
- **Bookmark System**: Save favorite standards
- **Advanced Analytics**: Usage statistics and insights
- **Mobile App**: Native mobile applications
- **API Integration**: Real-time data synchronization
- **Community Features**: Comments and ratings system

## 🐛 Known Issues

- Large datasets (1000+ items) may experience slight performance delays
- Some screen readers may need additional ARIA labels
- Internet Explorer is not supported

## 📞 Support

For questions, suggestions, or support:
- Open an issue on the project repository
- Contact Innovaciones MADFAM
- Check the documentation for common solutions

---

*Built with ❤️ for a sustainable future*
