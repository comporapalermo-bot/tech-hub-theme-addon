Redme

TechHub Theme Addon - Installazione

1. Carica il contenuto di "assets" in Online Store > Themes > Edit code > assets.
2. Carica i file in "snippets" nella cartella snippets del tema.
3. Carica i file in "sections" nella cartella sections del tema.
4. Includi gli snippet nel layout:
   - In theme.liquid aggiungi: {% render 'tech-header' %}
   - In homepage aggiungi la nuova sezione: Hero Tech (hero-tech).
5. Assicurati di collegare CSS e JS:
   {{ 'tech-style.css' | asset_url | stylesheet_tag }}
   <script src="{{ 'tech-scripts.js' | asset_url }}" defer="defer"></script>
6. Sostituisci immagini segnaposto con le tue (hero-console.jpg).
7. Per i prodotti, usa {% render 'product-card-tech', product: product %} nelle collection templates.
