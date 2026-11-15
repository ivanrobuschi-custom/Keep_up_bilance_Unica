---
title: "Pesate in cassa con QR Code – Configurazione bilancia Unica"
date: "2026-11-15"
version: "1.0"
categoria: software KeepUp Smart
---

# Configurazione bilancia Unica

## Tasti utilizzati

| Tasto | Funzione |
|-------|----------|
| ![Tasto più](assets/images/unica-tasto-piu.png) | Spostarsi tra le opzioni del menu |
| ![Tasto ENTER](assets/images/unica-tasto-enter.png) | ENTER: attivare o confermare |
| ![Tasto C](assets/images/unica-tasto-c.png) | C: uscire dalla programmazione |

## Configurazione QrCode

### Attivazione del formato FREEFORM

1. Dalla "Pagina Iniziale" richiamare la funzione **"QrCode"**: ![Tasti chiave, 2, 8](assets/images/unica-tasti-fn28.png)
2. Sul display viene visualizzato:

    ![Display funzione 28](assets/images/unica-display-fn28.png)

3. Spostarsi sull'opzione **FREEFORM** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e attivarla premendo il tasto ENTER ![Tasto ENTER](assets/images/unica-tasto-enter.png)
4. Spostarsi quindi sull'opzione **SET FREEFORM** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e confermare premendo il tasto ENTER ![Tasto ENTER](assets/images/unica-tasto-enter.png)
5. Sul display apparirà:

    ![Display funzione 28: prefisso, transazione, suffisso](assets/images/unica-display-fn28-freeform.png)

### Impostazione di prefisso, transazione e suffisso

1. Spostarsi sull'opzione **PREFISSO** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e confermare premendo il tasto ENTER.
2. Verificare che il parametro sia **vuoto**; qualora non lo fosse, cancellarne tutto il contenuto. Confermare premendo il tasto ENTER.
3. Spostarsi sull'opzione **TRANSAZIONE** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e confermare premendo il tasto ENTER.
4. Impostare il seguente testo nel parametro (rispettando le lettere minuscole):

    ```
    r07n05o05s03
    ```

5. Confermare premendo il tasto ENTER.
6. Spostarsi sull'opzione **SUFFISSO** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e confermare premendo il tasto ENTER.
7. Verificare che il parametro sia **vuoto**; qualora non lo fosse, cancellarne tutto il contenuto. Confermare premendo il tasto ENTER.
8. Al termine premere per due volte il tasto C per uscire dalla programmazione: ![Tasto C per due volte](assets/images/unica-tasto-c-x2.png)

### Attivazione della stampa del QR Code

1. Dalla "Pagina Iniziale" richiamare la funzione **"Personalizza Stampe"**: ![Tasti chiave, 4, 7](assets/images/unica-tasti-fn47.png)
2. Sul display viene visualizzato:

    ![Display funzione 47](assets/images/unica-display-fn47.png)

3. Spostarsi sull'opzione **ST. QR-CODE** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e attivarla premendo il tasto ENTER.
4. Al termine premere per due volte il tasto C per uscire dalla programmazione.

## Configurazione PLU

!!! note "Quando serve"
    Fare riferimento a questa programmazione solo nel caso in cui non ci sia un gestionale collegato alla bilancia per la generazione dell'anagrafica PLU. Se l'anagrafica viene inviata da KeepUp Smart, vedi [Anagrafica da cassa a bilance](anagrafica-introduzione.md).

1. Dalla "Pagina Iniziale" richiamare la funzione **"PLU"**: ![Tasti chiave, 2, 2](assets/images/unica-tasti-fn22.png)
2. Sul display viene visualizzato:

    ![Display funzione 22](assets/images/unica-display-fn22.png)

3. Selezionare **"PLU PROGRAMMAZ."** premendo il tasto ENTER. Sul display viene visualizzato:

    ![Display funzione 22: menu di programmazione PLU](assets/images/unica-display-fn22-menu.png)

