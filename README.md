# Studio Legale Maenza - Sito Hugo

Sito web statico generato con [Hugo](https://gohugo.io/) per lo Studio Legale Maenza.

## Informazioni
- Dominio: [www.avvocatomaenza.it](https://www.avvocatomaenza.it)
- Tema: [PaperMod](https://github.com/adityatelange/hugo-PaperMod)
- Hosting: GitHub Pages
- Lingua: Italiano

## Struttura
```
.
├── config.toml          # Configurazione
├── content/             # Contenuti
│   ├── _index.md        # Homepage
│   ├── chi-sono.md      # Chi sono
│   ├── servizi.md       # Servizi
│   ├── articoli/        # Blog
│   │   └── *.md         # Articoli
│   └── contatti.md      # Contatti
├── static/              # File statici
│   └── images/          # Immagini
└── themes/              # Temi
    └── PaperMod/        # Tema (submodule)
```

## Come iniziare

### 1. Aggiungi il tema PaperMod
```bash
git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
git submodule update --init --recursive
git add .gitmodules themes/PaperMod
git commit -m "Add PaperMod theme"
git push origin main
```

### 2. Testa localmente
```bash
hugo server -D
```

Il sito sarà accessibile all'indirizzo: [http://localhost:1313](http://localhost:1313)

## Deploy
Il sito si deploya automaticamente su GitHub Pages al push sul branch main.

## Personalizzazione
- Modifica i file in `content/` per aggiungere contenuti
- Modifica `config.toml` per personalizzare il sito
- Aggiungi immagini in `static/images/`
