# Assignment - First images and containers with Docker

Käytän esimerkkipalvelinta Käyttäjäkeskeinen sovelluskehitys -kurssilta. Tarkistaakseni, että se toimii paikallisesti, suoritin komennot npm i ja npm run dev. Vahvistettuani, että se toimii, alustasin Dockerin komennolla docker init.

Kävin läpi Dockerfile-tiedoston ja lisäsin watch-konfiguraation compose.yaml-tiedostoon. Muutin myös isäntäosoitteen index.js-tiedostossa osoitteeseen 0.0.0.0.

Lisäsin Mongo-toiminnallisuuden suorittamalla ensin komennon $env:MONGODB_VERSION="6.0-ubi8" ja sitten docker run --name mongodb -d mongodb/mongodb-community-server:$env:MONGODB_VERSION. Lisäsin myös Mongon compose.yaml-tiedostoon.

Lopuksi käytin komentoa docker compose up --build sovelluksen rakentamiseen mutta se ei toimi Dockerin kanssa.
