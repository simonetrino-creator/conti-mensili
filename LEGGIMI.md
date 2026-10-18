# Conti del mese – compilazione online con GitHub

Non serve installare nulla: GitHub costruisce l’APK per te.

1. Crea un account gratuito su https://github.com
2. Clicca **+** in alto a destra → **New repository**. Nome: `conti-mensili`. Scegli **Private**. Clicca **Create repository**.
3. Nella pagina del repository clicca **uploading an existing file**. Trascina dentro TUTTO il contenuto di questa cartella (`www`, `package.json`, `capacitor.config.json`, `.gitignore` e la cartella nascosta `.github`). Clicca **Commit changes**.
4. Se `.github` non è stata caricata (le cartelle nascoste a volte vengono saltate): **Add file → Create new file**, scrivi nel nome `.github/workflows/build.yml`, incolla il contenuto del file `build.yml` e clicca **Commit changes**.
5. Vai nella scheda **Actions**. Vedrai “Crea APK” in esecuzione (3–6 minuti). Se non parte: clicca “Crea APK” → **Run workflow**.
6. Quando compare la spunta verde, apri l’esecuzione e in fondo, sotto **Artifacts**, clicca `conti-del-mese-apk`. Scarica uno zip con dentro `app-debug.apk`.
7. Decomprimi, porta l’APK sul telefono e installalo (consenti l’installazione da origini sconosciute).

## Aggiornare l’app
Modifica `www/index.html` su GitHub (icona matita) e conferma: l’APK viene ricostruito da solo.

## Note
- I dati restano sul telefono, offline. Il codice su GitHub non contiene i tuoi dati.
- Se disinstalli l’app i dati vanno persi: usa “Esporta CSV” come copia di sicurezza.
- Reinstallando un APK più recente sopra quello vecchio i dati restano.
