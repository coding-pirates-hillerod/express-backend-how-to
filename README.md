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

Databehandling: 
- Håndtering af data, forretningslogik og regler.
- Database: Lagring, hentning og opdatering af data (fx MySQL, PostgreSQL, MongoDB).
- Autentificering & sikkerhed: Håndtering af login, sessions og brugerrettigheder.
- API’er: Tillader kommunikation mellem frontend og backend via fx REST eller GraphQL.
- Serverdrift: Kører på en server (fx Node.js, Python, Java, PHP) og sikrer, at systemet fungerer.

##### Eksempel
Når du fx bruger en webshop, så består denne så at sige af følgende 2 dele (hvor vi her vil beskæftige os med 'backend' delen selvfølgelig):

- **Frontend**: Du ser produkterne og tilføjer noget til kurven.
- **Backend**: Tjekker lagerstatus, beregner priser, gemmer ordren i databasen og sender bekræftelsesmail.

Så kort sagt: Backend er hjernen bag en applikation, som får den til at fungere. 🚀

