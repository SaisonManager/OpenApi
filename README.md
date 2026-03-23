# SaisonManager API v2 - Clients & OpenAPI Spec 🏑

Dieses Repository enthält eine inoffizielle [OpenAPI-Spezifikation](openapi.json) für die **SaisonManager API (v2)**, die primär für Floorball-Spieldaten genutzt wird. 

Da die externe API v2 historisch wertvolle, aber abgeschlossene Saisondaten liefert, sichert dieses Projekt den nahtlosen und typisierten Zugriff auf diese Daten, selbst wenn das Backend in Zukunft auf neuere Versionen aktualisiert wird.

Aus der OpenAPI-Spezifikation werden automatisch einsatzbereite API-Clients für **C# (.NET)** und **TypeScript** generiert und über GitHub Packages bereitgestellt.

🌐 **Zur interaktiven API-Dokumentation (Swagger UI):** [sm-openapi.floorball.fan](https://sm-openapi.floorball.fan/)

---

## 📦 Verfügbare Pakete

Die generierten Pakete werden bei jedem Push in den `main`-Branch automatisch gebaut und in der GitHub Package Registry veröffentlicht. In den jeweiligen Paketen auf GitHub findest du zudem spezifische Code-Beispiele zur Nutzung.

### TypeScript / Node.js
**Paketname:** `@saisonmanager/saisonmanager-api-v2`

**Installation:**
Um Pakete aus der GitHub Registry zu installieren, musst du zunächst sicherstellen, dass deine `.npmrc` Datei auf den GitHub-Scope zeigt:

```bash
echo "@saisonmanager:registry=[https://npm.pkg.github.com](https://npm.pkg.github.com)" >> .npmrc
```

Anschließend kannst du das Paket ganz normal installieren:

```bash
npm install @saisonmanager/saisonmanager-api-v2
```

### C# / .NET
**Paketname:** `SaisonManager.Api.V2`

**Installation:**
Füge die GitHub NuGet Registry als Paketquelle (Source) in deiner `nuget.config` oder per Kommandozeile hinzu:

```bash
dotnet nuget add source "[https://nuget.pkg.github.com/SaisonManager/index.json](https://nuget.pkg.github.com/SaisonManager/index.json)" --name "GitHub" --username "DEIN_GITHUB_NAME" --password "DEIN_GITHUB_PAT"
```

Installiere dann das Paket:

```bash
dotnet add package SaisonManager.Api.V2
```

---

## 🔑 Authentifizierung (GitHub Packages)
Da die Pakete in der GitHub Registry gehostet werden, benötigst du (oder andere Entwickler) ein **Personal Access Token (PAT)** mit der Berechtigung `read:packages`, um sie herunterladen zu können. 

* [Anleitung: GitHub PAT erstellen](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

## 🛠️ Lokale Entwicklung & Generierung
Wenn du die `openapi.json` anpasst und die Clients lokal generieren möchtest, kannst du das CLI-Tool von OpenAPI Generator nutzen:

```bash
# TypeScript generieren
npx @openapitools/openapi-generator-cli generate -i openapi.json -g typescript-fetch -o ./generated/typescript

# C# generieren
npx @openapitools/openapi-generator-cli generate -i openapi.json -g csharp -o ./generated/csharp
```