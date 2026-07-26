# LollozzOS Configurator

**Suite di ottimizzazione, debloat e configurazione avanzata per Windows**, sviluppata e mantenuta da Lollozz. Distribuita come eseguibile (`.exe`), LollozzOS Configurator è il pannello di controllo centrale dell'ecosistema **LollozzOS**, pensato per utenti gaming e power user che vogliono spremere il massimo dal proprio sistema Windows.

---

## 🖥️ Interfaccia

- Menu CLI interamente in italiano, con banner ASCII art dedicato per ogni modulo e schema colori ANSI differenziato (blu, verde, rosso, giallo, viola) per riconoscere a colpo d'occhio la sezione in cui ci si trova
- Navigazione a menu numerati con validazione dell'input e gestione errori
- Layout console ottimizzato (`mode con: cols=130 lines=40`) per una resa pulita anche su terminali grandi
- Ogni modulo include una voce **"Cosa fa?"** con documentazione tecnica dettagliata della singola ottimizzazione
- Sistema di licenza integrato con verifica avviata già dalla schermata iniziale

---

## 🔐 Licenza

LollozzOS è protetto da un sistema di licenza proprietario legato all'hardware del PC su cui viene attivato.

**Per richiedere una licenza**: entra nel canale Discord e scrivimi direttamente.

---

## ⚙️ Menu Principale — Windows Optimizer Ultimate Edition

1. **Windows** – apre il Windows Manager (debloat, privacy, riparazione, attivazione)
2. **Office Tool** – installazione e attivazione di Office
3. **Ottimizza Rete** – Network Optimizer avanzato
4. **Overclock USB** – polling rate e calibrazione periferiche
5. **Timer Resolution** – riduzione input lag a livello Kernel
6. **Imposta Profilo Energetico** – Power Manager
7. **Informazioni di Sistema**
8. **Aggiorna e Ottimizza GPU** – tweaks dedicati NVIDIA/AMD
9. **Ottimizza Archiviazione/RAM** – Disk & RAM Manager
10. **Scegli il tuo Gioco** – Game Config Manager (Warzone, Fortnite)
11. **Gestisci BIOS** – BIOS Manager
12. **Crea Punto di Ripristino** – Restore Manager
13. **I Miei Social**
14. **Esci**

---

## 🌐 Network Optimizer

Modulo dedicato all'ottimizzazione approfondita dello stack di rete, con tanto di documentazione tecnica integrata nel programma:

