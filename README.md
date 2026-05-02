# La Despensa del Llano

Sitio web de **La Despensa del Llano S.A.S**, empresa local de cárnicos y abarrotes ubicada en Villavicencio (Meta). El sitio presenta la propuesta de valor de la empresa, su catálogo, información de contacto y galería de imagen corporativa.

🌐 **Sitio publicado:** <https://rennier10.github.io/carnicos-abarrotes/>  
📦 **Repositorio:** <https://github.com/Rennier10/carnicos-abarrotes>

---

## Páginas del sitio

| Página | Archivo | Descripción |
|---|---|---|
| Inicio | [`index.html`](index.html) | Bienvenida, propuesta de valor y razones para elegir la marca. |
| Productos | [`productos.html`](productos.html) | Catálogo de cárnicos (res, cerdo, pollo, tocineta) y abarrotes (arroz, fríjol, aceite, huevos) con precios. |
| Galería | [`galeria.html`](galeria.html) | Galería de imagen corporativa: local, equipo, productores aliados, logística. |
| Contacto | [`contacto.html`](contacto.html) | Dirección, teléfonos, correo, horario y formulario de contacto. |

## Estructura del proyecto

```
carnicos-abarrotes/
├── index.html         # Página principal
├── productos.html     # Catálogo
├── contacto.html      # Contacto
├── galeria.html       # Galería corporativa
├── css/
│   └── styles.css     # Hoja de estilos común a todas las páginas
├── img/               # Imágenes
└── README.md
```

## Tecnologías

- **HTML5 semántico** con `<html lang="es-CO">` y `<meta charset="utf-8">`.
- **CSS3** sin frameworks: variables CSS, Grid y Flexbox para el layout responsive.
- Diseño adaptable a escritorio, tableta y móvil.

## Cómo ver el sitio

### En línea
Abre <https://rennier10.github.io/carnicos-abarrotes/> en cualquier navegador.

### Localmente
Clona el repositorio y abre `index.html` directamente:

```bash
git clone https://github.com/Rennier10/carnicos-abarrotes.git
cd carnicos-abarrotes
start index.html        # Windows
# open index.html       # macOS
# xdg-open index.html   # Linux
```

No requiere servidor ni dependencias.

## Proceso de desarrollo

El sitio se construyó siguiendo un flujo profesional de **ramas + pull requests**, con una sección por rama:

| Sección | Rama | Pull request |
|---|---|---|
| Catálogo de productos | `feature/catalogo` | [#1 fusionado](https://github.com/Rennier10/carnicos-abarrotes/pull/1) |
| Página de contacto | `feature/contacto` | [#2 fusionado](https://github.com/Rennier10/carnicos-abarrotes/pull/2) |
| Galería corporativa | `feature/galeria` | [#3 fusionado](https://github.com/Rennier10/carnicos-abarrotes/pull/3) |

Cada rama se desarrolló por separado, se subió al remoto y se integró a `main` mediante un pull request, manteniendo `main` siempre publicable.

### Pasos resumidos

```bash
# 1. Configurar identidad (una sola vez)
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"

# 2. Clonar el proyecto
git clone https://github.com/Rennier10/carnicos-abarrotes.git
cd carnicos-abarrotes

# 3. Crear una rama para tu cambio
git checkout -b feature/nueva-seccion

# 4. Editar archivos, registrar y subir cambios
git add .
git commit -m "feat: descripción del cambio"
git push origin feature/nueva-seccion

# 5. Abrir un Pull Request en GitHub y, tras revisión, hacer merge a main
```

## Publicación

El sitio se publica automáticamente con **GitHub Pages** desde la rama `main` (carpeta raíz). Cada `push` a `main` actualiza el sitio en menos de un minuto.

Para activarlo (si se clona el repo en otra cuenta):
1. Entrar a **Settings → Pages**.
2. En **Source** elegir `main` y la carpeta `/ (root)`.
3. Guardar y esperar a que GitHub genere la URL pública.

## Autor

**Rennier Santiago Colmenares Sánchez** · <renniersantiago03@gmail.com>
