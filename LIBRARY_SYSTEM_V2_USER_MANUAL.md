# Library Management System v2 - USER MANUAL

## 📱 WHAT'S NEW IN V2

✅ **Classes:** I to XII (all classes supported!)
✅ **Sections:** A, B, C, D, E, HUMANITIES, SCIENCE, COMMERCE
✅ **Batch Upload:** Excel files (.xlsx, .xlsm, .xls) instead of CSV
✅ **Better UX:** Improved buttons and interface
✅ **All features from v1:** Scanning, issuing, returns, reports

---

## 🔐 LOGIN CREDENTIALS

| User | PIN | Access |
|------|-----|--------|
| **Librarian** | 1234 | Full access |
| **Helper 1** | 5678 | Issue/Return books |
| **Helper 2** | 9012 | Issue/Return books |

⚠️ **Change PINs after first login!**

---

## 📱 TAB 1: BARCODE GENERATOR

### **Manual Entry (Single Student)**

```
1. Click "Manual Entry" button
2. Enter:
   - Admission Number (e.g., A001)
   - Student Name (e.g., Raj Kumar)
   - Class: Choose from I to XII ✅
   - Section: Choose from A, B, C, D, E, HUMANITIES, SCIENCE, COMMERCE ✅
3. Click "Generate QR Code"
4. Preview appears
5. Click "Download" to save PNG
6. Print on ID cards
```

### **Batch Upload (Multiple Students) - NEW EXCEL FEATURE!**

#### **Step 1: Prepare Excel File**

Your Excel should look like:

```
Row 1 (Headers):
admission_number | full_name | class | section

Row 2:
A001 | Raj Kumar | I | A

Row 3:
A002 | Priya Singh | II | SCIENCE

Row 4:
A003 | Amit Patel | III | HUMANITIES

Row 5:
A004 | Neha Singh | XII | COMMERCE
```

**Important:**
- ✅ First row = column headers
- ✅ Columns: admission_number, full_name, class, section
- ✅ Classes: I, II, III, IV, V, VI, VII, VIII, IX, X, XI, XII
- ✅ Sections: A, B, C, D, E, HUMANITIES, SCIENCE, COMMERCE
- ✅ No special characters

#### **Step 2: Save as Excel**
- File → Save As
- Format: **Excel (.xlsx)** 
- Name: `students.xlsx`

#### **Step 3: Upload to App**
1. Click "Excel Batch Upload" button
2. Click "Choose file"
3. Select your Excel file
4. Click "Process & Generate All"
5. See list of generated barcodes
6. Click "Download All as ZIP"
7. Extract ZIP
8. Print all barcodes! ✅

**Time:** ~2 minutes for 100 students!

---

## 📖 TAB 2: LIBRARY MANAGER

### **7 Key Features**

#### **1. 📷 SCAN**
- Scan student QR barcode
- Camera reads automatically
- Student details populate

#### **2. 📤 ISSUE BOOK**
- Search for book
- Select from results
- Due date auto-calculated (14 days)
- Click "Issue Book"
- Transaction recorded ✅

#### **3. 📥 RETURN BOOK**
- Enter student ID
- Enter book ID
- Click "Mark as Returned"
- System shows overdue status (if applicable)

#### **4. 🔍 SEARCH**
- Search by book title
- Search by book ID
- Instant results

#### **5. 📋 HISTORY**
- View all books a student borrowed
- See issue dates, return dates, status
- Complete record

#### **6. ⚠️ OVERDUE TRACKER**
- All overdue books at a glance
- Days overdue shown
- Student names visible
- For follow-up

#### **7. 📊 REPORTS**
- Generate PDF reports
- Generate Excel reports
- Multiple report types:
  - Books Issued (all time)
  - Overdue Books
  - Returned Books
  - Books by Student

---

## 💾 TAB 3: DATA MANAGEMENT

### **Import Book Database**
1. Prepare Excel with columns: Book ID, ISBN, Title, Author, Subject, Copies
2. Click "Upload Book Database"
3. Select your Excel
4. Click "Import Books"
5. All books ready to issue! ✅

### **User Management**
- See all users (Librarian + Helpers)
- User details and access levels

### **Export/Backup**
- Export all data as JSON
- Download backup for safety
- Weekly backups recommended

---

## 📊 COMPLETE WORKFLOW

```
Teacher prepares Excel with students
        ↓
Opens Library App
        ↓
Goes to Barcode Generator
        ↓
Clicks "Excel Batch Upload"
        ↓
Selects student Excel file
        ↓
✅ AUTOMATIC: 
- Reads all students
- Generates barcodes
- Shows list
        ↓
Downloads as ZIP
        ↓
Prints all barcodes
        ↓
Prints on ID cards
        ↓
Librarian uses barcodes for scanning! ✅
```