- **Reset profondo** di interfacce, Winsock, IP, TCP, Teredo, 6to4, firewall e cache DNS
- **Priorità gaming**: tuning di `NetworkThrottlingIndex`, `SystemResponsiveness` e priorità dei processi multimediali/giochi nello scheduler di sistema
- **Rimozione limiti di banda**: eliminazione dei throttling su QoS, SMB e Task Offload, ottimizzazione dei parametri AFD (Ancillary Function Driver)
- **TCP NoDelay** (disattivazione dell'algoritmo di Nagle) applicato a tutte le interfacce per ridurre ping e jitter
- **Tuning TCP globale avanzato** via `netsh`: autotuning, ECN, RSS, congestion provider CTCP, Fast Open, disattivazione euristiche e RSC
- **Ottimizzazione driver di rete**: rilevamento automatico della scheda attiva e disattivazione dei parametri di risparmio energetico/latenza (Gigabit auto-disable, DMA Coalescing, ecc.), con backup automatico del driver prima di ogni modifica
- **DNS Manager**: rilevamento della scheda di rete attiva, impostazione rapida di Cloudflare/Google DNS o ripristino DHCP, con test di latenza integrato
- **Strumenti diagnostici**: collegamenti rapidi a Speed Test, Bufferbloat Test e test di perdita pacchetti
- Avvio automatico di tool esterni dedicati (TestMb, TCP Optimizer) al termine dell'ottimizzazione

---

## 🎮 Overclock USB

- **Overclock del Polling Rate** delle periferiche USB (fino a 1000Hz+), per ridurre il ritardo di campionamento e il click-to-photon latency
- **Calibrazione analogici pad** tramite integrazione con tool online dedicati
- Creazione automatica di shortcut nel menu contestuale del desktop per accesso rapido a overclock e calibrazione
- Gestione tramite tool esterno dedicato con elevazione automatica dei permessi

---

## ⏱️ Timer Resolution

- Impostazione del **Timer di sistema a 0,5ms** (contro lo standard Windows di 15,6ms) per ridurre drasticamente l'input lag
- Verifica della risoluzione del timer attualmente attiva
- Backup automatico dei tool utilizzati e creazione di un collegamento in avvio automatico
- Script di ripristino generato automaticamente per tornare ai valori di default

---

## 🔋 Power Manager

- Importazione di un **profilo energetico personalizzato** ottimizzato per le prestazioni
- Ripristino totale dei piani energetici e delle impostazioni di alimentazione predefinite di Windows
- Verifica del **Core Parking della CPU** (per assicurarsi che tutti i core siano attivi e disponibili)

---

## 🎨 GPU Tweaks (NVIDIA / AMD)

- Percorsi dedicati e separati per schede **NVIDIA (GeForce)** e **AMD (Radeon Adrenalin)**
- Tweaks di registro "Deep" per ottimizzare driver e prestazioni GPU
- Estrazione sul desktop di utility dedicate per il produttore rilevato

---

## 💾 Disk & RAM Manager

- Avvio di **Windows Memory Cleaner** per liberare la RAM occupata
- Avvio di **ISLC** (Intelligent Standby List Cleaner), copiato e mantenuto in una cartella dedicata su `C:\LollozzOs`
- **Ottimizzazione latenza NVMe** tramite abilitazione dei parametri Native NVMe nel registro
- Documentazione integrata sull'ottimizzazione dell'I/O, TRIM e riduzione del micro-stuttering da caricamento texture

---

## 🧬 BIOS Manager

- **Procedura guidata di aggiornamento BIOS**: rilevamento automatico di produttore e modello scheda madre, versione e data del BIOS installato, con ricerca diretta dell'ultimo aggiornamento disponibile
- **Riavvio diretto nel BIOS/UEFI** da un'unica voce di menu
- **Sblocco impostazioni nascoste del BIOS** tramite Export/Import della NVRAM (integrazione SCEWIN)
- Shortcut dedicato "Riavvia nel BIOS" installabile nel menu contestuale del desktop

---

## 🔄 Restore Manager

- Creazione di un **punto di ripristino** prima di ogni sessione di ottimizzazione
- Elenco completo dei punti di ripristino disponibili, con log dedicato
- Avvio diretto di un punto di ripristino dal menu
- Sezione informativa su utilizzo e best practice dei punti di ripristino

---

## 📎 Office Manager

- Installazione guidata di **Microsoft Office**
- Attivazione di Office integrata nel medesimo modulo

---

## 🕹️ Ottimizzazione Giochi (Warzone / Fortnite)

Modulo "Scegli il tuo gioco" per applicare configurazioni pronte all'uso direttamente nei file di gioco:

- **Importazione di config ottimizzate** già pronte, salvate automaticamente nel percorso corretto dei file utente del gioco
- **Backup e ripristino** della configurazione attuale prima di ogni modifica, per garantire piena reversibilità
- Supporto dedicato a **Warzone**, incluso il download e la configurazione automatica della **Mod Audio**, pensata per migliorare la percezione di passi e suoni direzionali in game
- Documentazione tecnica integrata per ogni gioco supportato

---

## 🎥 Modulo OBS Studio (Installer & Configurator)

Modulo autonomo integrato nel menu principale che gestisce l'intero ciclo di vita di OBS Studio:

- Installazione automatica via Winget/Chocolatey con gestione errori
- **Configurazione guidata**: rilevamento GPU, scelta risoluzione (inclusi valori personalizzati/frazionari), FPS, tipo di connessione, generazione automatica di profilo, scena JSON (Monitor/Mic/Webcam) e bitrate CBR calcolato dinamicamente
- **Debloat OBS**: rimozione file di localizzazione non italiani/inglesi, pulizia pacchetti lingua CEF, rimozione temi inutili, pulizia cache/log/crash
- Reset configurazione e disinstallazione completa

---

## 🌐 Modulo Chrome Debloat by Lollozz

- Interfaccia ristilizzata con codifica colori ANSI coerente con il resto della suite
- Rimozione cronologia, cache, estensioni non necessarie
- Gestione aggiornamenti (disattivazione/riattivazione)
- Ottimizzazioni rete (Fast Internet, Data Saver, Low Power Mode)
- Gestione lingue e pulizia file superflui

---

## ⚙️ Windows Manager (sotto-menu debloat e privacy)

1. **Attiva Windows**
2. **Impostazioni Extra LollozzOS**
3. **Critus Tech** – strumenti di debloat/ottimizzazione dedicati
4. **Debloat Extra**
5. **Altre Ottimizzazioni**
6. **Ultimate Windows Tweaker**
7. **Rimuovi Windows AI** (Copilot e componenti IA integrate)
8. **Ripara Windows**
9. **Disattiva Privacy Windows** (basato su O&O ShutUp10)
10. **Gestione ricerca/barra applicazioni**
11. **Win11Debloat** integrato
12. **Download Browser**
13. **Installazione Playbook** (pacchetto extra di strumenti e configurazioni)
14. **Aggiornamento Chipset CPU** (rilevamento automatico AMD/Intel)
15. **Debloat Chrome**
16. **Debloat Discord**
17. **Gestione OBS Studio**
18. **Autoruns** (Sysinternals)
19. Info/changelog integrato ("Cosa fa?")

### Aree di intervento nel dettaglio

- **Telemetria e privacy**: disattivazione completa DiagTrack, CEIP, WER, PerfTrack, sincronizzazione impostazioni account Microsoft, Timeline/Activity Feed, raccolta dati vocali, KMS telemetry
- **Servizi e driver**: disabilitazione servizi non essenziali (OneSyncSvc, TrkWks, PcaSvc, UCPD, ecc.) e driver in background (GpuEnergyDrv, NetBT)
- **Registro di sistema**: centinaia di tweak HKLM/HKCU applicati sia all'utente corrente sia al profilo Default (per i nuovi account futuri), con branding personalizzato LollozzOS in `winver` e boot entry
- **Rimozione bloatware**: disinstallazione app AppX preinstallate, blocco reinstallazione automatica, rimozione OneDrive, Xbox, Cortana/Search estesa, LockApp, SmartScreen, sync programs
- **Gaming & performance**: Game Mode, priorità CPU al 90% per l'app attiva, disattivazione Page Combining, rimozione limiti SMB per LAN, gestione risoluzione/refresh rate
- **Sicurezza/Defender**: menu dedicato alla disattivazione controllata di Windows Defender con backup automatico dei servizi pre-modifica
- **Manutenzione**: script di ripristino generati automaticamente prima di ogni modifica critica, per garantire reversibilità

---

## 🧩 Architettura tecnica

- Eseguibile Windows (`.exe`) con interfaccia a console e navigazione a menu modulari
- Logica PowerShell integrata per operazioni avanzate su registro, WMI e gestione GPU
- Generazione dinamica di script di ripristino (rollback) prima di ogni modifica invasiva
- Gestione multi-utente: applicazione delle modifiche sia all'utente corrente sia al profilo Default di Windows

---

## ⚠️ Nota

LollozzOS Configurator apporta modifiche profonde a registro, servizi e componenti di sistema. Si raccomanda di creare un punto di ripristino prima dell'uso e di eseguire l'applicazione con privilegi di amministratore.

---

## 🙏 Crediti

LollozzOS Configurator è stato realizzato anche grazie all'integrazione di alcuni progetti open source disponibili su GitHub, tra cui:

- Chris Titus Tech's Windows Utility
- RemoveWindowsAI Zoocware
- Script di attivazione Microsoft (MAS)
- Win11Debloat Raphire
- OneClick Quaked

## 🌍 Sito Web

[Inserisci qui il link al sito ufficiale]

## 🔗 Community

- Discord: https://discord.gg/gd5cT3Jw9M
- TikTok: @lollozz_os
- Instagram: https://www.instagram.com/lollozz_labs?igsh=dnRuYzB0dXQwNDZh&utm_source=qr