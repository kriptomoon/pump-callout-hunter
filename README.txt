PUMP CALLOUT HUNTER V3 — PWA

V3 dodaje ograničeni live BUY/SELL uzorak za najviše 5 tokena istodobno preko PumpDev WebSocket API-ja (wss://pumpdev.io/ws). Novi tokeni se otkrivaju besplatnim subscribeNewToken; aplikacija zatim redom prati svaki token do 2 minute, u okviru anonimne kvote servisa.

VAŽNA OGRANIČENJA:
- Prema trenutno objavljenoj PumpDev dokumentaciji, anonimni pristup bez ključa ima najviše 5 aktivnih token/account pretplata i 1.000 trade poruka mjesečno. Besplatni račun/key ima više, ali V3 ne traži račun niti wallet.
- Ako kvota bude potrošena ili servis promijeni uvjete, trade podaci mogu prestati stizati. Odsutnost podataka NIJE dokaz da nema kupnji/prodaja.
- Signal BUY AKTIVNOST POTVRĐENA samo znači da je u kratkom prozoru zabilježen minimalni uzorak: najmanje 8 transakcija, 5 jedinstvenih kupaca, BUY udio >=65% i neto priljev >=0.5 SOL. To nije preporuka, predviđanje cijene ni sigurnosna provjera. Može zakasniti, biti izmanipulirano i token i dalje može pasti na nulu.
- Podaci su samo live; nema povijesne provjere ni garancije uspješnog callouta.
- Nema wallet povezivanja, privatnih ključeva, kupnje/prodaje ili automatskog objavljivanja.
- Feed radi samo dok je stranica otvorena; iOS može pauzirati pozadinske kartice.

OBJAVA:
Uploadaj/overwrite sve datoteke iz ovog ZIP-a u root GitHub repozitorija. Commit promjene. GitHub Pages će se automatski ponovno objaviti. Nakon objave napravi hard refresh (Ctrl+Shift+R) ili obriši site data ako je potrebno.

Izvori:
https://pumpdev.io/data-api
