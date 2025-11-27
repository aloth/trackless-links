# Trackless Links FAQ

**Häufig gestellte Fragen und Benutzerhandbuch**

Willkommen! Diese Anleitung hilft dir, Trackless Links optimal zu nutzen und beantwortet häufige Fragen.

---

## Hintergrund: Warum saubere URLs wichtig sind

Als Tim Berners-Lee 1989 das World Wide Web erfand, waren URLs als einfache Adressen gedacht: ein Weg, ein Dokument auf einem Server zu finden. Eine URL wie `shop.de/schuhe` zeigte dir genau, wohin du gehst.

Heute sind URLs zu Überwachungswerkzeugen geworden.

### Die verborgene Ökonomie deiner Klicks

Jedes Mal, wenn du einen Link in einer E-Mail anklickst, einen Beitrag in sozialen Medien antippst oder einem Suchergebnis folgst, wird zusätzlicher Code an die URL angehängt. Diese Tracking-Parameter verwandeln eine einfache Adresse in einen detaillierten Bericht über dich:

```
shop.de/schuhe?utm_source=newsletter&utm_campaign=fruehjahrsverkauf&utm_medium=email&fbclid=IwAR3x...&mc_eid=abc123
```

Diese einzelne URL verrät mehreren Unternehmen:
- Du kamst von einem E-Mail-Newsletter (nicht direkt von der Website)
- Du hast auf die Kampagne "Frühjahrsverkauf" reagiert
- Facebook weiß, dass du genau diesen Link angeklickt hast
- Die E-Mail-Marketing-Plattform hat deine eindeutige Abonnenten-ID protokolliert

Nichts davon beeinflusst, welche Seite du siehst. Es beeinflusst nur, was Unternehmen über dich erfahren.

### Wie Tracking-Parameter funktionieren

Das Fragezeichen (?) in einer URL trennt die Seitenadresse von ihren Parametern. Alles nach dem Fragezeichen sind Metadaten, und Unternehmen haben dies zu einem Überwachungssystem standardisiert:

| Parameter | Wer nutzt ihn | Was er verrät |
|-----------|---------------|---------------|
| `utm_source` | Marketer überall | Welche Website oder Plattform dich geschickt hat |
| `utm_campaign` | Marketer überall | Auf welche Anzeige oder E-Mail du geklickt hast |
| `fbclid` | Facebook/Meta | Deine Facebook-Nutzer-ID und dein Klickverhalten |
| `gclid` | Google | Dein Google-Werbeprofil |
| `mc_eid` | Mailchimp | Deine E-Mail-Abonnenten-Identität |
| `ttclid` | TikTok | Dein TikTok-Werbeprofil |
| `msclkid` | Microsoft/Bing | Dein Microsoft-Werbeprofil |

Wenn du einen Link mit Freunden teilst, teilst du oft auch diese Parameter mit. Das ermöglicht es Unternehmen, nicht nur dich zu tracken, sondern auch jeden, der den weitergeleiteten Link anklickt.

### Die Kosten für deine Privatsphäre

Dieses Tracking geschieht unsichtbar, aber die Folgen sind real:

**Websiteübergreifende Profilerstellung**: Unternehmen wie Facebook und Google sehen deine Aktivitäten auf Millionen von Websites und erstellen detaillierte Profile deiner Interessen, Käufe und Gewohnheiten.

**Preisdiskriminierung**: Einige Händler nutzen Tracking-Daten, um verschiedenen Nutzern unterschiedliche Preise anzuzeigen, basierend auf ihrer vermuteten Zahlungsbereitschaft.

**Filterblasen**: Werbeplattformen nutzen deine Klickhistorie, um zu entscheiden, welche Inhalte du siehst. Das kann deine Exposition gegenüber vielfältigen Standpunkten einschränken.

**Datenlecks**: Jedes Unternehmen, das deine Tracking-Daten speichert, ist ein potenzielles Ziel für Datenlecks. Je weniger Daten gesammelt werden, desto weniger können gestohlen werden.

### Was Trackless Links macht

