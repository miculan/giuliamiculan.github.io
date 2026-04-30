# Portfolio Giulia Miculan

Sito portfolio professionale per Giulia Miculan - Collection care specialist & restauratrice.

## Struttura del progetto

```
giulia-miculan-portfolio/
├── _config.yml                 # Configurazione Jekyll
├── Gemfile                     # Dipendenze Ruby
├── README.md                   # Questo file
├── index.html                  # Homepage
├── _layouts/                   # Template delle pagine
│   ├── default.html           # Layout principale
│   └── page.html              # Layout pagine standard
├── pages/                      # Pagine del sito
│   ├── about.md               # Chi sono
│   ├── progetti.html          # Portfolio
│   └── contatti.md            # Contatti
└── assets/                     # Risorse statiche
    ├── css/
    │   └── style.css          # Stili CSS
    └── images/                # Immagini (da aggiungere)
```

## Installazione

### Prerequisiti

- Ruby 2.7 o superiore
- RubyGems
- GCC e Make

### Installazione su macOS

```bash
# Installa Ruby (se non presente)
brew install ruby

# Aggiungi Ruby al PATH
echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

### Installazione su Windows

Scarica e installa [RubyInstaller](https://rubyinstaller.org/) con DevKit.

### Installazione su Linux

```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
```

## Setup del progetto

1. Crea la struttura delle cartelle:

```bash
mkdir giulia-miculan-portfolio
cd giulia-miculan-portfolio
mkdir -p _layouts pages assets/css assets/images
```

2. Copia tutti i file nelle rispettive posizioni seguendo la struttura sopra indicata.

3. Installa le dipendenze:

```bash
gem install bundler
bundle install
```

4. Avvia il server di sviluppo:

```bash
bundle exec jekyll serve
```

5. Apri il browser all'indirizzo: `http://localhost:4000`

## Personalizzazione

### Modificare le informazioni personali

Modifica il file `_config.yml` per aggiornare:
- Email, telefono, P.IVA
- Link ai social media
- Descrizione del sito

### Aggiungere immagini

1. Carica le tue immagini nella cartella `assets/images/`
2. Riferisci alle immagini nei file usando il percorso relativo:
   ```
   ![Descrizione](/assets/images/nome-immagine.jpg)
   ```

### Modificare i contenuti

- **Homepage**: modifica `index.html`
- **Chi sono**: modifica `pages/about.md`
- **Portfolio**: modifica `pages/progetti.html`
- **Contatti**: modifica `pages/contatti.md`

### Modificare lo stile

Modifica il file `assets/css/style.css` per personalizzare:
- Colori (variabili CSS in `:root`)
- Font
- Layout e spaziature

## Deployment

### GitHub Pages

1. Crea un repository su GitHub chiamato `username.github.io` (sostituisci `username` con il tuo username GitHub)
2. Pusha il codice:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/username.github.io.git
git push -u origin main
```

3. Il sito sarà disponibile su `https://username.github.io`

### Netlify

1. Connetti il repository GitHub a Netlify
2. Impostazioni build:
   - Build command: `jekyll build`
   - Publish directory: `_site`

## Manutenzione

### Aggiungere nuovi progetti

Per aggiungere progetti al portfolio, modifica il file `pages/progetti.html` seguendo la struttura esistente degli `article` con classe `project-item`.

### Aggiornare il CV

Modifica `pages/about.md` per aggiornare esperienze lavorative, formazione e pubblicazioni.

## Supporto

Per problemi o domande:
- Email: giulia@miculan.org
- LinkedIn: [Giulia Miculan](https://linkedin.com/in/giulia-miculan)

## Licenza

© 2026 Giulia Miculan. Tutti i diritti riservati.