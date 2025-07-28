# VoidShield Antivirus

VoidShield Antivirus is a free, open-source desktop antivirus tool written in C# and Windows Forms. It gives you basic protection with on-demand scanning, a quarantine manager, customizable themes, and an optional login screen—all with a sleek, futuristic UI that adapts to high-DPI displays and window resizing.

---

## Features

- **Login Screen** (optional)  
  Simple in-memory user authentication (admin/password123 by default).

- **Dashboard**  
  - Start on-demand virus scan (simulated progress bar)  
  - View and manage quarantined items (delete/restore)  
  - Access settings

- **Settings**  
  - Toggle real-time protection flag (in-memory)  
  - Choose Dark or Light theme

- **Resizable & DPI-Aware UI**  
  - `AutoScaleMode = Dpi` for crisp scaling at any Windows scale factor  
  - Sizable window with sensible minimum size  
  - Anchored controls and layout panels

- **Custom App Icon**  
  - Automatically loads `VoidShield.ico` from your Documents folder  
  - Fallback to default if icon not found

- **Status & Warning**  
  - “You have Basic Protection” status label  
  - “Do not close this application when in use!” warning

---

## Prerequisites

- Windows 10 or newer  
- [.NET 6.0 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/6.0) (or later)  
- Visual Studio 2022 (optional, for development)

---

## Installation & Build

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your-username/VoidShield.git
   cd VoidShield

- Open in Visual Studio
- Double-click VoidShield.sln
- Restore NuGet packages (if prompted)
- Set custom icon (optional)
- Place your VoidShield.ico in %USERPROFILE%\Documents\VoidShield.ico
- The app will automatically load it at runtime
- Build & Run
- Press F5 (Debug) or Ctrl+F5 (Run without debugging)

## Usage
- Login
- Enter admin / password123 (default credentials)
- Or add your own users in the in-memory Dictionary
- Dashboard
- Click Start Scan to simulate scanning
- Click View Quarantine to manage threats
- Click Settings to toggle theme and protection
- Quarantine
- Select an item and Delete or Restore
- Settings
- Enable/disable real-time protection flag (no real effect)
- Switch between Dark and Light themes
- Resize & Scale
- Drag window edges or maximize/minimize freely
- UI elements will reposition and scale automatically

## Project Structure
/VoidShield
```
├─ /VoidShield.sln
├─ /WindowsFormsApp2
│  ├─ Form1.cs
│  ├─ Form1.Designer.cs
│  ├─ Program.cs
│  ├─ AppSettings.cs
│  └─ ThreatItem.cs
└─ README.md
```

- Form1.cs: Main UI logic (login, dashboard, scan, quarantine, settings)
- Form1.Designer.cs: Auto-generated form initialization
- Program.cs: Entry point (launches Form1)
- AppSettings.cs: Simple settings model
- ThreatItem.cs: Data model for quarantined threats

## Contributing
- Fork the repository
- Create a feature branch (git checkout -b feature/YourFeature)
- Commit your changes (git commit -m "Add your feature")
- Push to your branch (git push origin feature/YourFeature)
- Open a Pull Request
Please keep contributions scoped, document new functionality, and follow the existing coding style.

## License
This project is licensed under the MIT License. See LICENSE for details.

Built with ♥ by the VoidShield community.
