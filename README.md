Step-by-Step Guide to Add Your Project to GitHub

Your current folder:

D:\Projects\Modular Monolithic Architecture

Inside it:

Backend
Frontend

We will:

Create Git files
Initialize Git
Create GitHub repository
Push code to GitHub



STEP 1 — Open Your Project Folder

Open:

D:\Projects\Modular Monolithic Architecture



STEP 2 — Open Terminal Here

Inside this folder:

Method 1

Right click empty space → Open in Terminal

Method 2

Click address bar and type:

cmd

then press Enter.

Now terminal opens in:

D:\Projects\Modular Monolithic Architecture>



STEP 3 — Initialize Git

In terminal run:

git init

After this, hidden .git folder gets created.



STEP 4 — Create .gitignore File

Where to create?

Create inside:

D:\Projects\Modular Monolithic Architecture

Same level as:

Backend
Frontend



How to create?

Method 1 (Easy)

Right click → New → Text Document

Rename:

.gitignore

IMPORTANT:
Remove .txt

If Windows warns:

Are you sure?

Click YES.



Final structure

Modular Monolithic Architecture
│
├── Backend
├── Frontend
└── .gitignore



STEP 5 — Add Content Inside .gitignore

Open .gitignore in Notepad.

Paste this:

# .NET
bin/
obj/
.vs/
*.user
*.suo

# Angular / Node
node_modules/
dist/

# Logs
*.log

# Environment
.env

# OS
Thumbs.db
.DS_Store

Save file.



STEP 6 — Verify Git Status

In terminal:

git status

You should see:

Backend
Frontend
.gitignore



STEP 7 — Add Files to Git

Run:

git add .

This stages all files.



STEP 8 — Commit Files

Run:

git commit -m "Initial modular monolith setup"



STEP 9 — Create GitHub Repository

Go to:

GitHub Create Repository



Repository Name

Example:

modular-monolith-architecture



IMPORTANT SETTINGS

Keep UNCHECKED:

Add README
Add .gitignore
Add License

Because already local project exists.

Then click:

Create Repository



STEP 10 — Copy Repository URL

After repo creation you will get:

Example:

https://github.com/yourusername/modular-monolith-architecture.git

Copy it.



STEP 11 — Connect Local Project to GitHub

Go back terminal.

Run:

git remote add origin https://github.com/yourusername/modular-monolith-architecture.git

Replace:

yourusername
repository name



STEP 12 — Push Project to GitHub

Run:

git branch -M main

Then:

git push -u origin main



STEP 13 — Login Popup

GitHub login popup may open.

Login with:

GitHub username
Password / token

After success:

Code uploads to GitHub.



FINAL STRUCTURE

Modular Monolithic Architecture
│
├── Backend
│
├── Frontend
│
├── .gitignore
│
└── .git



Recommended Backend Structure

Inside Backend create:

Backend
│
└── src
    │
    ├── API
    │
    ├── BuildingBlocks
    │
    ├── Modules
    │   ├── Identity
    │   ├── AWB
    │   ├── Booking
    │   └── Customer
    │
    └── Shared



Recommended Frontend Structure

Frontend
│
└── angular-app



Very Important

Before pushing:

remove bin
remove obj
remove node_modules

.gitignore handles this automatically.



Verify Git Installed

If git command not working:

Download Git:

Git Download

Install with default settings.