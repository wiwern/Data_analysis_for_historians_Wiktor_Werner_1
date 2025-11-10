# Course overview / Visión general del curso / Przegląd kursu

---

## 🇬🇧 Course overview (English)

This course introduces basic quantitative methods for historical research using Python and Jupyter Notebook.  
Each notebook focuses on a specific family of analytical techniques and is designed to be applied directly to empirical data (CSV files).

### Notebook 01 – Descriptive statistics for two quantitative variables

**Analytical tasks**

- Load a CSV file and select two quantitative variables.
- Compute standard descriptive statistics:
  - number of observations, mean, standard deviation,
  - minimum, maximum, quartiles, median.
- Visualize each variable:
  - histograms (shape and spread of the distribution),
  - boxplots (median, quartiles, outliers),
  - bar plot of means (comparison of central tendency).

**Theoretical background**

This notebook introduces **descriptive statistics**, which form the basis of quantitative historical research and social science more generally.  
The focus is on understanding:

- how a variable is distributed in a historical population (e.g. wages, prices, population counts),
- how to summarize this distribution with simple numerical indicators and graphical tools,
- how to identify asymmetry, dispersion and extreme values.

The emphasis is not on hypothesis testing but on careful **exploration and description** of the empirical material.

---

### Notebook 02 – Exploratory Data Analysis (EDA) and simple linear regression

**Analytical tasks**

- Load a CSV file and select two quantitative variables.
- Compute descriptive statistics and the Pearson correlation between the variables.
- Produce visualizations:
  - scatter plot showing the relationship between the two variables,
  - histograms for each variable.
- Fit a **simple linear regression** using one variable as predictor and the other as outcome.
- Report the regression equation and the coefficient of determination \(R^2\), with a short textual interpretation.

**Theoretical background**

This notebook introduces **Exploratory Data Analysis (EDA)** and **simple linear regression** as tools for investigating relationships between historical variables.

- EDA emphasizes visual inspection (scatter plots, distributions) and flexible exploration before formal modelling.
- Pearson correlation measures the **strength and direction of a linear association** between two variables.
- Simple linear regression models how changes in one variable are associated, on average, with changes in another.

The notebook stresses that:

- correlation and regression indicate **association, not causality**,
- interpretation must always be grounded in the historical context (period, sources, measurement practices, potential confounders).

---

### Notebook 03 – Time series analysis (decomposition and linear trend)

**Analytical tasks**

- Load a CSV file containing a date column and a quantitative value.
- Convert the date column to a datetime index, sort the series and clean invalid entries.
- Plot the time series to visualize the evolution of the variable over time.
- Optionally perform **additive decomposition** into:
  - trend component,
  - seasonal component,
  - residual (irregular) component.
- Estimate a **linear trend** using regression on a time index and compare the fitted trend line to the original series.

**Theoretical background**

This notebook introduces basic **time series analysis** for historical data, where observations are ordered in time (annual, quarterly, monthly, etc.).

- Decomposition follows classical approaches (e.g. separating trend, seasonality and noise) used in economic and demographic history.
- The linear trend is a simple model of long-term change, summarizing whether a series is increasing, decreasing or stable on average.

The notebook encourages students to interpret:

- how long-term trends relate to known historical processes (wars, reforms, technological change),
- how seasonal or cyclical patterns may reflect institutional or social rhythms.

---

### Notebook 04 – Correspondence analysis for two categorical variables

**Analytical tasks**

- Load a CSV file and select two categorical (qualitative) variables.
- Construct a **contingency table** (cross-tabulation) of the two variables.
- Compute row and column profiles (relative frequencies).
- Perform **correspondence analysis (CA)** using singular value decomposition of standardized residuals.
- Examine eigenvalues and the percentage of inertia explained by each dimension.
- Produce a **biplot** showing row and column categories in the same two-dimensional space.

**Theoretical background**

Correspondence analysis is a method for exploring relationships between **categorical variables** in a contingency table.  
It is widely used in quantitative history, sociology and political science when the data structure is:

- groups × categories (e.g. social class × occupation, region × party, actors × roles).

Key ideas:

