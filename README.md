# Portfolio — Edgar

Portfolio personal desarrollado con Astro 6, Tailwind CSS v4 y View Transitions. Diseño oscuro con estética de cuadrícula y tipografía Caveat para dar un toque artesanal.

---

## 🛠️ Stack

| Tecnología | Versión | Uso |
| :--- | :--- | :--- |
| [Astro](https://astro.build) | ^6.3.7 | Framework principal |
| [Tailwind CSS](https://tailwindcss.com) | ^4.3.0 | Estilos (vía plugin Vite) |
| [Lucide Astro](https://lucide.dev) | ^0.556.0 | Iconos |
| Node.js | >=22.12.0 | Entorno de ejecución |
| pnpm | — | Gestor de paquetes |

---

## 📁 Estructura del proyecto

```text
/
├── public/                   # Assets estáticos (favicon, imágenes públicas)
├── src/
│   ├── components/           # Componentes reutilizables (.astro)
│   ├── content/
│   │   └── proyectos/        # Colección de proyectos en Markdown
│   ├── layouts/
│   │   └── Layout.astro      # Layout base con fondo y fuentes
│   ├── pages/
│   │   ├── index.astro       # Página principal (Home)
│   │   └── proyectos/
│   │       └── [id].astro    # Página dinámica de cada proyecto
│   ├── styles/               # Estilos globales
│   └── content.config.ts     # Schema de la colección de proyectos
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

---

## ⚙️ Comandos

Ejecutar desde la raíz del proyecto:

| Comando | Acción |
| :--- | :--- |
| `pnpm install` | Instala las dependencias |
| `pnpm dev` | Servidor de desarrollo en `localhost:4321` |
| `pnpm build` | Build de producción en `./dist/` |
| `pnpm preview` | Preview del build antes de desplegar |

---

## 📄 Añadir un proyecto

Crea un archivo `.md` en `src/content/proyectos/` con el siguiente frontmatter:

```md
---
titulo: Nombre del proyecto
descripcion: Descripción corta
imagen: /imagenes/nombre.png
tecnologias:
  - Next.js
  - TypeScript
github: https://github.com/tu-usuario/repo
demo: https://tu-demo.com  # Opcional
---

Contenido largo del proyecto en Markdown...
```

Astro genera automáticamente la ruta `/proyectos/[id]` para cada archivo.

---

## ✨ Características

- **View Transitions** nativas de Astro para transiciones animadas entre páginas
- **Content Collections** con schema tipado via Zod
- **Diseño responsive** con Tailwind CSS v4
- Fuente [Caveat](https://fonts.google.com/specimen/Caveat) para títulos y elementos destacados
- Fondo oscuro con cuadrícula y color neón `#C7FF24`
