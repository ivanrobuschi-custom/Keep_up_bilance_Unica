---
title: "Pesate in cassa con QR Code – Configurazione bilancia Icona"
date: "2026-11-15"
version: "1.0"
categoria: software KeepUp Smart
---

# Configurazione bilancia Icona

!!! note "Limite di vendite per scontrino"
    Con la bilancia Icona il limite massimo di vendite per scontrino è di 35: superandolo, il QR Code non verrà stampato.

## Configurazione QrCode

1. Dalla "Pagina Iniziale" premere:

    ![Impostazioni, Formati Barcode, Composizione QRCode Data Collect](assets/images/icona-menu-composizione-qrcode.png)

2. Per creare una nuova sequenza di QR Code Data Collect, premere il tasto ![Tasto nuovo](assets/images/icona-tasto-nuovo.png)
3. Inserire il numero ID tramite il tastierino numerico (es. 3) e confermare con OK.

    ![Tastierino ID Formato](assets/images/icona-tastierino-id-formato.png)

4. Inserire una descrizione per identificare la programmazione:

    ![Campo Descrizione](assets/images/icona-campo-descrizione.png)

5. Spostarsi nella sezione:

    ![Sezione Parametri](assets/images/icona-sezione-parametri.png)

6. Selezionare il campo **Body** e inserire la stringa `r07n05o05s03`:

    ![Campo Body con la stringa r07n05o05s03](assets/images/icona-campo-body.png)

7. Uscire premendo due volte il tasto ![Tasto indietro per due volte](assets/images/icona-tasto-indietro-x2.png)

## Impostazione Barcode

1. Dalla "Pagina Iniziale" premere:

    ![Impostazioni, Configurazione, Configurazione Operativa, Opzioni Multipesata](assets/images/icona-menu-opzioni-multipesata.png)

2. Selezionare la voce **"Barcode => QR Code Datacollect"** e impostare il numero precedentemente programmato:

    ![Barcode QR Code Datacollect impostato a 3](assets/images/icona-barcode-qrcode-datacollect.png)

3. Impostare il parametro **"Barcode => Vendita"** in base a come viene generata l'anagrafica PLU:

    | Caso | Valore |
    |------|--------|
    | Nessun gestionale collegato alla bilancia: i PLU vengono programmati manualmente | **106** |
    | Articoli generati da un software esterno | **100** |

    ![Barcode Vendita impostato a 106](assets/images/icona-barcode-vendita-106.png)

    ![Barcode Vendita impostato a 100](assets/images/icona-barcode-vendita-100.png)

4. Uscire tramite il tasto ![Tasto indietro](assets/images/icona-tasto-indietro.png)

## Formato di stampa

1. Spostarsi in:

    ![Archivi Dati, Formati Etichetta](assets/images/icona-menu-formati-etichetta.png)

2. Premere il tasto dei formati fissi presenti nella memoria della macchina: ![Tasto formati fissi](assets/images/icona-tasto-formati-fissi.png)
3. Scorrere l'elenco fino alla posizione **86 "CODA SCONTRINO QrCode"**, selezionarlo e premere il tasto ![Tasto conferma](assets/images/icona-tasto-conferma.png)
4. Inserire il codice **51**, sovrascrivendo quello presente in memoria.

    ![Tastierino Formato Fisso 86 con nuovo formato 51](assets/images/icona-tastierino-formato-51.png)

5. Uscire tramite il tasto ![Tasto indietro](assets/images/icona-tasto-indietro.png)

## Operazioni aggiuntive

Per evitare vendite a prezzo libero, sconti manuali sugli articoli e operazioni in detrazione che potrebbero compromettere la lettura del QR Code in cassa, è necessario bloccare la possibilità di eseguire tali operazioni.

### Vendita solo tramite richiamo articolo

1. Dalla "Pagina Iniziale" premere:

    ![Impostazioni, Configurazione, Configurazione Operativa, Richiamo Articoli](assets/images/icona-menu-richiamo-articoli.png)

2. Impostare la modalità di richiamo in:

    ![Manuale - Modo Richiamo PLU: N. Cifre](assets/images/icona-modo-richiamo-plu.png)

3. Uscire tramite il tasto ![Tasto indietro](assets/images/icona-tasto-indietro.png)

L'opzione vincolerà lo strumento a vendere solo tramite il richiamo di un articolo. È possibile anche impostare un eventuale numero di cifre dopo il quale lo strumento richiama in automatico l'articolo senza premere il tasto PLU.

### Disattivazione di sconti, resi e vendite in sottrazione per operatore

1. Spostarsi nella sezione:

    ![Archivi Dati, Operatori](assets/images/icona-menu-operatori.png)

2. Selezionare dall'elenco il primo operatore in lista e accedere alla programmazione.
3. Spostarsi nella sezione:

    ![Sezione Operazioni su Vendita](assets/images/icona-sezione-operazioni-vendita.png)

4. Disattivare i parametri **Utilizzo Sconti**, **Utilizzo Resi** e **Vendite in Sottrazione**:

    ![Utilizzo Sconti, Utilizzo Resi e Vendite in Sottrazione disattivati](assets/images/icona-parametri-operatore.png)

5. Uscire tramite il tasto ![Tasto indietro](assets/images/icona-tasto-indietro.png)

!!! note "Nota"
    Lo strumento di default non ha operatori programmati: se l'elenco dovesse risultare "vuoto", creare gli operatori che saranno utilizzati con queste opzioni disattivate.
