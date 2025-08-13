## 📘 Learning Path Generator 🤖

A **Streamlit-powered web app** that generates personalized learning paths using the **Google Gemini** model and curated YouTube content. Paths can optionally be saved to **Google Drive** or **Notion** using **Pipedream MCP servers**.


## 🔐 Prerequisites

Before getting started, make sure you have:

- ✅ Gemini API Key  
- ✅ Authorized Pipedream URLs for YouTube (required), Google Drive (optional), and Notion (optional)


## 🔑 How to Get the Gemini API Key

1. Go to [Google AI Studio](https://makersuite.google.com/).
2. Sign in with your Google account.
3. Click **“Get API key”** in the left sidebar.
4. Click **“Create API Key”** at the top right.
5. Click **“Create API Key in New Project”** (or use an existing project).
6. Click **Copy** to store your API key securely.


## 🔄 How to Get Pipedream MCP Server URLs

1. Navigate to [Pipedream](https://pipedream.com/) and sign in using your Google account.

### Required:
- [YouTube Data MCP Server](https://pipedream.com/new)  
  > Connect Google → Grant permissions → Copy endpoint URL

### Optional:
- [Google Drive MCP Server](https://pipedream.com/new)
- [Notion MCP Server](https://pipedream.com/new)

> Follow the same steps: Connect → Authorize → Copy endpoint URL

## 💻 Project Setup Guide

### Prerequisites

- Terminal or command prompt
- [Cursor IDE](https://www.cursor.sh/)
- Python 3.10+ installed  
  - [Install Python on Windows](https://realpython.com/installing-python/)
  - [Install Python on macOS](https://docs.python-guide.org/starting/install3/osx/)
  - [Update Python on Windows – Quick Guide](https://phoenixnap.com/kb/update-python)


## ⚙️ Setup Steps

### Step 1: Clone the Repository

#### Option A: Using Git (Recommended)
```bash
git clone <your-github-repo-link>
cd <your-repo-folder-name>
```

#### Option B: Manual Download
- Go to your [GitHub Repo](https://github.com/)
- Click **Code → Download ZIP**
- Unzip the file in your Downloads folder

### Step 2: Open in Cursor IDE
1. Launch **Cursor IDE**
2. Go to **File → Open Folder**
3. Select your unzipped project folder


### Step 3: Create a Virtual Environment named `venv`
```bash
python -m venv venv
```
> This creates a virtual environment named `venv` inside your project folder.


### Step 4: Activate the Virtual Environment

#### On macOS/Linux:
```bash
source venv/bin/activate
```

#### On Windows (Command Prompt):
```cmd
venv\Scripts\activate
```

> After activation, you should see a prompt like:  
> `(venv) yourusername@yourmachine:~/project-folder$`


### Step 5: Install Requirements
```bash
pip install -r requirements.txt
```


### Step 6: Run the Application
```bash
streamlit run app.py
```

> The app will open automatically at: [http://localhost:8501](http://localhost:8501)


## 🛠️ Configuration in App Sidebar

1. Paste your **Gemini API Key**
2. Paste your **YouTube Pipedream URL**
3. Choose either **Google Drive** or **Notion** and paste the respective URL
4. Enter your **learning goal**
5. Click **"Generate Learning Path"**


## ✅ You’re Ready to Learn!

This app takes your goal, finds top YouTube content, and lays out a personalized learning journey — optionally saving it to the cloud.