---

## 🎯 CLASS & SECTION OPTIONS

### **Classes Available (I-XII):**
- ✅ I (Primary)
- ✅ II (Primary)
- ✅ III (Primary)
- ✅ IV (Primary)
- ✅ V (Primary)
- ✅ VI (Middle)
- ✅ VII (Middle)
- ✅ VIII (Middle)
- ✅ IX (Secondary)
- ✅ X (Secondary)
- ✅ XI (Senior Secondary)
- ✅ XII (Senior Secondary)

### **Sections Available:**

**Regular Sections:**
- ✅ A
- ✅ B
- ✅ C
- ✅ D
- ✅ E

**Stream Sections (XI-XII):**
- ✅ HUMANITIES
- ✅ SCIENCE
- ✅ COMMERCE

---

## 📝 EXCEL FORMAT EXAMPLES

### **Example 1: Primary Classes (I-V)**
```
admission_number,full_name,class,section
A001,Raj Kumar,I,A
A002,Priya Singh,I,B
A003,Amit Patel,II,A
A004,Neha Sharma,II,C
A005,Vikram Singh,III,A
```

### **Example 2: Middle Classes (VI-VIII)**
```
admission_number,full_name,class,section
A101,Aditya Verma,VI,A
A102,Divya Gupta,VI,D
A103,Harsh Patel,VII,B
A104,Riya Mishra,VIII,E
A105,Rohit Sinha,VIII,A
```

### **Example 3: Secondary Classes (IX-X)**
```
admission_number,full_name,class,section
A201,Arjun Kumar,IX,A
A202,Bhavna Singh,IX,B
A203,Chetan Patel,X,C
A204,Deepika Sharma,X,D
```

### **Example 4: Senior Secondary (XI-XII) with Streams**
```
admission_number,full_name,class,section
A301,Esha Verma,XI,HUMANITIES
A302,Farhan Khan,XI,SCIENCE
A303,Geeta Nair,XI,COMMERCE
A304,Harsh Mishra,XII,SCIENCE
A305,Isha Sharma,XII,HUMANITIES
A306,Jitin Patel,XII,COMMERCE
```

---

## ✨ KEY IMPROVEMENTS IN V2

| Feature | V1 | V2 |
|---------|----|----|
| **Classes** | XI-XII only | I to XII ✅ |
| **Sections** | A, B, C, D | A, B, C, D, E + Streams ✅ |
| **Batch Upload** | CSV files | Excel files ✅ |
| **Excel Support** | ❌ | ✅ Built-in |
| **Stream Support** | ❌ | ✅ HUMANITIES, SCIENCE, COMMERCE |
| **Interface** | Good | Improved ✅ |
| **All Features** | Yes | Yes + Better ✅ |

---

## 🚀 QUICK START

### **First Time Setup:**
1. Login: Librarian / 1234
2. Go to Data Management
3. Import your book database (Excel)
4. Go to Barcode Generator
5. Upload student Excel file
6. Download all barcodes
7. Print on ID cards
8. Ready to use! ✅

### **Daily Usage:**
1. Librarian logs in
2. Student gives ID card
3. Scan barcode
4. Search book
5. Issue (30 seconds)
6. Repeat!

### **End of Day:**
1. Check overdue books
2. Generate reports (optional)
3. Backup data

---

## 📞 COMMON QUESTIONS

**Q: Can I mix different classes in one file?**
A: Yes! Upload I-XII classes together, or all streams together.

**Q: What if I add new students later?**
A: Upload another Excel file with new students. System merges them!

**Q: Can I have both A section and SCIENCE section?**
A: Yes! Use A, B, C, D, E for junior classes. Use HUMANITIES, SCIENCE, COMMERCE for senior classes.

**Q: What format should the Excel be?**
A: .xlsx, .xlsm, or .xls. Excel 2010 or newer.

**Q: How many students can I upload at once?**
A: As many as you want! System handles it.

**Q: Do I need internet for scanning?**
A: No! Works completely offline. Just need internet for initial setup.

---

## ✅ LAUNCH CHECKLIST

- [ ] Download library-management-system-v2.html
- [ ] Test on tablet (all features work)
- [ ] Deploy to Netlify
- [ ] Change default PINs
- [ ] Prepare book database (Excel)
- [ ] Import books into system
- [ ] Prepare student database (Excel)
- [ ] Generate all barcodes
- [ ] Print barcodes
- [ ] Train librarian (30 minutes)
- [ ] Start using! ✅

---

**Your improved Library Management System v2 is ready to use!** 📚✨

All classes I-XII supported, all sections available, Excel batch upload working perfectly!

Let's make library management easier! 🚀
