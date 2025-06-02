# QC Progressive Report Web Application (Design)

## 📋 Description
A web application for daily production reports from the Quality Control Department - Cream Processing at PT. Anugrah Mitra Maju. This system enables 3 work shifts to perform continuous data input within a single production day.

## 🎯 Main Features
- **Multi-Shift Interface**: Three shift tabs with different working hours
  - 🌅 **Shift 1**: 07:00-15:00 (Morning)
  - 🌤️ **Shift 2**: 15:00-23:00 (Afternoon) 
  - 🌙 **Shift 3**: 23:00-07:00 (Night)

- **Progressive Data Entry**: Subsequent shifts can continue data from previous shifts
- **PDF Generation**: Generate reports in PDF format
- **Data Security**: Verification system to prevent data manipulation
- **Responsive Design**: Optimized for desktop and mobile

## 🔒 Security System

### Verification Code
- Each shift has a unique and confidential verification code
- Prevents other shifts from falsifying specific shift data
- Must be filled before generating PDF

### Production Code
- Format contains: day-date-year-shift-shift_name
- Example: `010151A` 
- Prevents data input from different days
- Ensures daily production continuity

## 🔄 Workflow

### Shift 1 (Morning)
- Start a new daily report
- Input initial production data
- Generate PDF to be passed to the next shift

### Shift 2 (Afternoon)
- **Option 1**: Upload PDF from Shift 1 to continue data
- **Option 2**: Start a new report if production begins from shift 2
- Generate combined PDF (Shift 1 + 2) or new PDF

### Shift 3 (Night)
- **Option 1**: Upload PDF from previous shift to continue
- **Option 2**: Start a new report if production begins from shift 3
- Generate final PDF for one production day

## 📊 Data Collected

### Storage Data
- Top Gap Storage BSC (cm)
- Top Gap Storage MCP (cm)

### Ballmill BSC
- Start Batch Amount in Ballmill (kg)
- BSC Process Amount Today (kg)
- End Batch Amount in Ballmill (kg)
- Usage Amount (kg)

### Ballmill MCP
- Start Batch Amount in Ballmill (kg)
- MCP Process Amount Today (kg)
- End Batch Amount in Ballmill (kg)
- Usage Amount (kg)

### Additional Information
- Shift notes (constraints/important notes)
- Production code
- Shift verification code

## 🛠️ Technology

### Frontend (Current - Design Only)
- **HTML5**: Application structure
- **CSS3**: Styling with responsive design
- **JavaScript**: Basic UI interactions (tab switching)

### Backend (In Development)
- PDF generation functionality
- Data persistence
- File upload handling
- Verification system

## 📁 File Structure
```
qc-progressive-report/
├── index.html          # Main HTML file
├── style.css           # Styling
├── README.md           # Documentation
```

## 🚀 Usage Guide

### Setup
1. Clone this repository
2. Open `index.html` in web browser
3. Select the appropriate shift according to working hours

### Shift 1 Data Input
1. Enter production code
2. Fill in all storage and ballmill data
3. Add notes if necessary
4. Enter shift 1 verification code
5. Generate PDF

### Shift 2/3 Data Input
1. **If continuing**: Upload PDF from previous shift
2. **If starting new**: Directly fill the form
3. Complete all required data
4. Enter the appropriate verification code
5. Generate PDF

## ⚠️ Development Status

### ✅ Completed (Design Phase)
- UI/UX Design
- Responsive layout
- Form structure
- Tab navigation
- CSS styling

### 🔄 In Development (Backend Team)
- PDF generation functionality
- File upload processing
- Data validation
- Verification system
- Data persistence
- Progressive data merging

## 📱 Compatibility
- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## 🔮 Roadmap
- [ ] Backend API development
- [ ] Database integration
- [ ] User authentication
- [ ] Data export features
- [ ] Historical report viewing
- [ ] Email notification system

## 👥 Development Team
- **Frontend/Design**: Current contributor
- **Backend/Functionality**: IT Department (In Progress)
- **Quality Control**: PT. Anugrah Mitra Maju

## 📞 Contact
For technical questions or feedback:
- diwangkararevan@gmail.com

---

## 📝 Important Notes
- This application is still in **DESIGN ONLY** phase
- Backend functionality is being developed by a separate team
- UI/UX is finalized and ready for backend implementation
- No data is stored in the current version

## 🤝 Contribution
Currently, this project is in the design completion phase. Backend contributions will be handled by the internal IT department.

---
*Last updated: May 2025*
