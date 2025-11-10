
## 🇬🇧 English – How to use this course

### 0. Install Python and Jupyter

* Install **Python 3** (e.g. from [python.org](https://www.python.org) or Anaconda).
* In a terminal / command prompt:

```bash
pip install jupyter pandas numpy matplotlib statsmodels
```

(If you use Anaconda, większość tego już jest.)

---

### 1. Download the course to your computer

Option A – with git:

```bash
git clone https://github.com/USER/REPO.git
cd REPO
```

Option B – without git:

1. On GitHub: click **“Code” → “Download ZIP”**.
2. Unzip the file.
3. Open a terminal in that folder.

---

### 2. Start Jupyter and open the notebooks

In the course folder:

```bash
jupyter notebook
```

Then in the browser:

1. Go to the `notebooks/` directory.
2. Open one of:

   * `01_descriptive_statistics.ipynb`
   * `02_eda_linear_regression.ipynb`
   * `03_time_series_analysis.ipynb`
   * `04_correspondence_analysis.ipynb`
3. Run the cells from top to bottom.

---

### 3. Load your data into the code

1. Put your **CSV file** in the main folder or in `data/`, e.g.:

   * `data/example_two_variables.csv`

2. When the notebook asks for the file name, type something like:

   ```text
   data/example_two_variables.csv
   ```

   (Always include `.csv`.)

3. When asked for **column names**, type them exactly as in the file
   (e.g. `value1`, `value2`, `Date`, `Close`, `region`, `party`, etc.).

4. The notebook will:

   * load the data,
   * show first rows,
   * and then run the analysis (statistics, plots, etc.).

---

## 🇪🇸 Español – Cómo usar este curso

### 0. Instalar Python y Jupyter

* Instala **Python 3** (por ejemplo desde [python.org](https://www.python.org) o Anaconda).
* En una terminal:

```bash
pip install jupyter pandas numpy matplotlib statsmodels
```

(Si usas Anaconda, la mayoría ya viene instalada.)

---

### 1. Descargar el curso al ordenador

Opción A – con git:

```bash
git clone https://github.com/USER/REPO.git
cd REPO
```

Opción B – sin git:

1. En GitHub: haz clic en **“Code” → “Download ZIP”**.
2. Descomprime el archivo ZIP.
3. Abre una terminal en esa carpeta.

---

### 2. Abrir los notebooks en Jupyter

En la carpeta del curso:

```bash
jupyter notebook
```

En el navegador:

1. Entra en el directorio `notebooks/`.
2. Abre uno de estos archivos:

   * `01_descriptive_statistics.ipynb`
   * `02_eda_linear_regression.ipynb`
   * `03_time_series_analysis.ipynb`
   * `04_correspondence_analysis.ipynb`
3. Ejecuta las celdas desde arriba hacia abajo.

---

### 3. Cargar tus datos en el código

1. Coloca tu archivo **CSV** en la carpeta principal o en `data/`, por ejemplo:

   * `data/example_two_variables.csv`

2. Cuando el notebook pida el nombre del archivo, escribe algo como:

   ```text
   data/example_two_variables.csv
   ```

   (Siempre con la extensión `.csv`.)

3. Cuando pida los **nombres de las columnas**, escríbelos exactamente como aparecen en el archivo
   (por ejemplo: `value1`, `value2`, `Date`, `Close`, `region`, `party`, etc.).

4. El notebook:

   * carga los datos,
   * muestra las primeras filas,
   * y luego ejecuta el análisis (estadística, gráficos, etc.).

---

## 🇵🇱 Polski – Jak korzystać z kursu

### 0. Instalacja Pythona i Jupytera

* Zainstaluj **Python 3** (np. z [python.org](https://www.python.org) albo Anacondę).
* W terminalu / PowerShellu:

```bash
pip install jupyter pandas numpy matplotlib statsmodels
```

(Przy Anacondzie większość pakietów już jest.)

---

### 1. Ściągnięcie kursu na komputer

Opcja A – z gitem:

```bash
git clone https://github.com/USER/REPO.git
cd REPO
```

Opcja B – bez gita:

1. Na GitHubie kliknij **„Code” → „Download ZIP”**.
2. Rozpakuj ZIP.
3. Otwórz terminal w tym katalogu.

---

### 2. Uruchomienie notebooków w Jupyterze

W katalogu kursu:

```bash
jupyter notebook
```

W przeglądarce:

1. Wejdź do folderu `notebooks/`.
2. Otwórz wybrany notebook:

   * `01_descriptive_statistics.ipynb`
   * `02_eda_linear_regression.ipynb`
   * `03_time_series_analysis.ipynb`
   * `04_correspondence_analysis.ipynb`
3. Uruchamiaj komórki po kolei, od góry do dołu.

---

### 3. Wczytanie danych do kodu

1. Włóż swój plik **CSV** do folderu repozytorium, najlepiej do `data/`, np.:

   * `data/example_two_variables.csv`

2. Gdy notebook poprosi o nazwę pliku, wpisz np.:

   ```text
   data/example_two_variables.csv
   ```

   (Zawsze z `.csv` na końcu.)

3. Gdy poprosi o **nazwy kolumn**, wpisz je dokładnie tak, jak są w pliku
   (np. `value1`, `value2`, `Date`, `Close`, `region`, `party` itd.).

4. Notebook:

   * wczyta dane,
   * pokaże kilka pierwszych wierszy,
   * a potem wykona analizę (statystyki, wykresy itd.).

