# Statistik 2 - Projekt: Umsatzprognose im Detailhandel

## Projektbeschreibung
**Fragestellung:** Welche Prädiktoren haben Einfluss bzw. sind signifikant für den Umsatz im Detailhandel?

Dieses Projekt analysiert mittels multipler Regression die Einflussfaktoren auf den Umsatz von Produkten in verschiedenen Filialen des Detailhandels.

## Hypothesen
- Die Grösse der Filiale hat keinen Einfluss auf den Umsatz
- Je älter der Laden, desto höher der Umsatz, d.h. Alter hat keinen Einfluss auf Umsatz
- Fett in Produkten haben keinen Einfluss auf den Umsatz

## Ziel
- Multiples Regressionsmodell erstellen
- Vorhersage des Umsatzes eines Produkts in einem bestimmten Geschäft
- Empfehlungen geben, welche Eigenschaften von Produkten und Geschäften eine wichtige Rolle für die Umsatzsteigerung spielen

## Datensätze

### Prädiktoren (Unabhängige Variablen)

**Produkt:**
| Variable | Beschreibung |
|----------|-------------|
| Item_Identifier | Eindeutige Produkt-ID |
| Item_Weight | Gewicht des Produkts |
| Item_Fat_Content | Fettgehalt-Kategorie (z.B. Low Fat) |
| Item_Visibility | Anteil der Regal-/Displayfläche im Store |
| Item_Type | Produktkategorie |
| Item_MRP | Maximaler Verkaufspreis (List Price/MRP) |

**Filiale/Geschäft:**
| Variable | Beschreibung |
|----------|-------------|
| Outlet_Identifier | Eindeutige Filial-ID |
| Outlet_Establishment_Year | Gründungsjahr der Filiale |
| Outlet_Size | Filialgrösse (Fläche) |
| Outlet_Location_Type | Standorttyp/Stadtklasse (Tier 1-3) |
| Outlet_Type | Filialtyp (z.B. Grocery Store, Supermarket) |

### Zielvariable (Abhängige Variable)
- **Item_Outlet_Sales:** Umsatz des Produkts in der jeweiligen Filiale

### Datengrundlage
- `Train.csv` - Enthält UV und die AV (für Training)
- `Test.csv` - Enthält nur die UV/Prädiktoren (für Vorhersage)

## Installation

### Voraussetzungen
- Python 3.8 oder höher
- Jupyter Notebook / JupyterLab oder VS Code mit Jupyter Extension

### Abhängigkeiten installieren

```bash
pip install numpy pandas seaborn matplotlib statsmodels scikit-learn
```

Oder mit requirements.txt:
```bash
pip install -r requirements.txt
```

## Ausführung

1. Repository klonen oder herunterladen
2. Abhängigkeiten installieren (siehe oben)
3. Jupyter Notebook starten oder in VS Code öffnen
4. `PK_Stat2_Projekt_LN2.ipynb` öffnen
5. Alle Zellen der Reihe nach ausführen

**Wichtig:** Die Datendateien (Train.csv, Test.csv) müssen sich im selben Verzeichnis wie das Notebook befinden.

## Projektstruktur

```
02Stats_Projekt_PK/
 README.md                    # Diese Dokumentation
 PK_Stat2_Projekt_LN2.ipynb   # Hauptnotebook mit Analyse
 Train.csv                    # Trainingsdaten
 Test.csv                     # Testdaten
 requirements.txt             # Python-Abhängigkeiten
```

## Verwendete Bibliotheken

- **numpy** - Numerische Berechnungen
- **pandas** - Datenmanipulation und -analyse
- **seaborn** - Statistische Datenvisualisierung
- **matplotlib** - Diagramme und Plots
- **statsmodels** - Statistische Modelle und Tests
- **scikit-learn** - Machine Learning Tools (MinMaxScaler)

## Autor
Statistik 2 Projekt - Pleurat Kelmendi HSLU
