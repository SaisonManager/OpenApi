# SaisonManager API v2 - Clients & OpenAPI 🏑

Dieses Repository bietet eine inoffizielle [OpenAPI-Spezifikation](openapi.json) und automatisch generierte, typisierte Clients für die **SaisonManager API (v2)**.

## 🌐 Dokumentations-Portal
Die vollständige Dokumentation inklusive interaktiver API-Referenz und SDK-Guides findest du hier:
👉 **[sm-openapi.floorball.fan](https://sm-openapi.floorball.fan/)**

---

## 📦 Verfügbare Pakete

Alle Pakete werden automatisch bei jedem Push in den `main`-Branch aktualisiert und in der **GitHub Package Registry** veröffentlicht.

### [C# / .NET SDK](https://sm-openapi.floorball.fan/sdk.html?sdk=csharp)
- **NuGet-Name:** `SaisonManager.Api.V2`
- **Installation:** [Guide & Beispiele ansehen](https://sm-openapi.floorball.fan/sdk.html?sdk=csharp)

### [TypeScript / NPM SDK](https://sm-openapi.floorball.fan/sdk.html?sdk=typescript)
- **NPM-Name:** `@saisonmanager/saisonmanager-api-v2`
- **Installation:** [Guide & Beispiele ansehen](https://sm-openapi.floorball.fan/sdk.html?sdk=typescript)

---

## 🛠️ Lokale Entwicklung
Um die Clients lokal zu generieren, nutze den OpenAPI Generator:

```bash
# TypeScript
npx @openapitools/openapi-generator-cli generate -i openapi.json -g typescript-fetch -o ./generated/typescript

# C#
npx @openapitools/openapi-generator-cli generate -i openapi.json -g csharp -o ./generated/csharp
```

---
&copy; 2026 Floorball.Fan