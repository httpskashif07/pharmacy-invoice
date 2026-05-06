
  # Pharmacy Invoice Generator

  A professional, browser-based invoice generator built for pharmacy delivery services. Upload your delivery data,
  configure rates, and produce polished PDF invoices — no backend or installation required.

  **Live site:**
  [httpskashif07.github.io/pharmacy-invoice-generator](https://httpskashif07.github.io/pharmacy-invoice-generator)

  ---

  ## Features

  ### File Import
  - Drag-and-drop or click-to-browse upload
  - Supports `.xlsx`, `.xls`, `.csv`, `.htm`, and `.html` spreadsheets
  - Auto-detects pharmacy name, delivery count, and distance columns
  - Handles multi-file Excel (HTML Frameset) format with guidance

  ### Flexible Rate Modes
  | Mode | Description |
  |---|---|
  | **Default** | Flat $5.00 per delivery for all pharmacies |
  | **Manual** | Custom flat rate you enter |
  | **By Distance** | Four configurable zones (0–5 km, 5–20 km, 20–30 km, 30+ km) |
  | **By Pharmacy** | Individual zone breakdown per pharmacy |

  - Optional tax rate (%) applied to subtotal

  ### Invoice Builder
  - Enter your company info: name, address, phone, email, HST number
  - Set the "Bill To" client details
  - Live invoice preview updates as you type
  - Professional typeset layout (DM Serif Display + DM Mono fonts)

  ### Save & Export Options
  - **Download PDF** — print-ready A4 PDF via jsPDF
  - **Email** — sends invoice via EmailJS
  - **Print** — browser print with colour-accurate output
  - **Save Draft** — persists your work locally and prompts restoration on next visit

  ### User Accounts
  - Sign in / Register with username and password
  - Forgot password — OTP emailed to your registered address
  - Forgot username — OTP recovery via email
  - Accounts and invoice history stored in Firebase Firestore

  ### Invoice History
  - Browse all past invoices per account
  - Filter by All / Drafts / Saved
  - Delete individual records

  ### Admin Dashboard
  - Overview stats (total users, invoices, tickets)
  - User management with password reveal
  - All-invoices table across all accounts
  - Support ticket queue

  ### Help & Support
  - In-app ticket submission: Feedback, Complaint, or Help Request
  - Ticket saved to Firestore and emailed to admin

  ---

  ## Tech Stack

  | Library | Purpose |
  |---|---|
  | [SheetJS (xlsx)](https://sheetjs.com/) | Parse Excel and CSV files |
  | [jsPDF](https://github.com/parallax/jsPDF) + jspdf-autotable | Generate PDF invoices |
  | [EmailJS](https://www.emailjs.com/) | Send emails from the browser |
  | [Firebase Auth + Firestore](https://firebase.google.com/) | User accounts and data storage |
  | Google Fonts (DM Serif Display, DM Mono, DM Sans) | Typography |

  No build step. No server. One HTML file.

  ---

  ## Usage

  1. Open the live site or download `pharmacy-invoice-generator.html` and open it in any modern browser.
  2. Create an account or sign in.
  3. **Upload** your delivery spreadsheet(s).
  4. Choose a **rate mode** and configure rates.
  5. Fill in your **company and client details**.
  6. Click **Generate Invoice** to preview.
  7. **Download PDF**, email, or print.

  ---

  ## Local Setup

  No installation needed. Clone the repo and open the HTML file directly:

  ```bash
  git clone https://github.com/httpskashif07/pharmacy-invoice-generator.git
  cd pharmacy-invoice-generator
  # Open pharmacy-invoice-generator.html in your browser

  ---
  License

  MIT — free to use and modify.