4. Utilizzare i tasti ![Tasti più oppure meno](assets/images/unica-tasti-piu-meno.png) per navigare all'interno del menu.
5. Selezionare **"PLU COMPLETO"** e confermare premendo il tasto ENTER. Sul display viene visualizzato:

    ![Display funzione 22: numero PLU](assets/images/unica-display-fn22-plu-numero.png)

6. Digitare il codice del PLU (esempio "1") e confermare premendo ENTER. Sul display viene visualizzato:

    ![Display funzione 22: dati del PLU](assets/images/unica-display-fn22-plu-dati.png)

7. Verranno richiesti in sequenza tutti i dati dell'articolo: digitarli uno alla volta confermando con il tasto ENTER. In particolare:

    | Dato | Valore |
    |------|--------|
    | **Tipo PLU** | **KG** per un PLU "pesato"; **PZ** per un PLU "a corpo" |
    | **Barcode** | Selezionare il formato **LPPPPPPIIIIIK** |

8. Al termine della programmazione del PLU il display tornerà alla richiesta del numero PLU: è quindi possibile procedere inserendo un nuovo numero di PLU seguito da ENTER, oppure premere il tasto C per uscire.

!!! warning "Tipo PLU NG"
    Non selezionare la tipologia **NG** (PLU "negativo"): non è compatibile con la generazione del QR Code.

!!! tip "Modifiche rapide"
    - In un impianto già installato, il 99% della programmazione quotidiana si riduce alla semplice modifica del prezzo degli articoli già presenti in memoria: tramite la voce di menu **"PLU SOLO PREZZO"** è possibile modificare rapidamente solo tale dato, lasciando inalterati i restanti.
    - Per modificare un singolo dato (descrizione, tipo, ecc.) di un PLU esistente è possibile utilizzare la voce di menu **"PLU SELEZIONE"**, che permette di scegliere direttamente quale dato modificare.

## Configurazione Barcode generale

!!! note "Quando serve"
    Questo passaggio si rende necessario nel momento in cui l'anagrafica degli articoli viene trasmessa alla bilancia tramite un gestionale esterno.

1. Dalla "Pagina Iniziale" richiamare la funzione **"Barcode"**: ![Tasti chiave, 4, 0](assets/images/unica-tasti-fn40.png)
2. Sul display viene visualizzato:

    ![Display funzione 40](assets/images/unica-display-fn40.png)

3. Premere il tasto ENTER.
4. Spostarsi sull'opzione **LBBBBBBIIIIIK** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e attivarla premendo il tasto ENTER.
5. Premere per due volte il tasto C per uscire dalla programmazione.

## Operazioni aggiuntive

Per evitare vendite a prezzo libero, sconti manuali sugli articoli e operazioni in detrazione che potrebbero compromettere la lettura del QR Code in cassa, è necessario bloccare la possibilità di eseguire tali operazioni.

### Vendita solo tramite PLU

1. Dalla "Pagina Iniziale" richiamare la funzione: ![Tasti chiave, 4, 2](assets/images/unica-tasti-fn42.png)
2. Spostarsi sull'opzione **"SOLO PLU"** con il tasto ![Tasto più](assets/images/unica-tasto-piu.png) e attivarla premendo il tasto ENTER.
3. Premere C per uscire dalla programmazione.

### Disattivazione di sconti e resi per operatore

1. Spostarsi nella funzione: ![Tasti chiave, 2, 1](assets/images/unica-tasti-fn21.png)
2. Sul display viene visualizzato:

    ![Display funzione 21](assets/images/unica-display-fn21.png)

3. Accedere alla programmazione premendo il tasto ENTER.
4. Inserire il codice dell'operatore (es. Op. 1) e confermare.
5. Disattivare con ENTER le opzioni **"SCONTO"** e **"RESO"**.
6. Premere C per uscire dalla programmazione.

!!! warning "Attenzione"
    Ripetere questa programmazione per tutti gli operatori che verranno utilizzati in fase operativa.