- The contingency table is treated as a cloud of points (row and column profiles) in a high-dimensional space.
- CA finds low-dimensional axes (principal dimensions) that best represent the variation (“inertia”) in the table.
- The geometric representation (biplot) allows one to interpret **associations and oppositions** between categories.

The notebook emphasizes that the geometric patterns must be interpreted together with substantive historical knowledge and source criticism.

---

## 🇪🇸 Visión general del curso (Español)

Este curso introduce métodos cuantitativos básicos para la investigación histórica utilizando Python y Jupyter Notebook.  
Cada notebook se centra en una familia específica de técnicas de análisis y está pensado para aplicarse directamente a datos empíricos (archivos CSV).

### Notebook 01 – Estadística descriptiva para dos variables cuantitativas

**Operaciones analíticas**

- Cargar un archivo CSV y seleccionar dos variables cuantitativas.
- Calcular estadísticos descriptivos estándar:
  - número de observaciones, media, desviación estándar,
  - mínimo, máximo, cuartiles, mediana.
- Visualizar cada variable:
  - histogramas (forma y dispersión de la distribución),
  - diagramas de caja (mediana, cuartiles, valores atípicos),
  - gráfico de barras con las medias (comparación de niveles medios).

**Fundamento teórico**

El notebook introduce la **estadística descriptiva**, que constituye la base de la investigación cuantitativa en historia y en ciencias sociales.

El objetivo es comprender:

- cómo se distribuye una variable en una población histórica (salarios, precios, población, etc.),
- cómo resumir esta distribución mediante indicadores numéricos y gráficos sencillos,
- cómo identificar asimetrías, dispersión y valores extremos.

El énfasis está en la **exploración y descripción cuidadosa** del material empírico, más que en pruebas de hipótesis formales.

---

### Notebook 02 – Análisis exploratorio de datos (EDA) y regresión lineal simple

**Operaciones analíticas**

- Cargar un archivo CSV y seleccionar dos variables cuantitativas.
- Calcular estadísticos descriptivos y la correlación de Pearson entre las variables.
- Producir visualizaciones:
  - diagrama de dispersión (relación entre ambas variables),
  - histogramas para cada variable.
- Ajustar una **regresión lineal simple**, utilizando una variable como predictor y la otra como resultado.
- Informar la ecuación de regresión y el coeficiente de determinación \(R^2\), con una interpretación textual breve.

**Fundamento teórico**

Este notebook introduce el **análisis exploratorio de datos (EDA)** y la **regresión lineal simple** como herramientas para investigar relaciones entre variables históricas.

- El EDA enfatiza la inspección visual (diagramas de dispersión, distribuciones) y la exploración flexible antes de la modelización formal.
- La correlación de Pearson mide la **fuerza y dirección de la asociación lineal** entre dos variables.
- La regresión lineal simple modeliza cómo los cambios en una variable se asocian, en promedio, con cambios en otra.

Se subraya que:

- correlación y regresión indican **asociación, no causalidad**,
- la interpretación debe situarse siempre en el contexto histórico (periodización, fuentes, prácticas de medición, posibles variables omitidas).

---

### Notebook 03 – Análisis de series temporales (descomposición y tendencia lineal)

**Operaciones analíticas**

- Cargar un archivo CSV con una columna de fecha y una variable cuantitativa.
- Convertir la columna de fecha en un índice de tipo datetime, ordenar la serie y limpiar valores no válidos.
- Representar la serie temporal para visualizar la evolución de la variable en el tiempo.
- Realizar, opcionalmente, una **descomposición aditiva** en:
  - componente de tendencia,
  - componente estacional,
  - componente residual (irregular).
- Estimar una **tendencia lineal** mediante regresión sobre un índice temporal y compararla con la serie original.

**Fundamento teórico**

El notebook introduce elementos básicos del **análisis de series temporales** aplicados a datos históricos (anuales, trimestrales, mensuales, etc.).

- La descomposición sigue enfoques clásicos que separan tendencia, estacionalidad y ruido, habituales en historia económica y demográfica.
- La tendencia lineal es un modelo sencillo del cambio a largo plazo, que resume si la serie aumenta, disminuye o permanece estable, en promedio.

