# Privacy Policy - Baby Touch Lock

*Last updated: November 17, 2026*

**Baby Touch Lock** (`com.babytouchlock`) is an open-source Android application designed to prevent accidental screen touches, gesture navigation, and hardware button presses while displaying media or playing games.

---

## English

### 1. No Data Collection or Storage
Baby Touch Lock does **not** collect, track, or share any personal information, sensitive data, device identifiers, or analytics.

If you choose to enable the optional **PIN Protection** feature, a salted cryptographic hash (SHA-256) of your chosen PIN is stored strictly locally on your device in private app storage solely to authenticate unlock attempts. The plain-text PIN is never stored, and no credential or data can ever leave your device.

### 2. No Internet Access
The application does not request or use the `android.permission.INTERNET` permission. All processing is executed **100% locally** on your device. No data can leave your device.

### 3. Use of the Android AccessibilityService API
Baby Touch Lock uses Android's AccessibilityService API exclusively for the following purpose:
- **Touch and Key Interception**: To display a transparent, modal overlay that prevents unintended touches on the screen, blocks navigation bar gestures (e.g. Back, Home, App Switch), and optionally suppresses physical volume key presses while the lock is engaged.

**Accessibility API Compliance Disclosures:**
- **No Screen Content Reading**: The service config explicitly sets `canRetrieveWindowContent="false"` and `accessibilityEventTypes=""`. The app **cannot** and does **not** read text, inspect UI elements, or record on-screen content.
- **No Keystroke Logging**: The app does not log, record, or transmit passwords, messages, or keystrokes from any application. When PIN protection is enabled, PIN digits entered on the local keypad are processed strictly in memory to authenticate unlocking.
- **Explicit User Control**: The service is activated only after the user grants explicit permission in Android Settings and is engaged on-demand (via the Quick Settings tile or the dashboard test button). It can be unlocked at any time by sliding the floating unlock handle (and entering your PIN if PIN protection is enabled).

### 4. Children's Privacy (COPPA & GDPR-K Compliance)
Baby Touch Lock is a tool intended for parents and guardians. Because the app collects no personal information whatsoever and contains no ads or external trackers, it complies with the Children's Online Privacy Protection Act (COPPA) and the General Data Protection Regulation (GDPR).

### 5. Open Source
Baby Touch Lock is free and open-source software licensed under the **GNU General Public License v3.0 (GPL-3.0)**. The full source code is publicly inspectable.

---

## Italiano (Informativa sulla Privacy)

### 1. Nessuna Raccolta o Memorizzazione di Dati
Baby Touch Lock **non** raccoglie, non traccia e non condivide alcuna informazione personale, dato sensibile, identificativo del dispositivo o dato statistico.

Se si sceglie di attivare la funzione opzionale di **Protezione con PIN**, un hash crittografico con salt (SHA-256) del codice PIN viene memorizzato esclusivamente in locale nella memoria privata dell'app sul dispositivo, al solo fine di autenticare i tentativi di sblocco. Il PIN in chiaro non viene mai salvato e nessun dato o credenziale lascia mai il dispositivo.

### 2. Nessun Accesso a Internet
L'applicazione non richiede il permesso `android.permission.INTERNET`. Tutte le operazioni avvengono **al 100% in locale** sul tuo dispositivo. Nessun dato lascia mai il dispositivo.

### 3. Utilizzo dell'API Android AccessibilityService
Baby Touch Lock impiega l'API di Accessibilità di Android esclusivamente per la seguente finalità:
- **Intercettazione di Tocchi e Tasti**: Per mostrare un overlay modale che impedisce tocchi accidentali sullo schermo, blocca i gesti di navigazione (Indietro, Home, App Recenti) e opzionalmente inibisce i tasti fisici del volume durante la visione di contenuti da parte dei bambini.

**Garanzie di Conformità dell'API di Accessibilità:**
- **Nessuna Lettura dei Contenuti a Schermo**: Il servizio configura espressamente `canRetrieveWindowContent="false"` ed `accessibilityEventTypes=""`. L'app **non può** e **non** legge testi, password, campi di input o elementi a video.
- **Nessun Keylogger**: L'app non registra né salva sequenze di tasti o testi digitati in alcuna applicazione. Se la protezione con PIN è attiva, le cifre inserite sul tastierino a schermo vengono elaborate unicamente in memoria per la convalida dello sblocco.
- **Controllo Totale dell'Utente**: Il servizio viene abilitato unicamente previa concessione esplicita dell'utente nelle Impostazioni di Sistema e viene attivato su richiesta (dal pannello Quick Settings o dall'app). È possibile sbloccare lo schermo in qualsiasi momento tramite lo slider dedicato (e inserendo il codice PIN qualora sia stato impostato).

### 4. Tutela dei Minori
Baby Touch Lock è un'utilità per genitori e tutori. Poiché non raccoglie alcun dato e non include pubblicità o librerie terze di profilazione, è pienamente conforme alle normative a tutela dei minori (COPPA e GDPR-K).

### 5. Open Source
Baby Touch Lock è software libero e open source distribuito con licenza **GNU General Public License v3.0 (GPL-3.0)**. Il codice sorgente è liberamente verificabile e trasparente.
