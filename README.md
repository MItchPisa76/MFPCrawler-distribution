# MFPCrawler - Distribution & Installer Pipeline

Questo repository gestisce la generazione automatizzata degli installer `.exe` e la distribuzione client di **MFPCrawler**.

> **Nota di Architettura:** Il codice sorgente dell'applicazione risiede nel repository privato `MitchPisa76/MFPCrawler-Private`. Questo repository pubblico contiene esclusivamente gli script di packaging `jpackage`, le risorse grafiche ed il sistema di iniezione dinamica dei token client.

---

## 🛠️ Generazione Installer Personalizzato (Token Cliente)

Per generare un installer `.exe` contenente un token cliente configurato (Base64):

1. Clicca sul badge **Inietta Token & Genera Installer** sottostante.
2. Inserisci i dati richiesti nei campi del form:
   * **Target Version:** Il Tag della release presente nel repository privato (es. `v1.0.0`).
   * **Parametro A:** Identificativo univoco del Cliente (es. `CLIENT_AOUP`).
   * **Parametro B:** Codice Licenza / Installazione (es. `KEY_998822`).
3. Clicca su **Run workflow**. L'installer con il token iniettato direttamente nel JAR sarà generato e reso disponibile nei Download / Artifacts.

[![Inietta Token & Genera Installer](https://img.shields.io/badge/Inietta%20Token-Genera%20Installer-blue?style=for-the-badge&logo=githubactions)](../../actions/workflows/generate-custom-installer.yml)

---

## 📥 Storico Build e Download

La tabella sottostante viene aggiornata automaticamente dalla pipeline GitHub Actions ad ogni nuova generazione di installer personalizzato.

| Versione | Data / Ora | Cliente / Ref (Param A) | Installer Windows (.exe) |
| :--- | :--- | :--- | :--- |
<!-- DOWNLOAD_TABLE_MARKER -->

---

## 🏗️ Architettura della Pipeline
