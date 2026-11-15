---
title: "Anagrafica da cassa a bilance – Configurazione di rete bilancia Unica"
date: "2026-11-15"
version: "1.0"
categoria: software KeepUp Smart
---

# Configurazione di rete bilancia Unica

Per configurare i parametri di connessione Ethernet della bilancia, fare riferimento al manuale utente del dispositivo.

## Modelli con tastiera a membrana o meccanica

Impostare tramite la **funzione 84** un indirizzo IP fisso e la porta di comunicazione desiderata.

!!! tip "Suggerimento"
    Impostare la porta **1001**, come suggerito nel manuale utente, oppure la porta **9002** per uniformità con i modelli Unica Touch.

## Modelli Unica Touch

- Impostare la porta LAN o Wi-Fi in modalità **IP fisso**.
- La porta di comunicazione non è modificabile ed è impostata in modo predefinito su **9002**.
- Verificare nelle impostazioni di Android che il time-out di spegnimento del display sia impostato su **"Never"**.

## Riepilogo porte di comunicazione

| Modello | Indirizzo IP | Porta TCP |
|---------|--------------|-----------|
| Unica con tastiera a membrana o meccanica | Fisso (funzione 84) | A scelta: 1001 (suggerita dal manuale utente) oppure 9002 |
| Unica Touch | Fisso (LAN o Wi-Fi) | 9002 (non modificabile) |

La porta e l'indirizzo IP impostati vanno riportati nell'[Anagrafica Bilance](anagrafica-configurazione-kus.md#anagrafica-bilance) di KeepUp Smart.

## Errore "Memoria Piena"

!!! warning "Attenzione"
    In caso di errore durante il trasferimento degli archivi, con comparsa del messaggio **"Memoria Piena"**, procedere alla cancellazione degli archivi Tare, Ingredienti e PLU tramite la **funzione 86** descritta nel manuale utente. Una volta completata la cancellazione, ritrasmettere tutta l'anagrafica articoli alla bilancia: vedi [Invio completo dell'intera anagrafica articoli](anagrafica-trasmissione.md#invio-completo-dellintera-anagrafica-articoli).
