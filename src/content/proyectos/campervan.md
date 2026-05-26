---
titulo: "CamperVan Co."
descripcion: "Landing corporativa de alquiler de furgonetas camper con catálogo, sistema de comentarios y panel de administración con roles."
imagen: "/campervan.png"
tecnologias:
  [
    "Next.js 16",
    "React",
    "Tailwind CSS",
    "PostgreSQL",
    "Prisma",
    "Auth.js",
    "Docker",
    "Vercel",
  ]
orden: 2
github: "https://github.com/edgarfpllefia/proyecto-mvc"
demo: "https://proyecto-mvc-orcin.vercel.app"
---

CamperVan Co. es una aplicación fullstack construida siguiendo el patrón MVC con Next.js 16 App Router. Incluye una landing pública con catálogo de modelos, sistema de comentarios para usuarios autenticados y un panel de administración protegido por roles.

El backend usa PostgreSQL con Prisma como ORM, levantado en local con Docker y desplegado en producción con Neon. La autenticación está implementada con Auth.js (NextAuth v5) y soporta tres roles: USER, EDITOR y ADMIN, cada uno con permisos distintos sobre el CRUD de modelos y la gestión de usuarios.