Trackless Links fängt URLs ab, bevor sie geladen werden, und entfernt Tracking-Parameter. Die bereinigte URL führt dich zur selben Seite, aber ohne deinen digitalen Fingerabdruck zu übertragen.

Vorher: `amazon.de/dp/1119737281?tag=influencer-20&ref=pd_sl_abc&utm_source=instagram`

Nachher: `amazon.de/dp/1119737281`

Das passiert automatisch für jeden Link in Safari und stellt URLs wieder so her, wie sie gedacht waren: einfache Adressen, mehr nicht.

---

## Erste Schritte

### Wie aktiviere ich die Safari-Erweiterung?

Nach der Installation der App:

1. Öffne **Safari** auf deinem Gerät
2. Tippe auf das **AA**-Symbol (oder den **Erweiterungen**-Button auf dem Mac) in der Adressleiste
3. Tippe auf **Erweiterungen verwalten**
4. Finde **Trackless Links** und schalte es **ein**
5. Erteile die erforderlichen Berechtigungen

Die Erweiterung ist jetzt aktiv und beginnt automatisch, URLs zu bereinigen.

### Warum funktioniert die Erweiterung nicht?

Stelle sicher, dass du:
- Die Erweiterung in den Safari-Einstellungen aktiviert hast (siehe oben)
- Die erforderlichen Berechtigungen erteilt hast, als du dazu aufgefordert wurdest
- Die Erweiterung benötigt die Berechtigung, auf Webseiteninhalte zuzugreifen

Auf dem Mac musst du möglicherweise auch unter **Systemeinstellungen > Datenschutz & Sicherheit > Erweiterungen** Trackless Links aktivieren.

### Muss ich etwas konfigurieren, um zu starten?

Nein. Trackless Links funktioniert sofort mit sinnvollen Standardeinstellungen:
- Tracking-Parameter werden automatisch entfernt
- Über 20 vordefinierte Weiterleitungen sind einsatzbereit (du kannst die aktivieren, die du möchtest)
- Alle Tweaks sind optional, aktiviere also nur, was du brauchst

---

## Datenschutz und Tracking-Filter

### Welche Tracking-Parameter werden entfernt?

Trackless Links entfernt gängige Tracking-Codes wie:
- `utm_source`, `utm_medium`, `utm_campaign` (Marketing-Attribution)
- `fbclid` (Facebook-Klick-Identifier)
- `gclid` (Google-Klick-Identifier)
- `msclkid` (Microsoft/Bing-Klick-Identifier)
- Und dutzende weitere

Du kannst die vollständige Liste im **Filter**-Tab einsehen und eigene Parameter hinzufügen.

### Wie füge ich einen eigenen Tracking-Parameter hinzu?

1. Öffne die Trackless Links App
2. Gehe zum **Filter**-Tab
3. Tippe auf die **+**-Schaltfläche
4. Gib den Parameternamen ein (z.B. `mein_tracker`)
5. Tippe auf **Sichern**

Beim nächsten Besuch einer URL mit diesem Parameter wird er automatisch entfernt.

### Kann ich die Tracking-Entfernung vorübergehend deaktivieren?

Ja. Im **Filter**-Tab kannst du einzelne Filter ein- oder ausschalten. Du kannst auch die gesamte Tracking-Entfernung deaktivieren, indem du alle Filter ausschaltest.

---

## Weiterleitungen

### Was sind Weiterleitungen und warum sollte ich sie nutzen?

Viele beliebte Websites sammeln umfangreiche Daten über ihre Nutzer. Weiterleitungen ermöglichen es dir, dich automatisch zu datenschutzfreundlichen Alternativen umzuleiten, die dieselben Inhalte ohne Überwachung bieten.

**Datenschutzfreundliche Frontends**: Projekte wie Nitter (für Twitter/X), Invidious (für YouTube) und Libreddit (für Reddit) zeigen Inhalte großer Plattformen an, ohne dich einzuloggen oder dein Verhalten zu verfolgen. Du bekommst die Inhalte, sie bekommen nicht deine Daten.

