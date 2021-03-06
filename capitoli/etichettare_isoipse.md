# Vestizione curve di livello

Come **tematizzare** e **etichettare** in modo particolare le curve di livello

<!-- TOC -->

- [Vestizione curve di livello](#vestizione-curve-di-livello)
  - [tematizzazione](#tematizzazione)
    - [stile layer](#stile-layer)
      - [Categorizzato](#categorizzato)
      - [tramite regole](#tramite-regole)
  - [etichettature](#etichettature)
    - [regole](#regole)
  - [etichettatura particolare](#etichettatura-particolare)

<!-- /TOC -->

## tematizzazione

Per una vestizione accattivante, le isoipse possono essere tematizzate in modo diverso a seconda del valore di quota, ecco un esempio:

![](../imgs/esempi/img_03.png)

### stile layer

#### Categorizzato

usando la seguente espressione:

```
"ELEV" % 500 = 0
```
dove `ELEV` è l'attributo che contiene i valori di elevazione/quota; l'espressione è vera (1) solo quando la divisione ELEV/500 non ha resto. 

![](../imgs/esempi/img_0311.png)


#### tramite regole

nel caso volessimo più valori diversificati, usare le Regole:

![](../imgs/esempi/img_0312.png)

ottenendo

![](../imgs/esempi/img_0313.png)

## etichettature

### regole

Per far seguire l'etichettatura alla tematizzazione particolare fatta prima:

![](../imgs/esempi/img_032.png)

oppure:

![](../imgs/esempi/img_0322.png)

## etichettatura particolare

Etichettare lungo una line

https://user-images.githubusercontent.com/7631137/156880668-d2d3835f-4a8e-46ea-a911-1a474420b201.mp4

espressione utilizzata:

```
intersection( 
$geometry, buffer(geometry(get_feature_by_id('linea', 1)),20))
```

blog post riferimento: <https://pigrecoinfinito.com/2020/01/31/qgis-come-allineare-le-etichette-delle-isoipse/>
