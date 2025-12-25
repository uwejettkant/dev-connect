<div align="center">
  <h3 align="center">DevConnect - Event Management Platform</h3>

   <div align="center">
    Folge der nachstehenden Anleitung, um diese Anwendung Schritt für Schritt einzurichten.
    </div>
</div>

## 📋 <a name="table">Inhaltsverzeichnis</a>

1. ✨ [Überblick](#introduction)
2. ⚙️ [Technologie-Stack](#tech-stack)
3. 🔋 [Funktionen](#features)
4. 🤸 [Erste Schritte](#quick-start)
5. 🔗 [Ressourcen](#links)
6. 🚀 [Weitere Informationen](#more)


## <a name="introduction">✨ Überblick</a>

Eine vollständige Event-Management-Plattform zur nahtlosen Verwaltung und Präsentation von Veranstaltungen. Die Anwendung bietet eine interaktive Startseite mit anstehenden Events, vollwertige API-Endpunkte für alle CRUD-Operationen, cloudbasierte Bildverwaltung via Cloudinary, umfassende Event-Detailseiten mit Registrierungsfunktion sowie Vorschläge für ähnliche Veranstaltungen. 

## <a name="tech-stack">⚙️ Technologie-Stack</a>

- **[Cloudinary](https://cloudinary.com/?utm_campaign=1329&utm_content=instapagelogocta-selfservetest)** – Eine cloudbasierte Medienplattform zur Vereinfachung von Bild- und Video-Uploads, Speicherung, Optimierung und Auslieferung. Sie ermöglicht eine effiziente Medienverwaltung und verbessert die Website-Performance.

- **[MongoDB](https://www.mongodb.com/products/platform/atlas-database)** – Eine flexible, dokumentenorientierte NoSQL-Datenbank, die Daten im JSON-ähnlichen Format speichert. Perfekt geeignet für moderne Anwendungen, die Skalierbarkeit, hohe Performance und flexible Schemas benötigen.

- **[Mongoose](https://mongoosejs.com/)** – Eine ODM-Bibliothek (Object Data Modeling) für MongoDB und Node.js. Sie bietet ein schemabasiertes System zur Modellierung von Anwendungsdaten, Validierung von Eingaben und effizienter Verwaltung von Datenbankinteraktionen.

- **[Next.js](https://nextjs.org/docs)** – Ein leistungsstarkes React-Framework zum Erstellen von Full-Stack-Webanwendungen. Es vereinfacht die Entwicklung durch Features wie Server-Side Rendering, Static Site Generation und API-Routen, sodass sich Entwickler auf das Produkt konzentrieren können.

- **[Tailwind CSS](https://tailwindcss.com/)** – Ein Utility-First CSS-Framework, das es Entwicklern ermöglicht, schnell individuelle Benutzeroberflächen mit minimalem Custom-CSS zu erstellen. Es fördert Konsistenz, Responsivität und schnelleres Styling direkt im HTML.

- **[TypeScript](https://www.typescriptlang.org/)** – Eine Erweiterung von JavaScript mit statischer Typisierung, die besseres Tooling, höhere Code-Qualität und frühzeitige Fehlererkennung bietet. Ideal für große Anwendungen und eine verbesserte Developer Experience.

- **[Warp](https://go.warp.dev/js-mastery)** – Ein modernes Terminal für Geschwindigkeit, Zusammenarbeit und Benutzerfreundlichkeit. Es steigert die Produktivität durch intelligente Befehle, Workflows und Session-Sharing.



## <a name="features">🔋 Funktionen</a>

👉 **Startseite**: Zeigt eine dynamische Liste von Veranstaltungen, sodass Nutzer kommende und hervorgehobene Events durchsuchen können.  

👉 **API-Endpunkte**: Vollständige CRUD-Operationen zum Erstellen, Aktualisieren, Löschen und Abrufen von Events aus der Datenbank.  

👉 **Cloudinary-Integration**: Nutzt das Cloudinary SDK für unkompliziertes Hochladen und Verwalten von Bildern in der Cloud.  

👉 **Event-Detailseite**: Präsentiert ausführliche Event-Informationen mit Registrierungsmöglichkeit und zeigt eine Liste ähnlicher Veranstaltungen.  

👉 **Next.js 16 Caching**: Implementiert einen völlig neuen Caching-Ansatz für verbesserte Performance und schnellere Ladezeiten.  


Und viele weitere Features, einschließlich durchdachter Code-Architektur und Wiederverwendbarkeit.

## <a name="quick-start">🤸 Erste Schritte</a>

Befolge diese Schritte, um das Projekt lokal auf deinem Rechner einzurichten.

**Voraussetzungen**

Stelle sicher, dass folgende Software auf deinem System installiert ist:

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/en)
- [npm](https://www.npmjs.com/) (Node Package Manager)

**Repository klonen**

```bash
git clone https://github.com/uwejettkant/dev-connect

cd dev-connect
```

**Abhängigkeiten installieren**

Installiere die Projekt-Dependencies mit npm:

```bash
npm install
```

**Umgebungsvariablen konfigurieren**

Erstelle eine neue Datei namens `.env` im Projekt-Root und füge folgenden Inhalt hinzu:

```env
NEXT_PUBLIC_BASE_URL=http://localhost:3000/

MONGODB_URI=

CLOUDINARY_URL=

```

Ersetze die Platzhalter mit deinen echten Zugangsdaten. Diese erhältst du hier: 
[**Cloudinary**](https://cloudinary.com/?utm_campaign=1329&utm_content=instapagelogocta-selfservetest),
[**MongoDB**](https://www.mongodb.com/products/platform/atlas-database), 

**Anwendung starten**

```bash
npm run dev
```

Öffne [http://localhost:3000](http://localhost:3000) in deinem Browser, um die Anwendung anzuzeigen.

## 📊 Datenbankschema

### Event-Schema

Events müssen in der MongoDB-Datenbank mit folgendem Schema angelegt werden:

```json
{
  "title": "Cloud Next 2026",
  "description": "Google's premier cloud computing event, showcasing innovations in AI, infrastructure, and enterprise solutions.",
  "overview": "Cloud Next 2025 highlights the latest in cloud-native development, Kubernetes, AI, and enterprise scalability. Developers, architects, and executives gather to learn about new Google Cloud services, best practices, and success stories.",
  "image": "image Url",
  "venue": "Moscone Center",
  "location": "San Francisco, CA",
  "date": "2025-04-10",
  "time": "08:30",
  "mode": "Hybrid (In-Person & Online)",
  "audience": "Cloud engineers, DevOps, enterprise leaders, AI researchers",
  "agenda": [
    "08:30 AM - 09:30 AM | Keynote: AI-Driven Cloud Infrastructure",
    "09:45 AM - 11:00 AM | Deep Dives: Kubernetes, Data Analytics, Security",
    "11:15 AM - 12:30 PM | Product Demos & Networking",
    "12:30 PM - 01:30 PM | Lunch",
    "01:30 PM - 03:00 PM | Workshops: Scaling with GCP",
    "03:15 PM - 04:30 PM | Fireside Chat: The Future of Enterprise Cloud"
  ],
  "organizer": "Google Cloud organizes Cloud Next to connect global businesses, developers, and innovators with the latest technologies and best practices in cloud computing.",
  "tags": ["Cloud", "DevOps", "Kubernetes", "AI"]
}
```

**Feld-Beschreibungen:**

- **title** (String): Der Event-Name
- **description** (String): Eine kurze Zusammenfassung des Events
- **overview** (String): Detaillierte Beschreibung des Events
- **image** (String): URL zum Event-Bild (via Cloudinary gehostet)
- **venue** (String): Name der Veranstaltungslocation
- **location** (String): Stadt und Land des Events
- **date** (String): Datum im Format YYYY-MM-DD
- **time** (String): Startzeit im Format HH:MM
- **mode** (String): Veranstaltungsformat (z.B. In-Person, Online, Hybrid)
- **audience** (String): Zielgruppe des Events
- **agenda** (Array): Liste der geplanten Sessions mit Zeitangaben
- **organizer** (String): Information über den Veranstalter
- **tags** (Array): Kategorien/Themen des Events

