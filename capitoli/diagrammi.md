# Diagrammi

## Introduzione

**QGIS** permette di visualizzare dei diagrammi sovrapposti alle geometrie:

![](../imgs/esempi/diagrammi1.png)

le tipologie presenti sono:

![](../imgs/esempi/diagrammi2.png)

## Esempio proposto

Tracciare diagramma a torta che rappresenti la percentuale, sul totale, dell'area comunale ricadente nel bacino:

### espressioni utilizzate

1. campo `perc1` : `$area/"Shape_Area"`
2. campo `perc2` : `1 - $area/"Shape_Area"`

![](../imgs/esempi/diagrammi3.png)

### risultato

![](../imgs/esempi/diagrammi4.png)

## Osservazioni

Purtroppo i Diagrammi in QGIS sono stati da sempre poco sviluppati per mancanza di sponsor.
