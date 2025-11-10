# Python and Jupyter Notebook – Installation Guide  
# Guía de instalación de Python y Jupyter Notebook

This document explains how to install **Python 3** and **Jupyter Notebook** on **Windows**, **macOS** and **Linux**.  
Este documento explica cómo instalar **Python 3** y **Jupyter Notebook** en **Windows**, **macOS** y **Linux**.

---

## Part I – English

### 1. Goal

By the end of this guide you will have:

- A working installation of **Python 3**  
- The **Jupyter Notebook** environment  
- A simple way to start Jupyter and create notebooks for the course  

You can choose between:

- **Option A – Anaconda (recommended for beginners)**  
- **Option B – “Pure” Python + `pip` + Jupyter**

Both are acceptable for the course.

---

### 2. Option A – Install Anaconda (recommended)

Anaconda is a distribution of Python that includes many scientific libraries and Jupyter Notebook out of the box.

#### 2.1. Windows (Anaconda)

1. Go to the official website:  
   <https://www.anaconda.com/download>
2. Download the **Anaconda Distribution for Windows** (64-bit, Python 3).
3. Run the installer (`.exe`) and follow the steps:
   - Choose **“Just Me”** (recommended) unless you know you need “All Users”.
   - Keep the default installation path unless you have a specific reason to change it.
   - When asked about **“Add Anaconda to my PATH environment variable”**, you can leave it **unchecked** (recommended).
4. Finish the installation.

**Start Jupyter Notebook (Windows, Anaconda):**

1. Open the **Start menu**.
2. Search for **“Anaconda Navigator”** and open it.
3. In Anaconda Navigator, find **“Jupyter Notebook”** and click **Launch**.
4. A browser window should open at `http://localhost:8888` with the Jupyter file browser.

---

#### 2.2. macOS (Anaconda)

1. Go to:  
   <https://www.anaconda.com/download>
2. Download the **Anaconda Distribution for macOS** (choose Apple Silicon or Intel according to your Mac).
3. Open the downloaded installer (`.pkg`) and follow the installation wizard.
4. Accept the default options unless you have specific needs.

**Start Jupyter Notebook (macOS, Anaconda):**

- **Option 1 – Anaconda Navigator**
  1. Open **Launchpad**, search for **“Anaconda Navigator”**, and start it.
  2. Click **Launch** under **Jupyter Notebook**.

- **Option 2 – Terminal**
  1. Open **Terminal**.
  2. (Optional) Activate the `base` environment:
     ```bash
     conda activate base
     ```
  3. Run:
     ```bash
     jupyter notebook
     ```

A browser window should open automatically.

---

#### 2.3. Linux (Anaconda)

1. Go to:  
   <https://www.anaconda.com/download>
2. Download the **Linux installer** (`.sh` file).
3. Open a terminal and navigate to your `Downloads` folder, for example:
   ```bash
   cd ~/Downloads