Se invita a los estudiantes a interpretar:

- cómo las tendencias de largo plazo se relacionan con procesos históricos conocidos (guerras, reformas, cambios tecnológicos),
- cómo los patrones estacionales o cíclicos pueden reflejar ritmos institucionales o sociales.

---

### Notebook 04 – Análisis de correspondencias para dos variables categóricas

**Operaciones analíticas**

- Cargar un archivo CSV y seleccionar dos variables categóricas (cualitativas).
- Construir una **tabla de contingencia** (tabulación cruzada) de las dos variables.
- Calcular perfiles de filas y columnas (frecuencias relativas).
- Realizar un **análisis de correspondencias (AC)** mediante descomposición en valores singulares de los residuos estandarizados.
- Examinar los autovalores y el porcentaje de inercia explicado por cada dimensión.
- Producir un **biplot** que muestra categorías de filas y de columnas en el mismo plano bidimensional.

**Fundamento teórico**

El análisis de correspondencias es un método para explorar relaciones entre **variables categóricas** en una tabla de contingencia.  
Se utiliza ampliamente en historia cuantitativa, sociología y ciencia política cuando la estructura de los datos es:

- grupos × categorías (por ejemplo, clase social × ocupación, región × partido, actores × roles).

Ideas clave:

- La tabla de contingencia se interpreta como una nube de puntos (perfiles de filas y columnas) en un espacio de alta dimensión.
- El AC identifica ejes de baja dimensión (dimensiones principales) que capturan la mayor parte de la variación (“inercia”) de la tabla.
- La representación geométrica (biplot) permite interpretar **asociaciones y oposiciones** entre categorías.

El notebook insiste en que los patrones geométricos deben interpretarse junto con el conocimiento sustantivo del contexto histórico y con una lectura crítica de las fuentes.

---

## 🇵🇱 Przegląd kursu (Polski)

Kurs wprowadza podstawowe metody ilościowe w badaniach historycznych z wykorzystaniem Pythona i środowiska Jupyter Notebook.  
Każdy notebook koncentruje się na określonym typie analizy i jest pomyślany tak, aby można go bezpośrednio zastosować do danych empirycznych (pliki CSV).

### Notebook 01 – Statystyka opisowa dla dwóch zmiennych ilościowych

**Czynności analityczne**

- Wczytanie pliku CSV i wybór dwóch zmiennych ilościowych.
- Obliczenie standardowych statystyk opisowych:
  - liczba obserwacji, średnia, odchylenie standardowe,
  - minimum, maksimum, kwartyle, mediana.
- Wizualizacja każdej zmiennej:
  - histogramy (kształt i rozproszenie rozkładu),
  - wykresy pudełkowe (mediana, kwartyle, obserwacje odstające),
  - wykres słupkowy średnich (porównanie poziomu przeciętnego).

**Umocowanie teoretyczne**

Notebook wprowadza **statystykę opisową**, stanowiącą fundament badań ilościowych w historii i naukach społecznych.

Chodzi o zrozumienie:

- jak rozkłada się dana cecha w populacji historycznej (np. płace, ceny, liczebność ludności),
- jak streścić ten rozkład prostymi wskaźnikami liczbowymi i wykresami,
- jak identyfikować asymetrię, rozproszenie i wartości skrajne.

Akcent położony jest na **eksplorację i opis** materiału empirycznego, a nie na formalne testowanie hipotez.

---

### Notebook 02 – Exploratory Data Analysis (EDA) i prosta regresja liniowa

**Czynności analityczne**

- Wczytanie pliku CSV i wybór dwóch zmiennych ilościowych.
- Obliczenie statystyk opisowych oraz korelacji Pearsona między zmiennymi.
- Wizualizacje:
  - wykres rozrzutu (relacja między dwiema zmiennymi),
  - histogramy dla każdej zmiennej.
- Dopasowanie **prostej regresji liniowej**, z jedną zmienną jako predyktorem, drugą jako zmienną objaśnianą.
- Podanie równania regresji oraz współczynnika determinacji \(R^2\) wraz z krótką interpretacją.

**Umocowanie teoretyczne**