**Interface-Präferenzen**: Reddits old.reddit.com bietet die klassische Oberfläche, die viele Nutzer bevorzugen. Einige Nachrichtenseiten haben übersichtlichere mobile Versionen. Mit Weiterleitungen landest du immer auf deiner bevorzugten Version.

**Regionale Umleitung**: Internationale Domains automatisch zu deiner lokalen Version umleiten oder umgekehrt.

### Wie aktiviere ich eine vordefinierte Weiterleitung?

1. Öffne die App und gehe zu **Weiterleitungen**
2. Durchsuche die Liste der vordefinierten Regeln
3. Schalte den Schalter neben einer Regel ein, um sie zu aktivieren
4. Die Weiterleitung ist sofort aktiv, kein Neustart erforderlich

### Wie erstelle ich eine eigene Weiterleitung?

1. Gehe zum **Weiterleitungen**-Tab
2. Tippe auf die **+**-Schaltfläche
3. Gib ein:
   - **Muster**: Die URL, VON der du weiterleiten möchtest (z.B. `reddit.com`)
   - **Ersetzung**: Wohin du weiterleiten möchtest (z.B. `old.reddit.com`)
   - **Titel** (optional): Ein freundlicher Name für diese Regel
4. Tippe auf **Sichern**

Du kannst exakte Übereinstimmungen oder reguläre Ausdrücke (Regex) für erweiterte Muster verwenden.

### Kann ich die Reihenfolge meiner Weiterleitungsregeln ändern?

Ja. Die Reihenfolge ist wichtig, da die erste passende Regel gewinnt. So änderst du die Reihenfolge:

1. Gehe zu **Weiterleitungen**
2. Halte eine Regel gedrückt und ziehe sie, um sie neu anzuordnen
3. Deine Priorität wird automatisch gespeichert

### Meine Weiterleitung funktioniert nicht. Was ist falsch?

Überprüfe diese häufigen Probleme:

- Ist die Regel **aktiviert**? (Schalter ist an)
- Ist das Muster korrekt? (teste zuerst mit einer einfachen exakten Übereinstimmung)
- Passt eine andere Regel zuerst? (überprüfe die Regelreihenfolge)
- Testest du in Safari? (die Erweiterung funktioniert nur in Safari, nicht in anderen Browsern)

---

## Tweaks

### Was sind Tweaks?

Moderne Websites schränken oft ein, was du in deinem eigenen Browser tun kannst. Sie deaktivieren die Textauswahl, um das Kopieren zu verhindern, spielen Videos automatisch ab, um Engagement-Metriken zu steigern, und zeigen aufdringliche Popups, um dich am Verlassen zu hindern.

Tweaks geben dir die Kontrolle zurück:

- Textauswahl auf Seiten wieder aktivieren, die sie blockieren
- Automatische Video- und Audiowiedergabe blockieren
- Dark Mode auf jeder Website erzwingen
- "Möchtest du diese Seite wirklich verlassen?"-Popups entfernen
- Und mehr

Alle Tweaks sind optional, du entscheidest also, welche du aktivierst.

### Wie aktiviere ich Tweaks?

1. Gehe zum **Tweaks**-Tab
2. Durchsuche die verfügbaren Optionen
3. Schalte jeden Tweak ein oder aus
4. Änderungen werden sofort wirksam

### Warum funktioniert ein Tweak auf einer bestimmten Seite nicht?

Einige Websites wehren sich aktiv gegen Modifikationen. Wenn ein Tweak nicht funktioniert:

- Die Seite verwendet möglicherweise aggressive Anti-Modifikations-Techniken
- Versuche, andere Erweiterungen zu deaktivieren, um Konflikte auszuschließen
- Melde das Problem auf GitHub. Wir verbessern ständig die Kompatibilität.

### Was ist der Unterschied zwischen "Mediensteuerung erzwingen" und "Autoplay blockieren"?

- **Mediensteuerung erzwingen**: Zeigt die Standard-Browser-Video-/Audio-Steuerelemente an, auch wenn die Seite sie versteckt
- **Autoplay blockieren**: Verhindert, dass Videos/Audio automatisch abgespielt werden, wenn du eine Seite lädst

