---
titulo: "Vinoteca"
descripcion: "Tienda online de vinos y cervezas con carrito de compra, gestión de pedidos por email, panel de administración con roles y subida de imágenes a Cloudinary."
imagen: "/vinoteca.png"
tecnologias:
  [
    "React",
    "Vite",
    "Tailwind CSS",
    "Node.js",
    "Express",
    "MongoDB",
    "Mongoose",
    "JWT",
    "Cloudinary",
    "Nodemailer",
    "Vercel",
  ]
orden: 3
github: "https://github.com/edgarfpllefia/frontend-vinoteca"
github_backend: "https://github.com/edgarfpllefia/api-express-vinos-cervezas"
---

Vinoteca es una aplicación fullstack de comercio electrónico para una tienda de vinos y cervezas. El frontend está construido con React + Vite y se comunica con una API REST propia hecha con Express y MongoDB Atlas.

Incluye autenticación con JWT, carrito de compra persistente, historial de pedidos y notificación por correo al realizar una compra. Las imágenes de productos y perfiles se gestionan con Cloudinary, lo que permite desplegar el backend en Render sin depender del sistema de archivos local.

El sistema de roles tiene tres niveles — usuario, editor y admin — con rutas protegidas tanto en frontend como en backend. Los editores pueden hacer CRUD de productos con subida de imágenes, y los admins gestionan usuarios y roles.
