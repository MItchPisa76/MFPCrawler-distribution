# MFPCrawler

**MFPCrawler** è una soluzione per la scansione e il monitoraggio di stampanti multifunzione (MFP) all'interno di reti locali tramite protocollo SNMP.

---

## 🛠️ Centro Generazione Installer Personalizzato

Per generare un installer `.exe` personalizzato (con il token cliente integrato nel JAR):

1. Clicca sul badge **Inietta Token & Genera Installer**.
2. Compila i campi richiesti:
   * **Target Version:** La versione del JAR da scaricare (es. `v1.0.0`).
   * **Parametro A:** Identificativo del Cliente (es. `CLIENT_AOUP`).
   * **Parametro B:** Codice Licenza / Installazione (es. `KEY_998822`).
3. Clicca su **Run workflow**. 

[![Inietta Token & Genera Installer](https://img.shields.io/badge/Inietta%20Token-Genera%20Installer-blue?style=for-the-badge&logo=githubactions)](https://github.com/MitchPisa76/MFPCrawler/actions/workflows/generate-custom-installer.yml)

---

## 📥 Storico Build e Download

La tabella sottostante viene aggiornata automaticamente dalla pipeline ad ogni generazione dell'installer.

| Versione | Data / Ora | Cliente / Ref (Param A) | Installer Windows (.exe) |
| :--- | :--- | :--- | :--- |
<!-- DOWNLOAD_TABLE_MARKER -->

---

## 🔒 Sicurezza e Gestione Token

Il token viene generato combinando i parametri cliente in formato **Base64** e iniettato direttamente nel file `token.properties` all'interno dell'archivio `MFPCrawler-fat.jar`.

All'avvio dell'applicazione, il client Java legge la configurazione direttamente dal classpath.

---

*Sviluppato per la gestione ed il monitoraggio centralizzato della flotta di stampa.*
