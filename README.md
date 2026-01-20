# 💰 Smart Expense Tracker

A beautiful, modern expense tracking web application built with HTML, CSS, and JavaScript. Track your spending across different categories and visualize your expenses with interactive charts.

## Features

✨ **Core Functionality**
- Add expenses with description, amount, and category
- Track spending across 5 pre-defined categories: Food, Travel, Rent, Utilities, and Other
- View recent expense history with dates
- Delete expenses with one click
- All data persists in browser's local storage

📊 **Visualization**
- Interactive bar chart showing total spending by category
- Real-time chart updates as you add/remove expenses
- Visual category breakdown for better spending insights

🎨 **Design Highlights**
- Modern glassmorphism UI with blue/teal/green gradient background
- Responsive layout that works on desktop and mobile devices
- Smooth animations and transitions
- Professional finance-themed color scheme
- Custom scrollbar styling for better aesthetics

## Getting Started

### Installation
No installation required! Simply open the HTML file in any modern web browser.

1. Download or clone the project
2. Open `smart.html` in your web browser
3. Start tracking your expenses!

### System Requirements
- Any modern web browser (Chrome, Firefox, Safari, Edge)
- No backend server or internet connection needed (works offline)
- Browser must support:
  - ES6 JavaScript
  - Local Storage API
  - CSS Grid and Flexbox
  - CSS Backdrop Filter

## How to Use

### Adding an Expense
1. Enter a **description** (e.g., "Lunch", "Gas")
2. Enter the **amount** (numerical value)
3. Select a **category** from the dropdown
4. Click the **"Add Expense"** button

### Viewing Expenses
- **Recent History Panel**: Shows all expenses with dates and amounts
- **Spending Overview Chart**: Visual representation of total spending by category

### Deleting an Expense
- Click the ❌ button next to any expense to remove it
- Changes are automatically saved to local storage

## Technical Details

### Technology Stack
- **HTML5**: Semantic markup and structure
- **CSS3**: Advanced styling with gradients, animations, and backdrop filters
- **JavaScript (ES6)**: Core application logic
- **Chart.js**: Library for creating the spending overview chart
- **LocalStorage API**: Client-side data persistence

### Key Components

#### State Management
- Expenses array stored in browser's localStorage
- Automatic save on every add/delete operation
- Data persists across browser sessions

#### Data Structure
Each expense object contains:
```javascript
{
  id: unique timestamp,
  desc: "Expense description",
  amount: numerical value,
  category: "Food|Travel|Rent|Utilities|Other",
  date: "MM/DD/YYYY"
}
```

#### Main Functions
- `addExpense()`: Adds new expense and validates input
- `deleteExpense(id)`: Removes expense by ID
- `saveAndRender()`: Saves to localStorage and updates UI
- `renderList()`: Updates expense list display
- `renderChart()`: Creates/updates the bar chart visualization

### CSS Features
- **Gradient Background**: Finance-focused blue-to-green theme
- **Glassmorphism**: Semi-transparent container with blur effect
- **Responsive Grid**: Adapts from 2 columns (desktop) to 1 column (mobile)
- **Smooth Animations**: Entrance animation and hover effects
- **Custom Scrollbar**: Styled for consistency with design theme

## Browser Compatibility

| Browser | Supported |
|---------|-----------|
| Chrome/Edge (Latest) | ✅ Yes |
| Firefox (Latest) | ✅ Yes |
| Safari (Latest) | ✅ Yes |
| Mobile Browsers | ✅ Yes |

## Data Storage

- All expenses are stored in **browser localStorage**
- Data is **not** sent to any server
- Clearing browser data/cache will delete expense history
- Back up your data by exporting JSON manually if needed

## Responsive Design

The app is fully responsive:
- **Desktop** (>768px): 2-column layout with chart beside list
- **Tablet** (768px): Single column layout
- **Mobile** (<480px): Optimized touch-friendly interface

## Future Enhancement Ideas

- 📅 Date range filtering
- 💾 Export/Import data as CSV
- 🎯 Budget goals and alerts
- 📱 PWA support for offline usage
- 🔒 Password-protected data
- 📈 Monthly/Yearly comparison charts
- 🏷️ Custom category creation

## License

Free to use and modify for personal projects.

## Support

For issues or feature requests, feel free to reach out or submit feedback.

---

**Happy Expense Tracking! 💳✨**
