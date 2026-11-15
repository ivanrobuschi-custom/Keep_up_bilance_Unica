---
title: "Suddivisione pesate multiple in cassa tramite QR Code – Introduzione"
date: "2026-11-15"
version: "1.0"
categoria: software KeepUp Smart
---

# Pesate multiple in cassa tramite QR Code

## Introduzione

Questa configurazione permette la suddivisione dello scontrino bilancia su un sistema di cassa con KeepUp Smart. Il sistema resta funzionante anche qualora i due strumenti non fossero connessi tra loro mediante rete locale, né collegati a un PC.

## Cosa serve

A KeepUp Smart bisogna collegare uno **scanner per codici a barre bidimensionali** (esempio Custom SM600) con collegamento **USB in emulazione di tastiera**.

## Note operative

!!! warning "Attenzione"
    - Con la bilancia **Unica**, se all'interno dello scontrino vengono effettuate molte vendite, verranno generati più QR Code da leggere in sequenza alla barriera cassa.
    - Con la bilancia **Icona**, il limite massimo di vendite per scontrino è di **35**: superandolo, il QR Code non verrà stampato.
    - Per la corretta generazione del QR Code non devono essere utilizzati articoli programmati come **NG**, né vendite con importo negativo. È necessario disabilitare a ogni operatore le funzionalità di **Resi** e **Sconti**.

!!! note "Nota"
    Sono possibili altre configurazioni funzionanti, oltre a quanto documentato in questo corso, per implementare specifici casi d'uso.

## Passi di configurazione

1. [Configurazione KeepUp Smart](qrcode-configurazione-kus.md) — barcode dinamici e codici degli articoli.
2. Configurazione della bilancia:
    - [bilancia Unica](qrcode-configurazione-unica.md);
    - [bilancia Icona](qrcode-configurazione-icona.md).
