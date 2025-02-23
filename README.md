# Ecommerce Project

Este proyecto es una aplicación de ecommerce que permite a los usuarios explorar productos, agregarlos a un carrito de compras y realizar una compra simulada, donde los productos se restan de la base de datos. El proyecto está desarrollado utilizando tecnologías modernas para el desarrollo web full-stack.

## Tecnologías Utilizadas

- **Frontend**: 
  - React + Vite
  - TailwindCSS
  - Typescript
  - Javascript

- **Backend**: 
  - Express
  - Javascript

- **Base de Datos**: 
  - MongoDB (Mongo Compass)

## Características Principales

- **Catálogo de Productos**: Muestra una lista de productos disponibles con detalles como nombre, descripción, precio e imagen.
- **Carrito de Compras**: Permite a los usuarios agregar productos al carrito, ver el resumen de la compra y ajustar las cantidades.
- **Simulación de Compra**: Los usuarios pueden "comprar" los productos en el carrito, lo que reduce el stock de los productos en la base de datos.

## Estructura del Proyecto

```
ecommerce-project/
├── public/
│   ├── images/
│   ├── index.html
├── src/
│   ├── components/
│   │   ├── card-product/
│   │   ├── form/
│   │   ├── ItemsClothing/
│   │   ├── paginationControls/
│   │   ├── searchBar/
│   │   ├── stats/
│   │   └── table/
│   ├── context/
│   ├── contexts/
│   ├── hooks/
│   ├── layouts/
│   ├── pages/
│   ├── router/
│   ├── server/
│   ├── services/
│   ├── types/
│   └── utils/
├── package.json
├── tailwind.config.js
├── vite.config.ts
├── README.md
```

## Instalación y Configuración

### Requisitos Previos

- Node.js (v16 o superior)
- MongoDB Compass (o cualquier cliente de MongoDB)
- Git (opcional)

### Pasos para la Instalación

1. **Clonar el Repositorio**:
   ```bash
   git clone https://github.com/Vizrell/PF2.git
   cd ecommerce-project
   ```

2. **Instalar Dependencias**:
   ```bash
   npm install
   ```

3. **Configurar la Base de Datos**:
   - Abre MongoDB Compass y crea una nueva base de datos llamada `ecommerce`.
   - Crea los datos de productos a la colección `ProductSchema`.
   - Ejemplo de producto:
   {
  "_id": {
    "$oid": "67b91e0830cc40d8da545457"
  },
  "name": "Zapato Sporte",
  "price": {
    "$numberDecimal": "12.3"
  },
  "image": "/img",
  "stock": 10,
  "gender": "men",
  "type": "zapato"
    }

5. **Iniciar el Servidor Backend**:
   ```bash
   cd server
   node server.js
   ```

6. **Iniciar el Servidor Frontend**:
   ```bash
   npm run dev
   ```

7. **Acceder a la Aplicación**:
   - Abre tu navegador y visita `http://localhost:3000` para acceder a la aplicación.

## Uso de la Aplicación

1. **Explorar Productos**: Navega por la lista de productos disponibles en la página de inicio.
2. **Agregar al Carrito**: Haz clic en "Agregar al carrito" para añadir productos al carrito.
3. **Ver Carrito**: Accede al carrito desde el ícono en la esquina superior derecha.
4. **Realizar Compra**: En el carrito, haz clic en "Comprar" para simular la compra. Los productos se restarán del stock en la base de datos.

---

**Nota**: Este proyecto es una simulación y no está destinado a ser utilizado en un entorno de producción real.