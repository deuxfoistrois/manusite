# manu.blog — Setup

## Estructura de archivos

```
├── index.html                  ← shell del blog (CSS, JS, nav)
├── netlify.toml                ← configuración de Netlify
├── admin/
│   ├── index.html              ← panel de Decap CMS
│   └── config.yml              ← configuración del CMS
├── content/
│   └── articles/
│       ├── englishlatino.json
│       ├── freelunch.json
│       ├── mainstream.json
│       ├── narrativeiap.json
│       ├── narrativegravity.json
│       └── newflatness.json
└── assets/
    ├── about.jpeg              ← foto del about
    └── heroes/
        ├── englishlatino.png
        └── freelunch.webp
```

## Setup inicial (una sola vez)

### 1. Crear repo en GitHub
1. Ir a github.com → New repository
2. Nombre: `manusite`
3. Público o privado (cualquiera)
4. Sin README (lo vas a reemplazar)
5. Subir todos estos archivos

### 2. Conectar Netlify al repo
1. En Netlify: Sites → Add new site → Import from Git
2. Seleccionar el repo `manusite`
3. Build command: (dejar vacío)
4. Publish directory: `.`
5. Deploy

### 3. Habilitar Netlify Identity
1. En Netlify: Site settings → Identity → Enable Identity
2. Registration: Invite only
3. Git Gateway: Enable Git Gateway
4. Invitarte a vos mismo por email

### 4. Entrar al admin
1. Ir a `tudominio.netlify.app/admin`
2. Aceptar la invitación
3. Listo — editás texto, guardás, se publica solo

## Cómo editar un artículo
1. `tudominio.netlify.app/admin`
2. Click en "Articles"
3. Elegir el artículo
4. Editar los campos de texto (Body EN / Body ES / etc.)
5. "Publish" → se publica en 30 segundos

## Agregar un nuevo artículo
Por ahora, pedirle a Vera que genere el JSON y lo agregue al repo.