Du kannst beide zusammen verwenden für maximale Kontrolle.

---

## Archivsuche

### Was ist die Archivsuche?

Das Web ist nicht dauerhaft. Seiten werden gelöscht, Artikel werden bearbeitet und ganze Websites verschwinden. Die Wayback Machine des Internet Archive und ähnliche Dienste bewahren Schnappschüsse des Webs auf und schaffen so eine historische Aufzeichnung dessen, was zu einem bestimmten Zeitpunkt existierte.

Die Archivsuche gibt dir sofortigen Zugang zu diesen gespeicherten Versionen:

- Gelöschte Inhalte finden oder sehen, wie eine Seite aussah, bevor sie geändert wurde
- Auf Seiten zugreifen, wenn eine Website vorübergehend nicht erreichbar ist
- Recherchieren, wie sich Websites und ihre Behauptungen im Laufe der Zeit entwickelt haben
- Zitate und Quellenangaben überprüfen, die möglicherweise verändert wurden

### Wie durchsuche ich ein Archiv?

**Von Safari aus:**
1. Tippe auf das **AA**-Symbol oder den **Erweiterungen**-Button
2. Wähle **Trackless Links**
3. Tippe auf den gewünschten Archivdienst (z.B. Wayback Machine)
4. Die aktuelle Seite wird in diesem Archiv gesucht

**Von jeder App aus (Share Sheet):**
1. Teile einen Link aus einer beliebigen App
2. Wähle **Im Archiv suchen**
3. Wähle deinen bevorzugten Archivdienst

### Kann ich weitere Archivdienste hinzufügen?

Ja. Du kannst eigene Archivdienste hinzufügen:

1. Gehe zu **Tweaks**, dann **Archivsuche**, dann **Dienste konfigurieren**
2. Tippe auf **+**, um einen Dienst hinzuzufügen
3. Gib das URL-Muster des Archivdienstes ein
4. Der Dienst ist jetzt im Popup verfügbar

### Sollte ich "Query-Parameter entfernen" aktivieren?

Empfohlen: Ja. Diese Option entfernt Tracking-Codes und andere Parameter vor der Archivsuche, was oft zu besseren Treffern führt. Deaktiviere sie nur, wenn du nach einer URL mit bestimmten Parametern suchen musst.

---

## Share Sheet-Integration

### Wie nutze ich das Share Sheet zum Bereinigen von Links?

Wenn du Links aus anderen Apps teilst, sind Tracking-Parameter mit dabei. Die Share Sheet-Erweiterung ermöglicht es dir, Links vor dem Teilen zu bereinigen:

1. Tippe in einer beliebigen App (Safari, Reddit, X usw.) auf den **Teilen**-Button
2. Scrolle und finde **Mit Trackless Links bereinigen**
3. Die bereinigte URL wird in deine Zwischenablage kopiert

Jetzt kannst du einen sauberen Link teilen, der nicht verrät, wo du ihn gefunden hast, und nicht jeden trackt, der ihn anklickt.

### Kann ich von anderen Apps aus in Archiven suchen?

Ja. Verwende dasselbe Share Sheet:

1. Tippe bei einem beliebigen Link auf **Teilen**
2. Wähle **Im Archiv suchen**
3. Wähle deinen Archivdienst
4. Safari öffnet sich mit den Archiv-Suchergebnissen

---

## iCloud-Synchronisierung

### Wie funktioniert die iCloud-Synchronisierung?

Deine Datenschutz-Einstellungen begleiten dich überall. Wenn du die iCloud-Synchronisierung aktivierst, wird deine Konfiguration automatisch über deinen persönlichen iCloud-Account auf iPhone, iPad und Mac synchronisiert:

- **Filter** (Tracking-Parameter)
- **Weiterleitungen** (eigene Regeln und Aktivierungsstatus)
- **Tweaks** (alle Einstellungen)
- **Archivdienste** (deine konfigurierten Dienste)

