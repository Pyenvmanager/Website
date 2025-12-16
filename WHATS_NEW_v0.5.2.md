# What's New in PyEnvManager v0.5.2

Welcome to PyEnvManager v0.5.2! This release brings exciting new features that make creating and managing Python environments even easier.

## 🎉 Create Environments Two Ways!

### Choose Your Style: Mamba or venv

When you create a new environment, you now have **two options** to pick from:

#### 🟢 Mamba (All-in-One)
Perfect if you want everything handled for you!

**What you get:**
- No need to install Python first - we've got you covered
- Choose any Python version from 3.7 to **3.13** (yes, we support the latest!)
- Works with conda packages
- Everything is self-contained

**Best for:**
- Beginners who want a simple setup
- Data science and machine learning projects
- When you need a specific Python version
- Projects that use conda packages

#### 🟢 venv (Use Your Python)
Perfect if you already have Python on your computer!

**What you get:**
- Uses Python that's already installed on your system
- Lightweight and fast
- Standard Python workflow
- We automatically find your Python installations

**Best for:**
- You already have Python installed
- Web development projects
- Quick project setups
- Standard Python workflows

## ✨ New Python Version Support

**Python 3.13 is here!** Stay ahead with support for the latest Python release. You can now create Mamba environments with Python 3.13.

## 🎨 Better Environment Creation Experience

### Smart Python Detection
When you choose venv, PyEnvManager automatically finds all Python installations on your computer and shows them to you. No more guessing!

### Can't Find Your Python? No Problem!
If your Python installation isn't detected, you can:
- **Type the path manually** - Just paste the location of your Python executable
- **Browse for it** - Click "Browse..." and we'll help you find it

### Visual Feedback
- Beautiful new design with **emerald green** highlighting for selected options
- See exactly what's happening during environment creation
- Real-time progress updates in the terminal view

## 📚 How to Create Your First Environment

### Step 1: Click "Create New Environment"

Look for the button on your main screen.

### Step 2: Choose Your Type

Pick between **Mamba** or **venv**. The selected card will light up in green!

**Not sure which one?** → Choose Mamba! It's the easiest option.

### Step 3: Pick Your Python Version

- **For Mamba:** Simply choose from the dropdown (Python 3.7 through 3.13)
- **For venv:** We'll show you what's installed, or you can browse for Python yourself

### Step 4: Name It

Give your environment a name like `my-web-project` or `data-analysis-2024`

### Step 5: Add Packages (Optional)

Want to install packages right away? Type them in:
```
requests flask pandas numpy
```

### Step 6: Click Create!

Watch as your environment is created in real-time. You'll see everything that's happening in the terminal output.

## 🌟 Quick Comparison

| Feature | Mamba | venv |
|---------|-------|------|
| **Requires Python Installed** | ❌ No | ✅ Yes |
| **Python Versions Available** | Any (3.7-3.13) | What you have installed |
| **Setup Speed** | Medium | Fast |
| **Size on Disk** | Larger | Smaller |
| **Package Support** | Conda + pip | pip only |
| **Best For** | Beginners, Data Science | Experienced users, Web Dev |

## 💡 Pro Tips

### Tip 1: Start with Mamba
If you're new to Python environments, start with Mamba. It handles everything for you!

### Tip 2: Use venv for Lightweight Projects
If you already have Python and want quick, lightweight environments, venv is perfect.

### Tip 3: Try Python 3.13
The latest Python version brings performance improvements and new features. Give it a try with Mamba!

### Tip 4: Name Your Environments Well
Use descriptive names like `django-blog-2024` instead of `env1` or `test`

### Tip 5: Add Core Packages During Creation
Install commonly used packages during creation to save time later:
- For data science: `pandas numpy matplotlib jupyter`
- For web dev: `flask requests python-dotenv`

## 🔧 Examples

### Example 1: Quick Data Science Environment
```
Type: Mamba
Python: 3.11
Name: data-analysis
Packages: pandas numpy matplotlib jupyter
```

### Example 2: Web Development with Your Python
```
Type: venv
Python: Auto-detected Python 3.12
Name: flask-website
Packages: flask flask-sqlalchemy
```

### Example 3: Testing Python 3.13
```
Type: Mamba
Python: 3.13
Name: python313-test
Packages: (none - add later)
```

## 🆘 Common Questions

### Q: Which should I choose - Mamba or venv?
**A:** If you're unsure, choose Mamba. It's easier and doesn't require Python to be installed first.

### Q: Can I use both types?
**A:** Absolutely! You can have some environments as Mamba and others as venv. Mix and match based on your needs.

### Q: What if I don't see my Python installation?
**A:** Click "Custom Python executable..." in the dropdown, then either type the path or click "Browse..." to find it.

### Q: Is Python 3.13 stable?
**A:** Yes! Python 3.13 is the latest official release. Some packages may still be catching up with compatibility, so check your specific packages.

### Q: Will this work on Mac/Linux?
**A:** Yes! Both Mamba and venv work on Windows, macOS, and Linux.

### Q: Can I still use my old environments?
**A:** Yes! This update is fully backward compatible. Your existing environments will work exactly as before.

## 🎓 Learn More

Want to dive deeper? Check out our detailed documentation:
- [Full venv Support Guide](VENV_SUPPORT.md) - Technical details and troubleshooting
- [Creating Environments Guide](CREATING_ENVIRONMENTS_GUIDE.md) - Step-by-step tutorial with pictures

## 🚀 Getting Started

Ready to try it out?

1. **Update PyEnvManager** to version 0.5.2
2. Click **"Create New Environment"**
3. Pick your style - **Mamba** or **venv**
4. Follow the prompts
5. Start coding!

---

**Have feedback?** We'd love to hear from you! Let us know what you think about the new features.

**Questions?** Check our documentation or reach out for support.

**Enjoying PyEnvManager?** Consider upgrading to Pro for advanced features like security scanning and SBOM export!

---

*Updated: November 2025*
