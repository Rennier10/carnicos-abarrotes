# La Despensa del Llano · Cárnicos y abarrotes

Sitio web de una empresa local de cárnicos y abarrotes en Villavicencio (Meta), construido como entrega del **Taller Práctico de GitHub** de 2 horas.

> **URL pública (GitHub Pages):** se publicará al final del taller en `https://Rennier10.github.io/carnicos-abarrotes/`

## Objetivo del taller

Aplicar el flujo profesional de Git/GitHub para construir y publicar un sitio web real:

1. Crear un repositorio en GitHub.
2. Registrar cambios con commits descriptivos.
3. Trabajar con ramas y pull requests para cada sección.
4. Publicar el sitio con GitHub Pages.

## Estructura del proyecto

```
carnicos-abarrotes/
├── index.html         # Página principal (bienvenida y propuesta de valor)
├── productos.html     # Catálogo de productos
├── contacto.html      # Información de contacto y formulario
├── galeria.html       # Galería de imagen corporativa
├── css/
│   └── styles.css     # Hoja de estilos principal
├── img/               # Imágenes (placeholders del taller)
└── README.md          # Este archivo
```

## Flujo de trabajo aplicado

| Sección | Rama | Pull request |
|---|---|---|
| Catálogo | `feature/catalogo` | PR fusionado a `main` |
| Contacto | `feature/contacto` | PR fusionado a `main` |
| Galería | `feature/galeria` | PR fusionado a `main` |

Cada sección se desarrolló en su propia rama, se subió al repositorio remoto y se integró a `main` mediante un pull request, simulando el trabajo colaborativo de tres equipos del taller.

## Comandos clave usados

```bash
# Configurar identidad (una sola vez)
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"

# Crear y moverse a una nueva rama
git checkout -b feature/catalogo

# Registrar cambios
git add .
git commit -m "Agrega sección catálogo de productos"
git push origin feature/catalogo

# Volver a main y traer los cambios fusionados
git checkout main
git pull origin main
```

## Cómo ver el sitio localmente

No requiere ningún servidor. Basta con abrir `index.html` en el navegador:

```bash
start index.html        # Windows
open index.html         # macOS
xdg-open index.html     # Linux
```

## Publicación con GitHub Pages

1. Entra al repositorio en GitHub.
2. Ve a **Settings → Pages**.
3. En **Source** elige `main` y la carpeta `/ (root)`.
4. Guarda y espera ~1 minuto a que GitHub genere la URL pública.

## Autor

- **Rennier Santiago Colmenares Sánchez** — Universidad Manuela Beltrán

## Licencia

Uso académico para el Taller Práctico de GitHub.
