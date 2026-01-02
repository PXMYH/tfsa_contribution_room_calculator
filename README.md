# TFSA Contribution Room Calculator

A web-based calculator to help Canadian residents track their Tax-Free Savings Account (TFSA) contribution room and transaction history.

## Features

### Core Functionality
- **Contribution Room Calculation**: Automatically calculates available TFSA contribution room based on year of birth and tax residency date
- **Transaction Tracking**: Record deposits and withdrawals with dates
- **Withdrawal Carry-Forward**: Accurately calculates re-contribution room from previous year withdrawals per CRA rules
- **Multi-Session Support**: Save and manage multiple user profiles

### User Experience
- **Input Validation**: Ensures year of birth (18+ required) and tax residency dates are valid
- **Confirmation Dialogs**: Warns before clearing data or overwriting sessions
- **Sortable History**: Click column headers to sort transactions by date or type
- **Delete Transactions**: Remove individual transactions with a single click
- **Responsive Design**: Mobile-friendly interface using Bootstrap

### Data Management
- **Session Persistence**: Save sessions to browser localStorage
- **Export/Import**: Download all data as JSON files for backup
- **Session Deletion**: Remove unwanted sessions with confirmation

## How to Use

1. **Open** [index.html](index.html) in any web browser
2. **Enter** your username, year of birth, and year you became a Canadian tax resident
3. **Add transactions** with date, type (deposit/withdraw), and amount
4. **View** your available and remaining contribution room automatically calculated
5. **Save** your session to preserve data
6. **Export** data regularly for backup (recommended due to browser cache limitations)

## TFSA Rules Implemented

- **Start Year**: 2009 (TFSA program inception)
- **Age Requirement**: Must be 18+ to contribute
- **Annual Limits**: Up-to-date limits from 2009-2025 (source: CRA)
- **Withdrawal Re-Contribution**: Withdrawals from year X can be re-contributed starting January 1 of year X+1

## Technical Details

- **Single File**: Everything in one HTML file for easy deployment
- **No Backend**: Runs entirely in the browser
- **Modern JavaScript**: Clean, well-organized code with clear section comments
- **Bootstrap 5**: Professional, responsive styling

## Data Backup

**Important**: Browser localStorage can be cleared by the browser. Use the Export/Import feature to:
- Create regular backups of your data
- Transfer data between computers/browsers
- Maintain long-term records independent of browser settings

Export creates timestamped JSON files (`tfsa_backup_YYYY-MM-DD.json`) that can be imported anytime.

## Browser Compatibility

Works in all modern browsers (Chrome, Firefox, Safari, Edge) that support:
- localStorage
- File API (for export/import)
- ES6+ JavaScript

## License

MIT License - Free to use and modify.
