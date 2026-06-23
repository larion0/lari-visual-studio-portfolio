# Lari Visual Studio portfolio weboldal

Ez a mappa a GitHubra és Cloudflare Pages-re feltölthető statikus weboldalhoz tartozik.

## Ezeket töltsd fel GitHubra

Csak ezek kellenek az élő weboldalhoz:

- `index.html`
- `assets/portfolio/`
- `README.md` opcionális, csak útmutató

A régi ZIP fájlok, Canva-próbák, `script.js`, `styles.css`, `services.html` és egyéb munkamappák nem kellenek ehhez a kész oldalhoz.

## GitHub feltöltés

1. Hozz létre egy új GitHub repositoryt.
2. A repository fő gyökerébe töltsd fel az `index.html` fájlt.
3. Mellé töltsd fel az `assets` mappát úgy, hogy az útvonal így maradjon:

```text
index.html
assets/
  portfolio/
    képek...
```

Fontos: az `assets/portfolio` mappa neve ne változzon, mert a HTML innen tölti be a képeket.

## Cloudflare Pages beállítás

Cloudflare Pages-ben a GitHub repositoryt válaszd ki.

Ajánlott beállítások:

- Framework preset: `None`
- Build command: hagyd üresen
- Build output directory: `/` vagy hagyd üresen, ha Cloudflare engedi
- Root directory: a repository fő mappája

Ez egy sima statikus HTML oldal, nincs szükség külön buildre.

## Contact Us űrlap

Az űrlap jelenleg a FormSubmit szolgáltatáson keresztül küldi az üzeneteket erre az email címre:

```text
larivisualstudio@proton.me
```

Az első éles teszt beküldés után a FormSubmit küldhet egy megerősítő emailt erre a Proton címre. Azt jóvá kell hagyni. Utána az űrlapon küldött üzenetek a Proton bejövő leveleid közé érkeznek.

Az `Email Directly` gomb közvetlen email ablakot nyit a látogatónál, ha neki be van állítva email kliens.
