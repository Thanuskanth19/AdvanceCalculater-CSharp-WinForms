# AdvanceCalculater (Windows Forms)

A simple, multi‑feature **Advanced Calculator** built with **C# (.NET) Windows Forms**. 
It includes basic arithmetic, scientific functions, a **unit converter**, and a **temperature converter**, with a splash screen and WinForms UI.

## ✨ Features
- Standard calculator operations (add, subtract, multiply, divide)
- Scientific functions (trig, power, etc.) — see forms in `/AdvanceCalculater/AdvanceCalculater/`
- **Unit Converter** and **Temperature Converter** forms
- Windows Forms UI with a splash screen

## 📁 Project Structure
```
/AdvanceCalculater.sln                # Solution
/AdvanceCalculater/AdvanceCalculater  # WinForms project
├─ *.cs, *.Designer.cs, *.resx       # Forms and resources
├─ App.config                         # App configuration
├─ bin/, obj/                         # Build outputs (git-ignored)
└─ Properties/                        # Assembly info & resources
```

## 🛠️ Build & Run

### Option A — Visual Studio (recommended)
1. Open **`AdvanceCalculater.sln`** in **Visual Studio 2019/2022** on Windows.
2. Set configuration to **Debug** and target **x86** or **Any CPU**.
3. **Build** → **Build Solution** (Ctrl+Shift+B).
4. **Start** (F5). The app launches with the splash screen and main form.

> If packages are needed, Visual Studio will restore them automatically.

### Option B — .NET CLI (if SDK-style project)
> Some WinForms projects target .NET Framework and require Visual Studio on Windows. 
> If this project is SDK-style and targets .NET (>= 6), you can try:
```bash
dotnet restore
dotnet build
dotnet run --project AdvanceCalculater/AdvanceCalculater/AdvanceCalculater.csproj
```

## 🧪 Manual Tests
- Open the **Unit Converter** and **Temperature Converter** forms and verify conversions.
- Check scientific operations edge cases (division by zero, large exponents).
- Resize the window and confirm controls remain usable.

## 📦 Create a Release (Windows .exe)
1. In Visual Studio: **Build** → **Publish** → **Folder** (or use ClickOnce).
2. Choose **Release** configuration for optimized binaries.
3. Upload the generated folder as a **GitHub Release** asset (see steps below).

## 🚀 How to Upload This Project to GitHub

### 1) Create a repository
- Suggested name: **AdvanceCalculater**
- Initialize **without** a README (we already have one).

### 2) Prepare local folder
Place the project folder on your PC (for example: `C:\Projects\AdvanceCalculater`).

### 3) Run these commands
```bash
cd C:\Projects\AdvanceCalculater

git init
git branch -M main

# Ignore build artifacts & VS files
copy NUL .gitignore >NUL
# (We already include a .gitignore in this repo; skip the above line if present)

git add .
git commit -m "Initial commit: AdvanceCalculater WinForms v1.0"

git remote add origin https://github.com/<your-username>/AdvanceCalculater.git
git push -u origin main

# (optional) tag a version and push it
git tag v1.0.0 -m "Initial release"
git push origin v1.0.0
```

### 4) Add screenshots (optional)
Create a `screenshots/` folder and add PNG/JPG images. 
Then reference them in this README.

### 5) Create a GitHub Release (optional)
- Go to **Releases** → **Draft a new release**
- Tag: `v1.0.0`, Title: `AdvanceCalculater v1.0.0`
- Attach your published **.zip** or **Setup.exe**

## 📜 License
This project is licensed under the **MIT License** (see `LICENSE`).

---

**Author:** Thanuskanth  
**Year:** 2025
