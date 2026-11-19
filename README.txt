PUMP CALLOUT HUNTER V1 — iPhone PWA

Sadržaj:
- index.html: aplikacija
- manifest.webmanifest: instalacija kao web aplikacija
- sw.js: osnovni offline cache za sučelje
- icon-192.png / icon-512.png: ikone

VAŽNO:
1) Ovo je V1 prototip · ispravak prikaza i ocjene podataka. Koristi PumpPortal WebSocket subscribeNewToken.
2) Feed novih tokena je besplatan prema PumpPortal dokumentaciji. Trade stream nije uključen jer može zahtijevati API ključ, financirani wallet i naplatu.
3) Ocjena potpunosti podataka (0–100) mjeri samo prisutnost osnovnih polja događaja kreiranja; nije ocjena kvalitete tokena niti signal za kupnju. INITIAL BUY je količina tokena, ne SOL.
4) Nema wallet povezivanja, privatnih ključeva, kupnje/prodaje ni automatskog objavljivanja.
5) WebSocket radi samo dok je stranica otvorena i mreža dostupna. iOS može pauzirati pozadinske kartice.
6) Za instalaciju na iPhone datoteke moraju biti hostane preko HTTPS-a. Najjednostavnije je GitHub Pages:
   - Napravi GitHub repozitorij (npr. pump-callout-hunter).
   - Uploadaj SVE datoteke iz ovog ZIP-a u root repozitorija.
   - Settings > Pages > Deploy from a branch > main > /(root) > Save.
   - Otvori generirani HTTPS URL u Safariju.
   - Share > Add to Home Screen > Add.
7) Ako se feed ne spoji, provjeri status i da li mreža blokira WebSocket. Neki javni servisi mogu mijenjati uvjete ili ograničenja.

Službeni izvor feeda:
https://pumpportal.fun/data-api/real-time/
