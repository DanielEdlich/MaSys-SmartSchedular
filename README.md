# Willkommen bei SmartSchedular!

Diese Repository dient als die Code-Basis für die Entwicklung von SmartSchedular. SmartSchedular ist ein Tool, das die Erstellung von Stundenplänen für Schüler und Lehrer erleichtert. Es bietet eine einfache und intuitive Benutzeroberfläche, die es ermöglicht, Stundenpläne zu erstellen, zu bearbeiten und zu verwalten. Sm

## Erste Schritte - Anwendung starten

Zuerst sollte der Entwicklungsserver gestartet werden:

```bash
npm install
# oder
pnpm install
```

```bash
npm run dev
# oder
pnpm dev
```

[http://localhost:3000](http://localhost:3000) sollte in deinem Browser geöffnet werden, um das Ergebnis zu sehen.

Die Seite kann bearbeitet werden, indem `app/page.tsx` modifiziert wird. Die Seite wird automatisch aktualisiert, wenn die Datei bearbeitet wird.


## Struktur des Projekts

### `src/`
- Enthält den gesamten Code deiner Anwendung.
- Die zentrale Organisation für deine App.

### `src/app/`
- **`page.tsx`**: Definiert eine Seite. Z. B. `src/app/page.tsx` ist die Startseite (`/`).
- **`layout.tsx`**: Definiert das Layout (z. B. Header, Footer) für eine Seite oder eine Gruppe von Seiten.
- **Unterseiten**: Erstelle Unterverzeichnisse mit einer eigenen `page.tsx`, um neue Routen hinzuzufügen (z. B. `src/app/unterseite/page.tsx` wird `/unterseite`).

### `src/components/`
- Enthält wiederverwendbare Komponenten (z. B. Buttons, Header).

### `src/styles/`
- Hier können CSS-Dateien oder CSS-Module abgelegt werden.

### `public/`
- Statische Dateien wie Bilder oder Icons. Inhalte sind direkt über die URL zugänglich.
  - Beispiel: `public/images/logo.png` ist unter `http://localhost:3000/images/logo.png` erreichbar.

### `next.config.js`
- Konfigurationsdatei für dein Projekt (z. B. benutzerdefinierte Routen oder Umgebungsvariablen).


## ✏️ Neue Seite hinzufügen

### 1. Neue Seite erstellen:
- Erstelle die Datei `src/app/neue-seite/page.tsx`:
  ```tsx
  export default function NeueSeite() {
    return <h1>Willkommen auf der neuen Seite!</h1>;
  }


## Abhängigkeiten und Versionsnummern

Die Abhängigkeiten und Versionsnummern sind in der `package.json` Datei definiert:

```json
{
  "dependencies": {
    "react": "^18",
    "react-dom": "^18",
    "next": "14.2.18"
  },
  "devDependencies": {
    "typescript": "^5",
    "@types/node": "^20",
    "@types/react": "^18",
    "@types/react-dom": "^18",
    "postcss": "^8",
    "tailwindcss": "^3.4.1",
    "eslint": "^8",
    "eslint-config-next": "14.2.18"
  }
}
```


## Mehr erfahren

Um mehr über Next.js zu erfahren, sollten die folgenden Ressourcen angesehen werden:

- [Next.js Dokumentation](https://nextjs.org/docs) - mehr über die Funktionen und die API von Next.js lernen.
- [Lerne Next.js](https://nextjs.org/learn) - ein interaktives Next.js Tutorial.


## ShadCN Komponenten hinzufügen

ShadCN bietet eine Reihe von Komponenten, die in dein Projekt eingefügt werden können. Die Komponenten können mit dem folgenden Befehl hinzugefügt werden:

```bash
npx shadcn add <gewünschte Komponente>
```

## Auf Vercel bereitstellen

Der einfachste Weg, die Next.js App bereitzustellen, ist die Verwendung der [Vercel Plattform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) von den Erstellern von Next.js.

Die [Next.js Bereitstellungsdokumentation](https://nextjs.org/docs/app/building-your-application/deploying) sollte für weitere Details angesehen werden.
