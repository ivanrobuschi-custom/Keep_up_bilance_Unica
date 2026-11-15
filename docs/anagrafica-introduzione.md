---
title: "Gestione anagrafica articoli / PLU da cassa verso bilance – Introduzione"
date: "2026-11-15"
version: "1.0"
categoria: software KeepUp Smart
---

# Anagrafica articoli / PLU da cassa verso bilance

## Introduzione

Questa configurazione permette di gestire l'anagrafica articoli al punto cassa con KeepUp Smart e trasmetterla a una o più bilance.

- I dispositivi devono essere tutti raggiungibili tramite rete locale e si consiglia di impostarli tutti con **indirizzo IP statico**.
- Le bilance possono essere, alla bisogna, raggruppate in **"banchi"**, in modo da suddividere i PLU perché siano inviati miratamente.
- Ogni singola bilancia può essere configurata per appartenere a uno o più banchi.

!!! tip "Sistemi semplici"
    In caso di sistemi semplici si consiglia l'utilizzo del solo banco "0", in modo che i tasti diretti in tastiera della bilancia siano già associati per default ai PLU aventi il medesimo numero del tasto.

### Bilance "a passaggio" (Master/Slave)

In caso di più bilance configurate per "scontrino a passaggio" (collegate tra loro tramite RS485), le comunicazioni dalla cassa avverranno unicamente con la bilancia **"Master"**, che si occuperà di allineare le sue bilance **"Slave"** (queste ultime potrebbero anche non essere collegate alla rete locale e non avere un proprio indirizzo IP).

!!! note "Nota"
    La configurazione della modalità "scontrino a passaggio" non è trattata in questo corso: si rimanda al manuale della bilancia.

## Differenze tra Unica EL e Unica R

Il sistema è compatibile sia con bilance Unica EL sia con Unica R, con alcune differenze operative.

| Caratteristica | Unica EL | Unica R |
|----------------|----------|---------|
| Caratteri grassetto nel testo ingredienti (tramite sequenze `^b+` e `^b-`) | NO | SI |
| Tabella testi ingredienti | 50 elementi | 500 elementi |
| Flag "tracciabilità" | NO | SI |
| Lunghezza massima del testo ingredienti per ciascun PLU | 144 caratteri | 162 caratteri (attivazione/disattivazione di grassetto conta come 1 carattere) |

## Logiche di sincronizzazione dati

!!! warning "Importante"
    - **Aggiornamenti/inserimenti**: il sistema invia nuovi articoli e modifiche anagrafiche (prezzo, descrizione, tipo vendita, tara, …) basandosi sull'univocità della coppia **Codice Banco + PLU**.
    - **Cancellazioni**: le eliminazioni effettuate su KeepUp Smart non sono sincronizzate. Un articolo rimosso dal gestionale di cassa rimarrà residente nella memoria della bilancia.
    - **Variazioni di Codice Banco o PLU**: se vengono modificati il Codice Banco o il PLU di un prodotto esistente, il sistema lo tratterà come un nuovo inserimento. In bilancia coesisteranno quindi sia il nuovo articolo sia quello precedente (non più aggiornato).

### Cancellare articoli in bilancia

Per cancellare un articolo in bilancia occorre agire sul dispositivo attraverso la **funzione 22** (selezionando PLU CANCELLA; fare riferimento al manuale utente del dispositivo per ulteriori dettagli).

In alternativa è possibile la cancellazione completa dell'archivio PLU attraverso la **funzione 86** (selezionando archivio PLU; fare riferimento al manuale utente del dispositivo per ulteriori dettagli). Al termine della cancellazione occorre procedere con l'[invio completo dell'intera anagrafica articoli](anagrafica-trasmissione.md#invio-completo-dellintera-anagrafica-articoli).

## Passi successivi

1. [Configurazione KeepUp Smart](anagrafica-configurazione-kus.md)
2. [Configurazione di rete della bilancia Unica](anagrafica-configurazione-unica.md)
3. [Trasmissione dati alle bilance](anagrafica-trasmissione.md)
