# 🚀 Installation Guide

Complete installation guide for the Employee Data Analysis & Visualization System.

---

## 📋 System Requirements

### Minimum Requirements
- **Operating System:** Windows 10/11, macOS 10.14+, or Linux (Ubuntu 20.04+)
- **Python:** 3.8 or higher
- **RAM:** 4 GB minimum (8 GB recommended)
- **Disk Space:** 500 MB free space
- **Display:** 1920x1080 resolution recommended

### Recommended Requirements
- **Python:** 3.10 or higher
- **RAM:** 8 GB or more
- **Disk Space:** 1 GB free space
- **GPU:** Not required (CPU only)

---

## 🔧 Installation Methods

### Method 1: Quick Install (Recommended)

#### Step 1: Clone Repository
```bash
git clone https://github.com/theabdulwasay/employe-data-analysis.git
cd employee-data-analysis
```

#### Step 2: Create Virtual Environment
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

#### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

#### Step 4: Run the Analysis
```bash
python employee_analysis.py
```

---

### Method 2: Manual Installation

#### Step 1: Install Python
Download and install Python from [python.org](https://www.python.org/downloads/)

Verify installation:
```bash
python --version
# Should show: Python 3.8.x or higher
```

#### Step 2: Install Required Libraries
```bash
pip install pandas numpy matplotlib seaborn scipy
```

#### Step 3: Download Project Files
Download the project ZIP from GitHub and extract it, or clone the repository:
```bash
git clone https://github.com/kashifali/employee-data-analysis.git
```

#### Step 4: Navigate to Project Directory
```bash
cd employee-data-analysis
```

#### Step 5: Run the Script
```bash
python employee_analysis.py
```

---

### Method 3: Anaconda Installation

#### Step 1: Install Anaconda
Download from [anaconda.com](https://www.anaconda.com/products/distribution)

#### Step 2: Create Conda Environment
```bash
conda create -n employee-analysis python=3.10
conda activate employee-analysis
```

#### Step 3: Install Dependencies
```bash
conda install pandas numpy matplotlib seaborn scipy
```

Or use pip within conda:
```bash
pip install -r requirements.txt
```

#### Step 4: Clone and Run
```bash
git clone https://github.com/kashifali/employee-data-analysis.git
cd employee-data-analysis
python employee_analysis.py
```

---

## 📦 Installing Individual Dependencies

If you encounter issues, install dependencies individually:

```bash
# Core data analysis
pip install pandas==1.5.3
pip install numpy==1.24.3

# Visualization
pip install matplotlib==3.7.1
pip install seaborn==0.12.2

# Statistical analysis
pip install scipy==1.10.1
```

---

## 🐧 Platform-Specific Instructions

### Windows

1. **Install Python:**
   - Download from [python.org](https://python.org)
   - Check "Add Python to PATH" during installation

2. **Open Command Prompt:**
   ```cmd
   Win + R → cmd → Enter
   ```

3. **Install Git (Optional):**
   - Download from [git-scm.com](https://git-scm.com)

4. **Follow Method 1 instructions above**

**Common Windows Issues:**
- If `pip` is not recognized, use: `python -m pip install <package>`
- If permissions error, run CMD as Administrator
- If firewall blocks downloads, temporarily disable or add exception

---

### macOS

1. **Install Homebrew (if not installed):**
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Python:**
   ```bash
   brew install python@3.10
   ```

3. **Install Git:**
   ```bash
   brew install git
   ```

4. **Follow Method 1 instructions above**

**Common macOS Issues:**
- If `python` command not found, use `python3`
- If `pip` command not found, use `pip3`
- For permission errors, use `sudo` (not recommended) or fix permissions

---

### Linux (Ubuntu/Debian)

1. **Update Package List:**
   ```bash
   sudo apt update
   ```

2. **Install Python and pip:**
   ```bash
   sudo apt install python3 python3-pip python3-venv
   ```

3. **Install Git:**
   ```bash
   sudo apt install git
   ```

4. **Follow Method 1 instructions above**

**Common Linux Issues:**
- Use `python3` instead of `python`
- Use `pip3` instead of `pip`
- Install python3-dev if compilation errors occur:
  ```bash
  sudo apt install python3-dev
  ```

---

## ✅ Verifying Installation

### Check Python Installation
```bash
python --version
# or
python3 --version
```

Expected output: `Python 3.8.x` or higher

### Check pip Installation
```bash
pip --version
# or
pip3 --version
```

### Test Import All Dependencies
```bash
python -c "import pandas, numpy, matplotlib, seaborn, scipy; print('All packages installed successfully!')"
```

### Run Quick Test
```bash
cd employee-data-analysis
python employee_analysis.py
```

You should see output starting with:
```
================================================================================
                  COMPREHENSIVE EMPLOYEE DATA ANALYSIS SYSTEM                   
================================================================================
```

---

## 🔍 Troubleshooting

### Issue: "python: command not found"
**Solution:**
- Windows: Reinstall Python with "Add to PATH" checked
- macOS/Linux: Use `python3` instead of `python`

### Issue: "No module named 'pandas'"
**Solution:**
```bash
pip install pandas
# or
pip3 install pandas
```

### Issue: "Permission denied"
**Solutions:**
1. Use virtual environment (recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate     # Windows
   ```

2. Or use `--user` flag:
   ```bash
   pip install --user -r requirements.txt
   ```

### Issue: "SSL Certificate Error"
**Solution:**
```bash
pip install --trusted-host pypi.org --trusted-host files.pythonhosted.org -r requirements.txt
```

### Issue: Matplotlib backend errors
**Solution:**
Add to script or use non-interactive backend:
```python
import matplotlib
matplotlib.use('Agg')
```

### Issue: Memory errors with large datasets
**Solution:**
- Increase system RAM
- Process data in chunks
- Use sampling for visualizations

---

## 🆙 Updating the Software

### Update from Git
```bash
cd employee-data-analysis
git pull origin main
```

### Update Dependencies
```bash
pip install --upgrade -r requirements.txt
```

### Update Individual Package
```bash
pip install --upgrade pandas
```

---

## 🗑️ Uninstallation

### Remove Virtual Environment
```bash
# Simply delete the venv folder
rm -rf venv        # macOS/Linux
rmdir /s venv      # Windows
```

### Remove All Packages
```bash
pip uninstall pandas numpy matplotlib seaborn scipy -y
```

### Remove Project
```bash
rm -rf employee-data-analysis  # macOS/Linux
rmdir /s employee-data-analysis  # Windows
```

---

## 🆘 Getting Help

### If Installation Fails:

1. **Check Python Version:**
   ```bash
   python --version
   ```
   Must be 3.8 or higher

2. **Check pip Version:**
   ```bash
   pip --version
   ```

3. **Try Clean Install:**
   ```bash
   pip uninstall -r requirements.txt -y
   pip install -r requirements.txt
   ```

4. **Check System Resources:**
   - Ensure 500 MB free disk space
   - Ensure 2 GB free RAM
   - Close other applications

5. **Contact Support:**
   - GitHub Issues: [Create Issue](https://github.com/kashifali/employee-data-analysis/issues)
   - Email: kashif.ali@example.com

---

## 📚 Additional Resources

- **Python Installation:** https://www.python.org/downloads/
- **pip Documentation:** https://pip.pypa.io/en/stable/
- **Virtual Environments:** https://docs.python.org/3/tutorial/venv.html
- **Anaconda Guide:** https://docs.anaconda.com/anaconda/install/

---

## ✨ Next Steps

After successful installation:

1. **Read the README:** `README.md`
2. **Try Example Notebook:** `examples/example_analysis.ipynb`
3. **Prepare Your Data:** See "Data Requirements" in README
4. **Run Analysis:** `python employee_analysis.py`
5. **View Results:** Check `/outputs` directory

---

**Installation Guide Version:** 1.0  
**Last Updated:** February 2026  
**Maintained by:** Abdul Wasay (FA22-BCS-127)

---

For the latest installation instructions, visit:
**https://github.com/theabdulwasay/employee-data-analysis**
