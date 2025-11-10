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

### Notebook 03b – Time series analysis with a causal moment (CausalImpact)

**Analytical tasks**

- Load a CSV file and select:
  - a date column,
  - a numeric value column representing the historical series of interest.
- Ask the user to provide an approximate **critical / causal date** (e.g. the date of a reform, crisis, war, policy change).
- Snap the user’s date to the **nearest observed time point** in the series (to handle annual, monthly or irregular data with gaps).
- Split the series into:
  - a **pre-intervention period** (before the critical moment),
  - a **post-intervention period** (after the critical moment).
- Use the `CausalImpact` package to:
  - learn the typical level, variance and trend of the series in the pre-intervention period,
  - construct a **counterfactual** trajectory for the post-intervention period (“what would have happened without the critical moment”),
  - estimate the point-wise and cumulative effect of the intervention.
- Produce plots:
  - observed vs. predicted (counterfactual) series,
  - point-wise causal effects,
  - cumulative effect over the post-intervention period.
- Print a numerical summary (average and relative effect, tail-area probability) and a **verbal template in English** to help students interpret the results.

**Theoretical background**

This notebook extends the basic time series analysis by introducing a formal treatment of a **“causal moment”** in a historical series.  
Instead of only describing long-term trends and seasonality, we:

- treat a specific date (or short time window) as a potential **turning point** in the process,
- use Bayesian structural time series (via `CausalImpact`) to estimate how the series would have continued if that turning point had not occurred,
- measure the **difference** between the counterfactual trajectory and the actual post-intervention path.

In methodological terms, this is an operationalisation of Werner’s idea of a **causal moment** in historical time-series research: the moment is not assumed to be decisive by definition; it is **tested** against the data.  
The student is invited to connect the detected break to concrete historical events, policies or processes, and to discuss alternative explanations (changes in measurement, data coverage, other contemporaneous shocks).


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


### Notebook 03b – Análisis de series temporales con un momento causal (CausalImpact)

**Operaciones analíticas**

- Cargar un archivo CSV y seleccionar:
  - una columna de fechas,
  - una columna numérica que representa la serie histórica de interés.
- Pedir al usuario una **fecha crítica / causal aproximada** (por ejemplo, la fecha de una reforma, una crisis, una guerra o un cambio de política).
- Ajustar la fecha introducida al **punto temporal observado más cercano** en la serie (para manejar datos anuales, mensuales o irregulares con huecos).
- Dividir la serie en:
  - un **periodo pre-intervención** (antes del momento crítico),
  - un **periodo post-intervención** (después del momento crítico).
- Utilizar el paquete `CausalImpact` para:
  - aprender el nivel, la variabilidad y la tendencia típicos de la serie en el periodo pre-intervención,
  - construir una trayectoria **contrafactual** para el periodo posterior (“qué habría pasado sin el momento crítico”),
  - estimar el efecto puntual y acumulado de la intervención.
- Producir gráficos:
  - serie observada vs. serie predicha (contrafactual),
  - efectos causales punto a punto,
  - efecto acumulado en el periodo post-intervención.
- Imprimir un resumen numérico (efecto medio y relativo, probabilidad en la cola posterior) y una **plantilla de interpretación en inglés** para ayudar a los estudiantes a leer los resultados.

**Fundamento teórico**

Este notebook amplía el análisis básico de series temporales introduciendo un tratamiento formal de un **“momento causal”** en una serie histórica.  
En lugar de limitarse a describir la tendencia y la estacionalidad, se:

- toma una fecha concreta (o una ventana corta) como posible **punto de inflexión** en el proceso,
- utiliza un modelo bayesiano de series temporales estructurales (a través de `CausalImpact`) para estimar cómo habría continuado la serie si dicho punto no hubiera ocurrido,
- mide la **diferencia** entre la trayectoria contrafactual y el comportamiento observado en el periodo posterior.

En términos metodológicos, esto opera la idea de Werner de un **momento causal** en el análisis de series históricas: el momento no se considera decisivo por definición, sino que se **pone a prueba** empíricamente.  
Se invita al estudiante a vincular la ruptura detectada con acontecimientos, políticas o procesos históricos concretos, y a discutir explicaciones alternativas (cambios en la medición, cobertura de los datos u otros choques simultáneos).

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


### Notebook 03b – Analiza szeregu czasowego z „momentem kauzalnym” (CausalImpact)

**Czynności analityczne**

- Wczytanie pliku CSV i wybór:
  - kolumny z datami,
  - kolumny ze zmienną ilościową, która tworzy analizowany szereg historyczny.
- Poproszenie użytkownika o **przybliżoną datę momentu krytycznego / kauzalnego** (np. reformy, kryzysu, wojny, zmiany polityki).
- „Dopasowanie” tej daty do **najbliższego realnie obserwowanego punktu czasowego** w szeregu (umożliwia pracę z danymi rocznymi, miesięcznymi czy nieregularnymi).
- Podział szeregu na:
  - **okres przedinterwencyjny** (przed momentem kauzalnym),
  - **okres pointerwencyjny** (po momencie kauzalnym).
- Zastosowanie pakietu `CausalImpact` w celu:
  - nauczenia się typowego poziomu, zmienności i trendu szeregu w okresie przedinterwencyjnym,
  - zbudowania **kontrafaktycznego przebiegu** szeregu w okresie pointerwencyjnym („jak wyglądałby szereg, gdyby moment kauzalny nie nastąpił”),
  - oszacowania efektów punktowych i efektu skumulowanego.
- Wygenerowanie wykresów:
  - szereg obserwowany vs. kontrfaktyczny,
  - efekt w poszczególnych punktach,
  - efekt skumulowany po interwencji.
- Wypisanie podsumowania liczbowego (efekt średni, efekt względny, miara istotności) oraz **szablonu interpretacji po angielsku**, który pomaga studentowi przełożyć wyniki modelu na opis historyczny.

**Umocowanie teoretyczne**

Notebook rozwija podstawową analizę szeregu czasowego o formalne ujęcie **„momentu kauzalnego”**.  
Zamiast tylko opisywać trend i sezonowość:

- traktujemy wskazaną datę (lub krótki odcinek czasu) jako kandydat na **punkt zwrotny**,
- przy użyciu bayesowskiego modelu strukturalnego szeregu czasowego (`CausalImpact`) konstruujemy **scenariusz kontrfaktyczny** – przebieg zjawiska, gdyby kontynuowało ono dotychczasową dynamikę,
- mierzymy **różnicę** między tym scenariuszem a rzeczywistym szeregiem po momencie kauzalnym, co pozwala ocenić rozmiar i trwałość przełomu.

W kategoriach metodologii historii jest to operacjonalizacja koncepcji **momentu kauzalnego** (Werner): moment nie jest z góry przyjmowany jako decydujący, lecz jest **testowany** na danych.  
Student zachęcany jest do powiązania wykrytej zmiany z konkretnymi wydarzeniami, decyzjami i procesami historycznymi oraz do rozważenia alternatywnych wyjaśnień (np. zmiany sposobu pomiaru, luki w danych, inne jednoczesne szoki).

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
