# Master — A Monster Rapallo Nuoto

Prima versione di prototipo interattivo per la web app installabile.

## Avvio locale
Apri `index.html` nel browser per una prova rapida. Per verificare la PWA/service worker serve un server HTTP/HTTPS, ad esempio GitHub Pages o Cloudflare Pages.

## Schermate incluse
- Accesso e scelta del percorso atleta/coach
- Home
- Allenamenti settimanali
- Calendario con selezione della data
- Bacheca comunicazioni
- Profilo e diario personale dei tempi

## Importante: questa non è ancora la versione online sicura
Questo pacchetto è un prototipo frontend. Usa dati demo e `localStorage` del browser. Il cambio ruolo è solo una simulazione, non una verifica dei permessi. I tempi salvati qui non sono sincronizzati fra dispositivi e non hanno ancora protezione server-side. **Non inserire dati personali reali né usare questa demo per dati che richiedono riservatezza.**

Prima di usare il sistema con gli atleti:
1. Collegare Supabase per autenticazione e database.
2. Definire ruoli autorizzati lato server.
3. Applicare policy Row Level Security (RLS) ai tempi personali: ogni atleta può leggere e modificare solo i propri record; coach e altri atleti non devono poterli leggere.
4. Spostare allenamenti e bacheca su database condiviso.
5. Testare permessi con account distinti.

## Fasce orarie previste
- 12:45–14:00
- 19:30–21:00

Nel prototipo il coach può scegliere una delle due fasce e pubblicare note per la seduta selezionata.
