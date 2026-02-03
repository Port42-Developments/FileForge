# 🗂️ FileForge - Advanced File Renaming Tool

<div align="center">

**A powerful and fully customizable file renaming application with a modern, user-friendly interface**

[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey.svg)](https://www.microsoft.com/windows)

*Transform your file management workflow with intelligent renaming capabilities*

</div>

---

## 🚀 Installation

### Quick Start

1. **Download** `FileForge.exe`
2. **Double-click** to run - no installation required!
3. **Start renaming** your files immediately

**Note:** This is a standalone executable - no additional software or dependencies needed!

---

## ✨ Features

### 🎯 Core Capabilities

- **📑 Multiple Configuration Profiles** - Create and switch between different renaming configurations using intuitive tabs
- **🔧 Customizable Name Parts** - Build complex filenames with multiple parts (first, second, third, etc.)
- **📋 Flexible Input Types** - Each part supports:
  - **Dropdown** - Select from predefined options
  - **Free Text** - Type any custom text
- **🔀 Configurable Separator** - Choose any character(s) to separate name parts (default: `_`)
- **💾 Persistent Fields** - Fields don't reset when selecting different files - perfect for batch renaming
- **👁️ Live Preview** - See the new filename before renaming (supports batch preview)
- **💾 Auto-Save** - All configurations are saved automatically

### 🚀 Advanced Features

- **📦 Batch Renaming** - Select and rename multiple files at once with automatic numbering
- **↶↷ Undo/Redo** - Full undo/redo support for rename operations (up to 50 operations)
- **🔄 Text Transformations** - Apply case conversions and whitespace handling:
  - UPPERCASE, lowercase, Title Case, Sentence case
  - Trim whitespace, Remove all spaces, Trim extra spaces
- **🔢 Numbering Patterns** - Smart numbering with multiple formats:
  - `{001}` or `{0001}` - Zero-padded numbers (001, 002, 003...)
  - `{COUNTER:3}` - Custom width counter
  - `{A}` or `{a}` - Letters (A, B, C... or a, b, c...)
  - `{I}` or `{i}` - Roman numerals (I, II, III... or i, ii, iii...)

### 🛡️ Smart File Management

- **🔍 File Status Detection** - Automatically detects if a file is currently open
- **🔓 Auto-Close on Rename** - Attempts to close open files before renaming
- **✅ Visual Status Indicators** - Clear visual feedback for file availability
- **📋 Batch Selection Counter** - See how many files are selected at a glance

### 🎨 Modern Interface

- **🎨 Beautiful UI** - Modern, clean design with intuitive navigation
- **📱 Responsive Layout** - Optimized for different screen sizes
- **🎯 Color-Coded Actions** - Easy-to-identify buttons and status indicators
- **📊 Scrollable Batch Preview** - View up to 15 file renames before applying

---

## 📖 Usage Guide

### 🎬 Basic Workflow

1. **📁 Select Folder**
   - Click the "📁 Select Folder" button in the header
   - Choose the directory containing files you want to rename

2. **📄 Select File(s)**
   - **Single file**: Click on a file in the file list
   - **Multiple files**: Hold `Ctrl` and click to select individual files, or `Shift` and click to select a range
   - View file status (available/open) in the preview panel
   - See selection count in the file list header

3. **⚙️ Configure Name Parts**
   - Each part can be set to **"dropdown"** or **"free"** type
   - **For dropdown**: Enter comma-separated options (e.g., `Category1,Category2,Category3`)
   - **For free**: Type any text directly
   - Use **➕ Add Part** to add more parts
   - Use **➖ Remove Last** to remove parts

4. **🔄 Apply Transformations** (Optional)
   - Select a transformation from the dropdown for each part:
     - **Case**: uppercase, lowercase, title, sentence
     - **Whitespace**: trim, trim_all, remove_spaces

5. **🔢 Use Numbering Patterns** (For Batch Renaming)
   - Use patterns like `{001}`, `{A}`, `{COUNTER:3}` in your name parts
   - Each file will get a unique number/letter automatically
   - Example: `Photo_{001}` → `Photo_001.jpg`, `Photo_002.jpg`, etc.

6. **🔀 Set Separator**
   - Enter the character(s) to separate name parts
   - Examples: `_`, `-`, `.`, ` - `, etc.

7. **👁️ Preview**
   - **Single file**: Shows the new filename
   - **Batch**: Shows up to 15 files with before/after names
   - Updates in real-time as you make changes

8. **✨ Rename**
   - Click "✨ Rename File" for single file
   - Click "✨ Rename X Files" for batch operations
   - The app will attempt to close files if they're open

9. **↶ Undo / ↷ Redo**
   - Use **Undo** button to reverse the last rename operation
   - Use **Redo** button to re-apply undone operations
   - Supports up to 50 operations in history

10. **🔄 Next File(s)**
    - Select another file or files - your fields stay filled!
    - Just change what you need and rename again

### 📑 Multiple Configurations

FileForge supports multiple renaming profiles for different use cases:

- **➕ Create New Config** - Click "+ New Config" to create a new renaming configuration
- **🔄 Switch Between Configs** - Click on the tabs at the top to switch between different configurations
- **✏️ Rename Config** - Click "✏️ Rename" to rename the current configuration tab
- **🗑️ Delete Config** - Click "🗑️ Delete" to remove the current configuration (at least one must remain)

### 📊 Example Workflows

#### Example 1: Batch Renaming Photos

**Scenario**: Renaming vacation photos with date and sequential numbers

1. Select folder: `vacation_2024/`
2. Create a new configuration called "Vacation Photos"
3. **Part 1** (dropdown): `Summer,Winter,Spring,Autumn`
4. **Part 2** (dropdown): `2023,2024,2025`
5. **Part 3** (free text with pattern): `Photo_{001}`
6. **Separator**: `_`
7. Select multiple files (Ctrl+Click)
8. Preview shows: 
   - `IMG001.jpg` → `Summer_2024_Photo_001.jpg`
   - `IMG002.jpg` → `Summer_2024_Photo_002.jpg`
   - etc.
9. Click "✨ Rename X Files" to apply all changes

#### Example 2: Organizing Documents with Case Conversion

**Scenario**: Renaming documents to Title Case

1. Select folder with documents
2. **Part 1** (free text): `{A}` (for letter sequence)
3. **Part 2** (free text): `document name`
4. **Transformation**: Set Part 2 to "title" case
5. **Separator**: ` - `
6. Result: `A - Document Name.pdf`, `B - Document Name.pdf`, etc.

#### Example 3: Using Roman Numerals

**Scenario**: Creating numbered chapters

1. **Part 1** (free text): `Chapter {I}`
2. **Part 2** (free text): `Introduction`
3. **Separator**: ` - `
4. Result: `Chapter I - Introduction.pdf`, `Chapter II - Introduction.pdf`, etc.

### 🔢 Numbering Patterns Reference

| Pattern | Example Output | Description |
|---------|---------------|-------------|
| `{001}` | 001, 002, 003... | Zero-padded numbers (3 digits) |
| `{0001}` | 0001, 0002, 0003... | Zero-padded numbers (4 digits) |
| `{COUNTER:5}` | 00001, 00002, 00003... | Custom width counter |
| `{A}` | A, B, C... Z, AA, AB... | Uppercase letters |
| `{a}` | a, b, c... z, aa, ab... | Lowercase letters |
| `{I}` | I, II, III, IV, V... | Uppercase Roman numerals |
| `{i}` | i, ii, iii, iv, v... | Lowercase Roman numerals |

**Tips:**
- Patterns work in any name part
- Combine with other text: `Photo_{001}_backup`
- Each selected file gets the next number/letter automatically
- Perfect for batch renaming!

### 🔄 Text Transformations Reference

| Transformation | Example Input | Example Output |
|----------------|--------------|----------------|
| **none** | `My File Name` | `My File Name` |
| **uppercase** | `My File Name` | `MY FILE NAME` |
| **lowercase** | `My File Name` | `my file name` |
| **title** | `my file name` | `My File Name` |
| **sentence** | `my file name` | `My file name` |
| **trim** | `  my file  ` | `my file` |
| **trim_all** | `  my   file  ` | `my file` |
| **remove_spaces** | `My File Name` | `MyFileName` |

### 🔍 File Status Indicators

- **✅ Green "✓ File is available"** - File is ready to be renamed
- **⚠️ Red "⚠ File is currently OPEN"** - File is open in another program
  - The app will attempt to close it before renaming
  - You may need to close it manually if the rename fails

### ↶↷ Undo/Redo System

- **Undo Button** - Reverses the last rename operation(s)
- **Redo Button** - Re-applies undone operations
- **History Limit** - Stores up to 50 operations
- **Button States** - Buttons are disabled when there's nothing to undo/redo
- **Batch Support** - Undo/redo works for both single and batch operations

---

## ⚙️ Settings & Configuration

Settings are automatically saved to `fileforge_settings.json` in the same directory as the executable. This includes:

- ✅ All configuration profiles (name parts, separators, transformations)
- ✅ Currently selected configuration
- ✅ Last used directory
- ✅ All dropdown options and values

**No manual saving required** - everything is saved automatically! 🎉

---

## 🎯 Keyboard Shortcuts

- **Ctrl+Click** - Select multiple individual files
- **Shift+Click** - Select a range of files
- **Click** - Select single file

---

## 💡 Tips & Best Practices

1. **Always Preview First** - Use the preview feature to verify your renaming pattern before applying
2. **Use Undo** - If you make a mistake, the undo feature can quickly reverse changes
3. **Save Configurations** - Create different configurations for different renaming tasks
4. **Batch Operations** - Select multiple files to rename them all at once with automatic numbering
5. **Close Files** - Close files in other programs before renaming for best results

---

## ⚠️ Important Notes

- **Windows Only** - This application is designed for Windows operating systems
- **File Safety** - Always preview changes before renaming. Use undo if needed.
- **Open Files** - Files that are open in other programs may need to be closed manually
- **Settings File** - The `fileforge_settings.json` file is created automatically and stores your preferences

---

## 📝 License

© 2025 **Port42 Developments**

See [LICENSE](LICENSE) file for details.

---

## 🙏 Support

For issues, questions, or feedback, please contact the developer or visit the project repository.

---

<div align="center">

**Made with ❤️ by Port42 Developments**

*Simplifying file management, one rename at a time* 🚀

</div>

