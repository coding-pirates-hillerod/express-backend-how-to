# express-backend-how-to

Dette repo forsøger at forklare og vise, hvad en backend er, og hvordan man kan lave, en godt nok meget simpel, backend selv med med [Express.js](https://expressjs.com/).

## 'Backend' .. hvad er det!?

Inden vi går i gang med overhovedet at lave en backend selv, så skal vi lige have følgende på plads:

1. Hvad er en backend?
2. Hvad er Express.js?

### Hvad er en 'backend'?

En backend er den del af et computersystem, en softwareapplikation eller et website, som kører "bag kulisserne" og håndterer logik, databaser, autentificering og kommunikation med frontend (den del, brugeren ser og interagerer med).

#### Hvad gør en 'backend'?

Backend er ansvarlig for:

- Databehandling: Håndtering af data, forretningslogik og regler.
- Database: Lagring, hentning og opdatering af data (fx MySQL, PostgreSQL, MongoDB).
- Autentificering & sikkerhed: Håndtering af login, sessions og brugerrettigheder.
- API’er: Tillader kommunikation mellem frontend og backend via fx REST eller GraphQL.
- Serverdrift: Kører på en server (fx Node.js, Python, Java, PHP) og sikrer, at systemet fungerer.

##### Eksempel

Når du fx bruger en webshop, så består denne så at sige af følgende 2 dele (hvor vi her vil beskæftige os med 'backend' delen selvfølgelig):

- **Frontend**: Du ser produkterne og tilføjer noget til kurven.
- **Backend**: Tjekker lagerstatus, beregner priser, gemmer ordren i databasen og sender bekræftelsesmail.

Så kort sagt: Backend er hjernen bag en applikation, som får den til at fungere. 🚀

### Hvad er Express.js?

Express.js (eller bare Express) er et minimalistisk og fleksibelt webapplikations-framework for Node.js, designet til at bygge webapplikationer og API'er hurtigt og effektivt.

#### Funktioner i Express

Man kan mange ting med Express.js, og nogle af dets funktioner er bl.a.:

- ✅ Routing – Nem håndtering af URL-ruter
- ✅ Middleware – Mulighed for at tilføje funktionalitet som godkendelse, logging og parsing af anmodninger
- ✅ Hurtig og letvægt – Minimal overhead sammenlignet med andre frameworks
- ✅ Understøtter templates – Kan bruge EJS, Pug eller Handlebars til at generere HTML
- ✅ REST API-venligt – Perfekt til at bygge RESTful API'er

##### Eksempel på en simpel Express-server

Som et eksempel på, hvor nemt det er at lave en (super) simpel Express server, der svarer med "Hello World!" på root (/) ruten, så er følgende den eneste kode der er nødvendig til det:

```javascript
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.send("Hello World!");
});

app.listen(3000, () => {
  console.log("Serveren kører på http://localhost:3000");
});
```

## Lav selv din egen Express.js backend

Nu hvor du forhåbentlig har forstået lidt om, hvad en backend er, og hvad er Express.js er og kan i den forbindelse, så gennemgås i det følgende, hvordan du selv laver en simpel backend med Express.js.

Alt koden til nedenstående gennemgang kan i øvrigt findes i mappen kaldet "mybackend" i dette repo.

### Nødvendigt software
For overhovedet at kunne komme i gang med at lave din egen backend med Express.js, så er det nødvendigt at du har/får Node.js installeret.

Node.js er dog heldigvist nemt at installere. Så download derfor Node.js via dette link:

- [Node.js](https://nodejs.org/en)

### Lav en mappe til din backend
Når du har fået installeret Node.js, så er første step at lave en mappe til backend.

Kør derfor først denne kommando fra din terminal/kommandolinje for at lave en ny mappe, som vi her vil kalde "mybackend":

```bash
mkdir mybackend
```

Og når det er gjort, så gå ned i denne nye mappe vhja. følgende kommando:

```bash
cd mybackend
```

### Skab en 'server.js' fil
Efter du er gået ned i din nye "mybackend" mappe, så er det første du skal gøre at lave en ny fil, som er den der vil indeholde koden til din backend.

Kør derfor denne kommando for skabe en fil kaldet "server.js" i din "mybackend" mappe:

```bash
touch server.js
```

### Initialiser din Express backend og projekt
Når du har fået lavet din "server.js" fil, så er det næste du skal at initialisere din backend vhja. en "package manager" kaldet <code>npm</code>, som bliver installeret sammen med Node.js.

Fra din backend mappe skal du derfor blot først køre denne kommando for at initialisere din backend:

```bash
npm init -y
```

Med denne kommando vil der blive skabt en fil kaldet "package.json" i din mappe, som bruges til lidt forskellige ting (for nu vil vi ikke gå så meget op i den, da det primære formål er at lære dig at lave en simpel backend).

### Installer Express
Næste step er nu at installere Express.js, således at du kan begynde at kode din backend.

Installer derfor først express via følgende kommando:

```bash
npm i express
```

