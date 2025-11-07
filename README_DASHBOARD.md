# Noon Recruitment Dashboard

## Overview
Professional recruitment dashboard for Noon delivery driver applications with bilingual support (English/Arabic) and Noon's brand colors.

## Features

### 🎨 Design
- **Brand Colors**: Yellow (#FFD600) and Black (#111) throughout
- **Responsive**: Mobile-friendly layout
- **Modern UI**: Gradient backgrounds, hover effects, shadows

### 🌐 Language Support
- **Bilingual**: Switch between English and Arabic
- **Dynamic**: Content updates without page reload
- **RTL Support**: Proper right-to-left layout for Arabic

### 📊 Statistics Dashboard
- **6 Stat Cards**:
  - Total Applicants
  - Qualified (Vehicle + Experience)
  - Available Immediately
  - Today's Applications
  - With Valid License
  - This Week's Applications

### 📈 Visualizations
- **4 Interactive Charts**:
  - Applicants by Emirate (Bar Chart)
  - Qualifications Overview (Doughnut Chart)
  - 7-Day Trend (Line Chart)
  - Availability Status (Pie Chart)

### 🔍 Filters
- Filter by Emirate
- Filter by Vehicle Ownership
- Filter by Delivery Experience
- Refresh Data button

### 📋 Recent Applications Table
- Last 10 applicants
- Name, Emirate, Vehicle, Experience, Status, Date
- Color-coded status badges

## Data Structure

### CSV Format (`applicants_data.csv`)
```
Timestamp,Full Name,Nationality,Age,Phone Number,Email,Emirate,Has Driving License,Has Valid Residency,Owns Vehicle,Vehicle Type,Has Delivery Experience,Available Immediately
```

### Google Sheets Integration
- Columns A:K (11 columns)
- Auto-updates from form submissions
- Real-time statistics

## Files

- `index.html` - Application form
- `dashboard.html` - Dashboard page
- `applicants_data.csv` - Cleaned applicant data (32 records)

## Security Notes

⚠️ **Known Issue**: API credentials are currently hardcoded in the client-side JavaScript. This is a pre-existing issue that should be addressed by:
1. Moving credentials to server-side code
2. Using environment variables
3. Implementing backend proxy for API calls

## Statistics (as of commit 46e9b3c)

- **32 Applicants** in cleaned data
- **26 with vehicles** (81%)
- **20 with experience** (63%)
- **Emirates**: Dubai (10), Ajman (8), Sharjah (7), Abu Dhabi (5), Ras Al Khaimah (1), Others (1)

## Browser Support
- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers

## Dependencies
- Chart.js (CDN)
- Google Sheets API
- Cairo font (Google Fonts)
