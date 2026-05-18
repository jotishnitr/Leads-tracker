# 📈 Leads Tracker Chrome Extension

A lightweight Chrome extension built using HTML, CSS, and JavaScript to save and manage useful links (leads) directly from your browser.

This extension allows users to:
- Save custom URLs manually
- Save the currently opened browser tab instantly
- Store leads permanently using Local Storage
- Quickly access saved links anytime

---

## 🚀 Features

- ✅ Save URLs manually
- ✅ Save current browser tab with one click
- ✅ Persistent storage using Local Storage
- ✅ Open saved links in new tabs
- ✅ Delete all saved leads instantly
- ✅ Clean and minimal UI
- ✅ Fast and lightweight Chrome extension

---

## 🧠 Concepts Used

- DOM Manipulation
- Event Listeners
- Local Storage
- Chrome Extension APIs
- Chrome Tabs API
- Dynamic HTML Rendering
- Manifest V3

---

## 📂 Project Structure

```bash
Leads-Tracker/
│
├── index.html
├── index.css
├── index.js
├── manifest.json
├── icon.png
```

---

## ⚙️ How the Extension Works

### SAVE INPUT
- Manually enter a URL
- Click **SAVE INPUT**
- The link gets stored permanently

### SAVE TAB
- Saves the URL of the currently active browser tab
- Uses Chrome Tabs API

### DELETE ALL
- Clears all saved leads from Local Storage

---

# 🛠️ How to Use This Extension

## Step 1 — Download the Project

Clone or download this repository.

```bash
git clone https://github.com/your-username/leads-tracker.git
```

Or download ZIP and extract it.

---

## Step 2 — Open Chrome Extensions Page

Open Chrome and go to:

```bash
chrome://extensions/
```

---

## Step 3 — Enable Developer Mode

- Turn ON **Developer Mode** (top-right corner)

---

## Step 4 — Load the Extension

- Click **Load unpacked**
- Select the project folder

Example:

```bash
Leads-Tracker/
```

---

## Step 5 — Start Using

- Click the extension icon in Chrome
- Save URLs manually or save current tabs instantly

---

## 💾 Data Storage

All saved leads are stored in:

- Browser Local Storage

This means:
- Leads remain saved after closing the browser
- No backend or database required

---

## 📸 Preview

### Real Usage Example
<img width="1891" height="1080" alt="image" src="https://github.com/user-attachments/assets/073b599a-1c4c-4f60-9ed4-2f3c22223f1a" />

### Extension Popup
<img width="533" height="216" alt="image" src="https://github.com/user-attachments/assets/8daa669d-19d2-4c47-9d29-a38b3d96f7f4" />


## 🔧 Future Improvements

- Add categories/tags for leads
- Add export/import feature
- Add search functionality
- Add dark mode
- Add duplicate link detection
- Add edit/update feature

---

## 📌 Permissions Used

### Tabs Permission

Used to access the current browser tab URL.

From `manifest.json`:

```json
"permissions":["tabs"]
```

---

## 🎨 UI Details

The extension uses:
- Gradient buttons
- Clean responsive layout
- Minimal design system
- Hover animations
- Smooth transitions

---

## 🧩 Technical Implementation

### Local Storage

Saved leads are stored using:

```javascript
localStorage.setItem("myLeads", JSON.stringify(myLeads))
```

### Chrome Tabs API

Current tab URL is captured using:

```javascript
chrome.tabs.query({active:true, currentWindow:true}, function(tabs){
```

---

## 📌 Note

This project was built as part of my JavaScript and Chrome Extension learning journey to strengthen frontend development fundamentals and browser API usage.
