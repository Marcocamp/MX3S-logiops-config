[English](README.md) | [Italiano](README.it.md)
# 🖱️​​ Configurazione per Logiops del MX Master 3s

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/Marcocamp/MX3S-logiops-config?style=social)](https://github.com/Marcocamp/MX3S-logiops-config/stargazers)

**Descrizione:** Questa repository offre una configurazione di [logiops](https://github.com/PixlOne/logiops) che implementa l'utilizzo delle gesture del Logitech MX Master 3S.


## Funzionalità
Profilo testato per Ubuntu 22.04
- **Rotella laterale:** Controllo del volume
- **Tasto Gesutre:** Mostra la scrivania
- **Tasto Gesutre + su:** Apri il terminale predefinito
- **Tasto Gesutre + sx:** Passa alla scrivania di sinistra
- **Tasto Gesutre + dx:** Passa alla scrivania di destra

## Istruzioni per l'Installazione 
Segui questi passaggi semplici per avviare la configurazione:

1. **Installa logiops:** segui le istruzioni dalla [repository ufficiale](https://github.com/PixlOne/logiops) per installare il pacchetto
2. **Clonare il Repository:** Apri il terminale ed esegui:
    ```bash
    git clone https://github.com/Marcocamp/MX3S-logiops-config.git
    ```
3. **Applicazione del File di Configurazione:** Questo passaggio richiede permessi di root (`sudo`).

    **Backup:** Esegui questo comando per salvare la configurazione attuale:
    ```bash
    sudo cp /etc/logid.cfg /etc/logid.cfg.bkp 
    ```
    **Copiare il Nuovo File:** Copia il file `logid.cfg` presente nella directory clonata al percorso di sistema:
    ```bash
    sudo cp logid.cfg /etc/logid.cfg 
    ```
    **Riavviare e Verificare il Servizio:** Ricarica i servizi per applicare le modifiche in tempo reale:
    ```bash
    sudo systemctl restart logid 
    sudo systemctl status logid
    ```
4. **Testa la configurazione:** Prova ad utilizzare il tasto gesture o a modificare il volume


## Contributo e Supporto
Hai trovato un bug o hai miglioramenti da suggerire?  Sentiti libero/a di:
1.  Creare una `Branch` per le tue modifiche.
2.  Aggiungere un *Pull Request* (PR) direttamente su questo repository.

**Contatti:**
Se hai bisogno di assistenza o vuoi vedere altri miei progetti, visita il mio profilo GitHub: 
 [Marcocamp](https://github.com/Marcocamp) 

Grazie per aver visitato la mia repository! Spero che questa configurazione ti sia utile.
