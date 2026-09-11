# MFPCrawler - Distribution & Installer Pipeline

Questo repository gestisce la generazione automatizzata degli installer `.exe` e la distribuzione client di **MFPCrawler**.

> **Nota di Architettura:** Il codice sorgente dell'applicazione risiede nel repository privato `MitchPisa76/MFPCrawler-Private`. Questo repository pubblico contiene esclusivamente gli script di packaging e la pipeline di distribuzione.

---

## 🚀 Generazione Rapida per Versione

Seleziona la versione desiderata e clicca il bottone per generare un installer personalizzato con il tuo token cliente:

> **Per ogni versione**, configura nel form:
> * **Dato A (Parametro A):** Identificativo univoco del Cliente (es. `CLIENT_AOUP`)
> * **Dato B (Parametro B):** Codice Licenza / Installazione (es. `KEY_998822`)

### Versioni Disponibili

| Versione | Stato | Azione |
| :--- | :--- | :--- |
| V3.4.5 | ✅ Disponibile | [![Genera V3.4.5](https://img.shields.io/badge/Genera%20V3%2E4%2E5-blue?style=flat-square&logo=githubactions)](https://github.com/MItchPisa76/MFPCrawler-distribution/actions/workflows/generate-custom-installer.yml) |
| NEWT2 | ✅ Disponibile | [![Genera NEWT2](https://img.shields.io/badge/Genera%20NEWT2-blue?style=flat-square&logo=githubactions)](https://github.com/MItchPisa76/MFPCrawler-distribution/actions/workflows/generate-custom-installer.yml) |
| NTY | ✅ Disponibile | [![Genera NTY](https://img.shields.io/badge/Genera%20NTY-blue?style=flat-square&logo=githubactions)](https://github.com/MItchPisa76/MFPCrawler-distribution/actions/workflows/generate-custom-installer.yml) |
| NEWT | ✅ Disponibile | [![Genera NEWT](https://img.shields.io/badge/Genera%20NEWT-blue?style=flat-square&logo=githubactions)](https://github.com/MItchPisa76/MFPCrawler-distribution/actions/workflows/generate-custom-installer.yml) |
| V-new | ✅ Disponibile | [![Genera V-new](https://img.shields.io/badge/Genera%20V-new-blue?style=flat-square&logo=githubactions)](https://github.com/MItchPisa76/MFPCrawler-distribution/actions/workflows/generate-custom-installer.yml) |
| v1.0.0-manual | ✅ Disponibile | [![Genera v1.0.0-manual](https://img.shields.io/badge/Genera%20v1%2E0%2E0-manual-blue?style=flat-square&logo=githubactions)](https://github.com/MItchPisa76/MFPCrawler-distribution/actions/workflows/generate-custom-installer.yml) |

---

## 🛠️ Generazione Installer Personalizzato (Token Cliente)

Per generare un installer `.exe` contenente un token cliente configurato (Base64):

1. Seleziona la **versione desiderata** dalla tabella sopra e clicca il bottone corrispondente.
2. Inserisci i dati richiesti nei campi del form:
   * **Target Version:** Verrà precompilato con la versione selezionata (es. `v1.5.2`).
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
| **V3.4.5** | 2026-09-11 09:21 | `APPENA_CREATO_1` | [⚡ Scarica MFPCrawler-1.3.5.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/V3.4.5/APPENA_CREATO_1/MFPCrawler-1.3.5.exe) |
| **V3.4.5** | 2026-09-11 09:18 | `Tizio` | [⚡ Scarica MFPCrawler-1.3.5.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/V3.4.5/Tizio/MFPCrawler-1.3.5.exe) |
| **NEWT2** | 2026-09-09 17:58 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.3.5.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT2/CLIENT_001/MFPCrawler-1.3.5.exe) |
| **NEWT2** | 2026-09-07 14:45 | `CLIENT_00D` | [⚡ Scarica MFPCrawler-1.3.5.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT2/CLIENT_00D/MFPCrawler-1.3.5.exe) |
| **NTY** | 2026-09-07 14:08 | `CLIENT_00D` | [⚡ Scarica MFPCrawler-1.3.4.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NTY/CLIENT_00D/MFPCrawler-1.3.4.exe) |
| **NTY** | 2026-09-07 13:32 | `CLIENT_00D` | [⚡ Scarica MFPCrawler-1.3.4.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NTY/CLIENT_00D/MFPCrawler-1.3.4.exe) |
| **NTY** | 2026-09-07 12:11 | `CLIENT_00D` | [⚡ Scarica MFPCrawler-1.3.4.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NTY/CLIENT_00D/MFPCrawler-1.3.4.exe) |
| **NTY** | 2026-09-06 18:50 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.3.4.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NTY/CLIENT_001/MFPCrawler-1.3.4.exe) |
| **NEWT** | 2026-09-06 18:39 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.0.0.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT/CLIENT_001/MFPCrawler-1.0.0.exe) |
| **NEWT** | 2026-09-06 18:18 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.0.0.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT/CLIENT_001/MFPCrawler-1.0.0.exe) |
| **NEWT** | 2026-09-06 18:09 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.0.0.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT/CLIENT_001/MFPCrawler-1.0.0.exe) |
| **NEWT** | 2026-09-06 17:58 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.0.0.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT/CLIENT_001/MFPCrawler-1.0.0.exe) |
| **NEWT** | 2026-09-06 17:48 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.0.0.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT/CLIENT_001/MFPCrawler-1.0.0.exe) |
| **NEWT** | 2026-09-06 17:24 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.0.0.exe](https://github.com/MItchPisa76/MFPCrawler-distribution/releases/download/NEWT/MFPCrawler-1.0.0.exe) |
| **NEWT** | 2026-09-06 17:11 | `CLIENT_001` | [⚡ Scarica MFPCrawler-1.0.0.exe](https://github.com/MitchPisa76/MFPCrawler/releases/download/NEWT/MFPCrawler-1.0.0.exe) |

---

## 🏗️ Architettura della Pipeline

