# BuildV Themes

Repositório de layouts Elementor para uso com o plugin **BuildV Layouts**.

## Estrutura

```
buildv-themes/
├── layouts.json          ← índice principal
├── templates/
│   └── hero-001.json     ← JSONs exportados do Elementor
└── thumbs/
    └── hero-001.jpg      ← screenshots dos layouts (800×500px)
```

## Como adicionar um layout

1. Monte a seção no Elementor
2. Salve como Template → exporte como `.json`
3. Suba o `.json` em `templates/`
4. Suba o screenshot em `thumbs/`
5. Adicione a entrada em `layouts.json`:

```json
{
  "id": "meu-layout-001",
  "name": "Nome do Layout",
  "category": "hero",
  "thumbnail": "https://seuusuario.github.io/buildv-themes/thumbs/meu-layout-001.jpg",
  "template_url": "https://seuusuario.github.io/buildv-themes/templates/meu-layout-001.json"
}
```

## Publicar no GitHub Pages

1. Crie o repositório como **Public** com o nome `buildv-themes`
2. Suba todos os arquivos
3. Vá em **Settings → Pages → Source: main**
4. URL final: `https://seuusuario.github.io/buildv-themes`
5. Cole essa URL nas configurações do plugin BuildV Layouts no WordPress
