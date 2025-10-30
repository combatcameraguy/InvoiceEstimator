# COMCAM Video Production Quote Calculator

A professional, interactive quote calculator for video production services built with HTML, CSS, and JavaScript. Features real-time price calculations, Firebase integration for quote submissions, and a beautiful card-based UI.

## 🎬 Features

### Filming Services
- **Card-based selection interface** with three options:
  - Post-Production Only (client provides footage)
  - Daily Rate ($650/day) - Best for multi-day shoots
  - Hourly Rate ($200/hour) - Best for short projects
- **Bulk pricing discounts**:
  - Weekly rate: $3,000/week (~$600/day)
  - Monthly rate: $10,000/month (~$333/day)
- **Travel fee calculation** automatically added based on location
- **Complimentary hard drive** with all raw 4K footage

### Post-Production Services
- **5 duration options** with card-based selection:
  - Filming Only (no editing)
  - 15 seconds ($40)
  - 30 seconds ($75)
  - 45 seconds ($120)
  - 1 minute+ (custom input)
- **Auto-calculated color correction**:
  - FREE for videos 1 minute or longer
  - Auto-priced for shorter videos
- **Additional services**:
  - Basic Color Correction (auto-calculated)
  - Advanced Color Grading ($500 flat, $90/min over 5 min)
  - Audio Mixing ($45/min)
  - Sound Design/SFX ($150 flat)
  - Motion Graphics (tiered pricing: $15-$65/sec)
  - Original Music Composition ($200-$500)
  - Professional Voiceover ($300/min)

### Priority Service
- **Fast Lane / Rush Delivery**: +30% fee
- Move to front of production queue for faster turnaround

### Smart Features
- ✅ Real-time price calculation
- ✅ Itemized breakdown with all services listed
- ✅ Visual card selection with hover effects
- ✅ Selected cards highlighted, others dimmed
- ✅ Automatic rounding (to nearest $1 under $1000, nearest $50 over $1000)
- ✅ Firebase integration for quote submissions
- ✅ Responsive design for mobile, tablet, and desktop
- ✅ Form validation and error handling

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/comcam-quote-calculator.git
   cd comcam-quote-calculator
   ```

2. **Open the calculator**
   - Simply open `CLIENT_CALCULATOR_FINAL.html` in your web browser
   - No build process or dependencies required!

3. **Configure Firebase (Optional)**
   - Update the Firebase configuration in the HTML file (lines 805-813)
   - Replace with your own Firebase project credentials
   - Set up Firebase Realtime Database rules

## 📋 Usage

### For Clients
1. Fill in your contact information (Name, Email, Project Name)
2. Select filming services if needed
3. Choose your video duration or select "Filming Only"
4. Check additional services you need
5. Enable Fast Lane if you need rush delivery
6. Review the itemized breakdown
7. Submit your quote request

### For Developers
The calculator is built with vanilla JavaScript - no frameworks required!

**Key Functions:**
- `calculatePrice()` - Calculates total price with all services
- `updateItemizedList()` - Updates the breakdown display
- `updateColorPricingLabels()` - Updates dynamic pricing labels
- `getFilmingRateType()` - Gets selected filming option

## 🎨 Customization

### Modify Pricing
Edit the pricing constants in the JavaScript section:
```javascript
// Filming rates
const hourlyRate = 200;
const dailyRate = 650;
const weeklyRate = 3000;
const monthlyRate = 10000;

// Editing rate
const editingRate = 150; // per minute

// Duration-specific pricing
const duration15sec = 40;
const duration30sec = 75;
const duration45sec = 120;
```

### Styling
All styles are contained in the `<style>` section. Key CSS classes:
- `.duration-checkbox-group` - Card grid layout
- `.duration-option` - Individual card styling
- `.section` - Main content sections
- `.itemized-list` - Price breakdown

### Color Scheme
Primary colors:
- Blue gradient: `#1e3c72` → `#2a5298`
- Accent: `#28a745` (green for success/free items)
- Warning: `#ffc107` (yellow for disclaimers)

## 📱 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Grid, Flexbox, animations
- **Vanilla JavaScript** - No frameworks
- **Firebase** - Realtime Database for quote submissions
- **html2pdf.js** - PDF generation (optional)

## 📦 File Structure

```
comcam-quote-calculator/
│
├── CLIENT_CALCULATOR_FINAL.html    # Main calculator file
├── README.md                        # This file
├── LICENSE                          # MIT License
└── .gitignore                       # Git ignore file
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎯 Roadmap

- [ ] Add PDF export functionality
- [ ] Email integration for automatic quote sending
- [ ] Admin dashboard for managing quotes
- [ ] Payment integration
- [ ] Multi-language support
- [ ] Dark mode theme

## 📞 Support

For questions or support, please contact:
- Email: support@comcam.com
- Website: https://comcam.com

## 🙏 Acknowledgments

- Built for COMCAM Video Production
- Designed for professional videographers and production companies
- Inspired by modern SaaS pricing calculators

---

**Made with ❤️ for video production professionals**
