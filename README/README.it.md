# redstar upscaler
Potente strumento di upscaling video che utilizza FFmpeg, Real-ESRGAN, Flowframes - ora supporta **l'interfaccia utente multilingue**!

🌐 Lingua:
[한국어](https://github.com/redstar-programmer/upscaler/blob/main/README.md) | [English](https://github.com/redstar-programmer/upscaler/blob/main/README/README.en.md) | [日本語](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ja.md) | [中文](https://github.com/redstar-programmer/upscaler/blob/main/README/README.zh.md) |
[Français](https://github.com/redstar-programmer/upscaler/blob/main/README/README.fr.md) | [Deutsch](https://github.com/redstar-programmer/upscaler/blob/main/README/README.de.md) | [Español](https://github.com/redstar-programmer/upscaler/blob/main/README/README.es.md) | [Português](https://github.com/redstar-programmer/upscaler/blob/main/README/README.pt.md) |
[Русский](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ru.md) | [Italiano](https://github.com/redstar-programmer/upscaler/blob/main/README/README.it.md) | [Tiếng Việt](https://github.com/redstar-programmer/upscaler/blob/main/README/README.vi.md) | [Bahasa Indonesia](https://github.com/redstar-programmer/upscaler/blob/main/README/README.id.md) |
[ภาษาไทย](https://github.com/redstar-programmer/upscaler/blob/main/README/README.th.md) | [العربية](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>Strumento di upscaling video basato su fmpeg, realesrgan, flowframes</strong><br>
  <em>Moderna interfaccia grafica, impostazioni preimpostate, supporto per l'elaborazione di più file</em>.
</p>

---.

Download: [Release](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ Supporta l'upscaler "redstar".

Vi piace questo progetto o volete sostenerne lo sviluppo?
Fai una piccola donazione per aiutarci a migliorare le funzionalità e ad avere aggiornamenti affidabili!

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub Sponsors** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 La vostra sponsorizzazione dei costi del server, del tempo di sviluppo e di una tazza di caffè è molto importante. Grazie!

## Indice dei contenuti

- [👋 Introduzione](#Introduzione)
- [💾 Installazione e preparazione](#Installazione-e-Preparazione)
- [🔧 Caratteristiche principali](#Caratteristiche principali)
- [🚀 Come usare (Avvio rapido)](#Come usare l'avvio rapido)
- [⚙️ Descrizione dettagliata delle funzioni](#detailed-feature-description)
- [🙏 Ringraziamenti](#Riconoscimenti)
- Storia](#storia)

## 👋 Introduzione
**redstar upscaler è uno strumento GUI basato su Python per scalare automaticamente i video a risoluzioni più elevate utilizzando `ffmpeg`, `Real-ESRGAN` e `Flowframes`.

- Estrazione di fotogrammi video → upscaling → unione di video in un unico passaggio
- Supporta vari modelli realesrgan
- Interpolazione opzionale tramite Flowframes
- Estrazione ed elaborazione automatica dei codec audio
- Lavora sulla posizione della sorgente o su un percorso specificato

> ⚠️ Sviluppato e testato in ambiente Windows.

Di seguito è riportata una semplice dimostrazione d'uso; fare clic su di essa per essere indirizzati a YouTube:<br>
[![Guarda la demo](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co "Guarda su YouTube")

## 💾 Installazione e preparazione

1. installare e localizzare i seguenti strumenti esterni (notare che il file di distribuzione include i file di installazione di ffmpeg, Real-ESRGAN e Flowframes (vedere la cartella Programmi nel percorso))
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - [Flowframes](https://github.com/n00mkrad/flowframes) *(opzionale)*.
2. decomprimere ed eseguire upscaler.exe di readstar.
3. nel caso di Flowframes, i modelli caricati possono essere diversi a seconda dell'ambiente utente, quindi assicurarsi di eseguire Flowframes e verificare che l'AI di interpolazione e il Modello AI nella scheda Interpolazione corrispondano alla versione di resources/flowframes_models.ini di redstar upscaler. <br>Segnalare i modelli non caricati contrassegnandoli con # e assicurarsi che l'ordine dei modelli nella finestra delle impostazioni di redstar upscaler corrisponda all'ordine dei modelli in <br>Flowframes prima di procedere.

## 🔧 Caratteristiche principali.

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
- ✅ Selezione video multipla e funzionamento sequenziale
- ✅ Aggiunta di video con trascinamento
- ✅ Disponibilità del programma principale e selezione diretta
- Modalità di risparmio del disco
- ✅ Supporto multilingue (15 lingue)
<br><br>
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
- Salvataggio delle preimpostazioni e loro applicazione automatica
- Rilevamento automatico del codec audio e impostazione del bitrate
- Rilevamento e selezione automatica dei modelli di realesrgan
- ✅ Impostazioni dettagliate per FFMPEG, real-ESRGAN e Flowframes
- ✅ Modifica delle impostazioni delle opzioni in base alla versione di Flowframes<br>(la versione può essere cambiata specificando il percorso della versione in flowframes nella pagina principale)
<br><br>
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
- ✅ Controllare il comando di esecuzione dell'upscale (può essere copiato ed eseguito separatamente su CMD)
<br><br>
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
- Monitorare l'avanzamento generale dell'operazione di upscale
- Controllare la registrazione dell'upscale (i file di log vengono creati in base alla data nella cartella log della cartella live).
- Pulire automaticamente i deliverable dopo il completamento del lavoro (con prefisso [REDSTAR])
- ✅ Impostare l'azione dopo il completamento dell'attività<br>( Non fare nulla / Esci dal programma / Sleep / Modalità ibernazione / Chiudi finestra)
<br><br>
## 🚀 Come si usa (Avvio rapido)

1. aggiungere file video (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV supportati)
2. specificare la posizione di lavoro o spuntare la casella "Usa percorso file originale".
3. fare clic sul pulsante "Impostazioni" del video aggiunto
4. impostazioni dettagliate di ffmpeg, realESRGAN, Flowframes
5. fare clic su Batch applica a tutti i file / Applica solo ai file selezionati
6. fare clic sul pulsante "Conferma
7. selezionare i comandi da eseguire e fare clic sul pulsante "Avvia attività".

> Il risultato dell'operazione sarà costituito da due file: il video upscalato e il video interpolato nella cartella selezionata.
> I file completati saranno salvati con il prefisso [REDSTAR].
---]

## ⚙️ Descrizione dettagliata della funzione

| Voce | Descrizione |
|------|------|
| **Impostazione del percorso di lavoro** | Fornire un percorso predefinito o l'opzione "Usa il percorso del file originale".
| **Formato video supportato** | La maggior parte dei formati supportati, tra cui MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV, ecc.
| **Modelli in scala** | Rileva automaticamente realesr-animevideov3, realesr-general, 4xplus, ecc.
| **Elaborazione audio** | Supporto per la codifica di vari formati come `aac`, `mp3`, `flac`, ecc.
| **Integrazione dei fotogrammi di flusso** | È possibile impostare l'interpolazione (FPS ×2, ×4, ×8).
| **Modalità di risparmio del disco** | Eliminazione automatica delle immagini intermedie

## 🙏 Ringraziamenti

- realesrgan di [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes di [n00mkrad](https://github.com/n00mkrad/flowframes)
- Se volete contribuire a questo progetto o suggerire una funzionalità, lasciate un commento su [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).

# 📜 Storia

v 1.1.0
 > 1. configurazione del menu (aprire file, chiudere file, impostazioni del registro, impostazioni della lingua)
 > 2. Aggiunte impostazioni multilingue (lingue disponibili: Coreano, Inglese, 日本語, 中文, Français, Deutsch, Español, Português, Русский, Tiếng Việt, Bahasa Indonesia, ไทย, Italiano, العربية)
 > 3. Modifiche ai messaggi e ad alcuni codici per adattarli alle impostazioni linguistiche aggiunte.
 > 4. alcune modifiche alla configurazione dell'interfaccia utente
 > 5. visualizzazione delle informazioni sulla versione di ffmpeg, real-ESRGAN e Flowframes (schermata principale)
 > 6. Supporto della versione 1.41.0 di Flowframes (attualmente sono disponibili solo le versioni 1.40.0 e 1.36.0 a causa di un problema del comando cmd nella versione 1.41.0)
 > 7. Corretto un problema per cui gli elementi di AI Models venivano visualizzati in lettere minuscole
 > 8. Aggiunte opzioni FFMPEG (Pixel, codec video) - le opzioni sono visualizzate in base al PC dell'utente
 > 9. Migliorato il controllo di CUDA per ogni PC dell'utente - verifica la disponibilità e il tipo di GPU (schermata principale)

v 1.0.0
 > 1. Riscrittura completa del codice
 > 2. Modifiche all'interfaccia utente
 > 3. Aumento della gamma di video/audio che possono essere elaborati
 > 4. aggiunta la modalità di risparmio del disco
 > 5. Distribuzione dei principali programmi

v 0.1.92
 > 1. Corretto un problema che causava il fallimento dell'interpolazione a causa della duplicazione dell'input nella casella combinata del modello AI quando si cambiava il percorso dei Flowframes.
 > 2. Aggiunto un codice di controllo per lo stato di selezione della casella combinata durante l'interpolazione.

v 0.1.91
 > 1. Aggiunte alcune funzioni di aggiornamento della casella combinata relative a Flowframes.
 > 2. Aggiustati alcuni file di distribuzione

v 0.1.9
 > 1. Applicate modifiche al modello Flowframes
 > 2. Nuovo modello Flowframes 1.36.0, implementazione modello 1.40.0
 > 3. Non si verifica più il fallimento della riga di comando di Flowframes
 > 4. I file possono ora essere aggiunti trascinandoli e rilasciandoli
 > 5. Fissate le impostazioni di Flowframes che non vengono applicate

v 0.1.8
 > 1. Corretto l'errore di controllo della nuova versione quando si controlla la versione
 > 2. Se flowframes è installato nel percorso predefinito (es. C:\Users\Administrator\AppData\Local\Flowframes\), impostare il percorso come predefinito prima di iniziare.
 > 3. Quando si aggiungono più selezioni di file, l'applicazione si blocca a causa di un errore.
 > 4. Corretto un errore all'avvio dell'attività dopo l'aggiunta di più file.

v 0.1.7
 > 1. È possibile modificare le dimensioni del programma
 > 2. Corretto un errore quando si lavora con file senza voce
 > 3. modificata l'intera configurazione dell'interfaccia utente (riconfigurata per adattarsi alla modifica delle dimensioni)

v 0.1.6
 > 1. Corretto il problema delle diverse dimensioni dei caratteri a seconda della risoluzione dello schermo
 > 2. Corretto un problema per cui il titolo del programma non mostrava le informazioni sulla versione come nuova versione
 > 3. Corretto un problema per cui il file config.ini veniva salvato in un percorso differente
 > 4. Quando si modifica il moltiplicatore di upscaling realesrgan, viene modificata anche la casella combinata del modello di upscaling.
 > 5. Aggiunta la funzione di controllo degli aggiornamenti
 > 6. Sistemata una certa logica
 > 7. Modificato il colore delle tabelle di risoluzione e fps
 > 8. Permettere all'utente di modificare la risoluzione (deve essere inserita come 1024x768)

v 0.1.5
 > 1. Corretto il problema per cui il modello AI non viene cambiato automaticamente quando si seleziona l'interpolazione FLOWFRAMES AI
 > 2. Corretto un problema per cui l'interpolazione dei flowframes non veniva interpolata in base all'opzione selezionata
 > 3. Aggiunta casella combinata "Metodo di calcolo FPS" per evitare un calcolo FPS errato per alcuni video.
        -> r_frame_rate / avg_frame_rate, l'impostazione predefinita è r_frame_rate
 > 4. visualizzare l'avanzamento del recupero delle informazioni video quando si seleziona un file video.
 > 5. cambiare l'impostazione predefinita per l'apertura dell'ultima cartella selezionata quando si seleziona nuovamente un file dopo la sua apertura

v 0.1.4
 > 1. modificato il modo in cui viene letto il file config.ini
 > 2. cambiato il modo di ottenere le informazioni video da Python AV a ffmpeg
 > 3. aggiunta la chiusura della finestra al termine dell'attività
 > 4. Mostra il nome completo del file come tooltip al passaggio del mouse nell'elenco attività
 > 5. Mostra risoluzione (prima) / risoluzione (dopo) / FPS (prima) / FPS (dopo) per ogni file nell'elenco delle attività.
 > 6. Rimuovere la casella di immissione FPS (a causa dell'etichettatura di cui sopra per ciascun file).
 > 7. rimuovere la dimensione della stima degli FPS in uscita (rimossa a causa dell'etichettatura specifica per ogni file)
 > 8. visualizzare l'avanzamento come due barre di avanzamento per tutti i file/compiti

v 0.1.3
 > 1. Corretto l'errore di calcolo degli FPS dei file, a causa del quale alcune informazioni sugli FPS erano errate durante il caricamento dei file.

v 0.1.2
 > 1. Modifiche alla configurazione dell'interfaccia utente
 > 2. modifiche alla logica interna
 > 3. risolto il problema per cui il modello realesrgan non veniva eseguito quando si selezionavano due dei seguenti modelli
 > 4. modificato il modo di utilizzare i modelli realesrgan
 > -> Copiare il nuovo file del modello (*.param) nella cartella models della cartella di installazione di realesrgan per poterlo utilizzare.
 > 5. Visualizzazione delle informazioni sulla larghezza, l'altezza e la dimensione stimata dell'upscale dell'ultimo file dell'immagine di destinazione con cui lavorare.
 > 6. Scrivere il codice per migrare il file config.ini
 > 7. cambiare l'immagine di decomposizione FFMPEG AAC -> FLAC
 > 8. altre correzioni di bug

v 0.1.1
 > 1. Primo programma di upscaling video con ffmepg, realesrgan e flowframe.