Datenschutz-Statistiken (wie die Anzahl blockierter Tracker) bleiben gerätespezifisch und werden nicht synchronisiert.

### Muss ich die iCloud-Synchronisierung aktivieren?

Sie ist optional. Die iCloud-Synchronisierung ist standardmäßig deaktiviert. So aktivierst du sie:

1. Gehe in der App zu **Einstellungen**
2. Finde **iCloud-Synchronisierung**
3. Schalte sie **ein**

Deine Einstellungen werden jetzt auf allen Geräten synchronisiert, die mit demselben iCloud-Account angemeldet sind.

### Meine Änderungen werden nicht zwischen Geräten synchronisiert. Was ist falsch?

Überprüfe Folgendes:

- Ist die iCloud-Synchronisierung auf beiden Geräten **aktiviert**?
- Sind beide Geräte mit **demselben iCloud-Account** angemeldet?
- Ist iCloud Drive in den **Systemeinstellungen** (Mac) oder **Einstellungen** (iOS) aktiviert?
- Sind beide Geräte mit dem Internet verbunden?
- Versuche, die App zu beenden und neu zu öffnen

Wenn die Synchronisierung immer noch nicht funktioniert, versuche, die iCloud-Synchronisierung aus- und wieder einzuschalten.

### Kann ich Trackless Links ohne iCloud verwenden?

Ja. Die iCloud-Synchronisierung ist vollständig optional. Die App funktioniert einwandfrei mit lokal auf jedem Gerät gespeicherten Einstellungen.

---

## Tipps und Tricks

### Wie kann ich sehen, welche Tracking-Parameter entfernt wurden?

Schau dir die **Statistiken** auf dem Haupt-Dashboard an. Sie zeigen:
- Insgesamt bereinigte URLs
- Angewendete Weiterleitungen

### Kann ich meine Einstellungen exportieren?

Einstellungen werden in iCloud (falls aktiviert) oder lokal auf deinem Gerät gespeichert. Alle Daten bleiben unter deiner Kontrolle und werden niemals an Drittanbieter-Server gesendet.

### Verlangsamt Trackless Links das Surfen?

Nein. Die Erweiterung ist extrem leichtgewichtig und verarbeitet URLs in Millisekunden, bevor Seiten fertig geladen werden. Du wirst keinen Leistungsunterschied bemerken.

### Kann ich Trackless Links mit anderen Safari-Erweiterungen verwenden?

Ja. Trackless Links ist so konzipiert, dass es mit anderen Erweiterungen zusammenarbeitet. Bei Konflikten versuche, die Ausführungsreihenfolge in den Safari-Erweiterungseinstellungen anzupassen.

### Was ist der Unterschied zwischen Trackless Links und Trackless Links Pro?

| Funktion | Trackless Links | Trackless Links Pro |
|----------|----------------|---------------------|
| iPhone und iPad | Ja | Ja |
| Mac-App | Nein | Ja |
| iCloud-Synchronisierung | Ja | Ja |
| Preis | Einmalkauf (nur iOS) | Universalkauf (alle Plattformen) |

Trackless Links Pro ist ein Universalkauf. Einmal kaufen und auf iPhone, iPad und Mac nutzen.

---

## Problembehandlung

### Ich kann die Erweiterung in Safari nicht finden

Stelle sicher:
- Du hast die App aus dem App Store installiert
- Du hast die App mindestens einmal geöffnet
- Safari-Erweiterungen sind in deinen Systemeinstellungen aktiviert

### Links werden nicht bereinigt

Überprüfe:
- Ist die Erweiterung in Safari **aktiviert**?
- Hast du die erforderlichen Berechtigungen erteilt?
- Sind Filter im Filter-Tab **aktiviert**?

### Meine eigene Weiterleitung funktioniert nicht

- Überprüfe die Mustersyntax (versuche zuerst eine exakte Übereinstimmung)
- Stelle sicher, dass die Regel **aktiviert** ist
- Überprüfe, ob keine andere Regel zuerst passt (Regelreihenfolge beachten)
