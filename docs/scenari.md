---
title: "Scenari di applicazione"
date: "2026-11-15"
categoria: software KeepUp Smart
---

# Scenari di applicazione

## Scenario 1 – Negozio con una cassa e una bilancia

La cassa con KeepUp Smart e la bilancia Unica sono collegate alla stessa rete locale (LAN Ethernet).

![Scenario 1: una cassa e una bilancia in rete locale](assets/images/scenario-1-una-cassa-una-bilancia.png)

## Scenario 2 – Negozio con una cassa e più bilance "a passaggio"

La cassa comunica in rete locale con una bilancia; le bilance sono collegate tra loro tramite RS485 per lo scontrino "a passaggio".

![Scenario 2: una cassa e più bilance a passaggio collegate in RS485](assets/images/scenario-2-bilance-a-passaggio.png)

!!! note "Nota"
    Nella modalità "a passaggio" KeepUp Smart invia i dati alla sola bilancia master, che allinea le slave: vedi [Introduzione e sincronizzazione](anagrafica-introduzione.md).

## Scenario 3 – Negozio con una cassa e più bilance (più banchi o modelli diversi)

La cassa raggiunge in rete locale bilance di banchi o modelli differenti; alcune bilance possono essere a loro volta collegate tra loro in RS485.

![Scenario 3: una cassa e più bilance di banchi o modelli diversi](assets/images/scenario-3-piu-banchi.png)

## Scenario 4 – Più negozi con Inventa Backoffice

Inventa Backoffice gestisce da remoto più punti vendita, ciascuno con la propria cassa e le proprie bilance in rete locale.

![Scenario 4: più negozi collegati a Inventa Backoffice](assets/images/scenario-4-inventa-backoffice.png)

!!! tip "Approfondimento"
    I vantaggi dell'abbinamento sono descritti nella pagina [Integrazione con Inventa Backoffice](inventa-backoffice.md).