Notebook wprowadza **analizę eksploracyjną danych (EDA)** oraz **prostą regresję liniową** jako narzędzia badania związków między zmiennymi historycznymi.

- EDA kładzie nacisk na oglądowe, wizualne rozpoznanie danych (wykresy rozrzutu, rozkłady) przed konstrukcją bardziej złożonych modeli.
- Korelacja Pearsona mierzy **siłę i kierunek liniowej zależności** między dwiema zmiennymi.
- Prosta regresja liniowa opisuje, jak zmiany jednej zmiennej wiążą się – przeciętnie – ze zmianami drugiej.

Podkreślane jest, że:

- korelacja i regresja mówią o **związku, a nie o przyczynowości**,
- interpretacja musi być zakorzeniona w kontekście historycznym (chronologia, źródła, praktyki pomiaru, możliwe zmienne pominięte).

---

### Notebook 03 – Analiza szeregów czasowych (dekompozycja i trend liniowy)

**Czynności analityczne**

- Wczytanie pliku CSV z kolumną daty i zmienną ilościową.
- Konwersja kolumny daty do indeksu typu datetime, uporządkowanie szeregu, oczyszczenie błędnych wartości.
- Narysowanie szeregu czasowego, aby zobaczyć przebieg zmiennej w czasie.
- Opcjonalnie: wykonanie **dekompozycji addytywnej** na:
  - komponent trendu,
  - komponent sezonowy,
  - komponent resztowy (losowy).
- Oszacowanie **trendu liniowego** za pomocą regresji względem indeksu czasowego i porównanie linii trendu z szeregiem empirycznym.

**Umocowanie teoretyczne**

Notebook wprowadza podstawy **analizy szeregów czasowych** w zastosowaniu do danych historycznych (np. rocznych, kwartalnych, miesięcznych).

- Dekompozycja na trend, sezonowość i składnik losowy odwołuje się do klasycznych ujęć obecnych w historii gospodarczej i demograficznej.
- Trend liniowy stanowi prosty model zmiany długookresowej, pokazujący, czy w badanym okresie dominuje tendencja wzrostowa, spadkowa czy względna stabilność.

Studenci zachęcani są do interpretacji:

- jak trendy długookresowe wiążą się z procesami historycznymi (wojny, reformy, zmiany technologiczne),
- jak wzory sezonowe lub cykliczne odzwierciedlają rytmy instytucjonalne lub społeczne.

---

### Notebook 04 – Analiza korespondencji dla dwóch zmiennych jakościowych

**Czynności analityczne**

- Wczytanie pliku CSV i wybór dwóch zmiennych jakościowych.
- Zbudowanie **tablicy kontyngencji** (tablicy krzyżowej) dla tych zmiennych.
- Obliczenie profili wierszy i kolumn (udziałów względnych).
- Przeprowadzenie **analizy korespondencji (CA)** poprzez dekompozycję wartości osobliwych znormalizowanych reszt.
- Analiza wartości własnych i odsetka inercji wyjaśnianej przez kolejne wymiary.
- Utworzenie **biplotu**, na którym kategorie wierszy i kolumn przedstawione są we wspólnej przestrzeni dwuwymiarowej.

**Umocowanie teoretyczne**

Analiza korespondencji jest metodą eksploracji zależności między **zmiennymi kategorialnymi** zapisanymi w tablicy kontyngencji.  
Stosuje się ją szeroko w historii ilościowej, socjologii czy naukach politycznych, gdy dane mają strukturę:

- grupy × kategorie (np. klasa społeczna × zawód, region × partia, aktorzy × role).

Kluczowe idee:

- Tablica kontyngencji traktowana jest jako zbiór punktów (profili wierszy i kolumn) w przestrzeni wielowymiarowej.
- Analiza korespondencji wyznacza wymiary główne (osie), które najlepiej oddają zróżnicowanie („inercję”) w tablicy.
- Geometryczna reprezentacja (biplot) pozwala interpretować **podobieństwa, przeciwstawienia i skojarzenia** między kategoriami.

Notebook akcentuje, że obserwowane konfiguracje geometryczne muszą być interpretowane łącznie z wiedzą o kontekście historycznym i z krytyczną analizą źródeł.

