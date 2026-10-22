# Shopping Cart App

<div align="center">
  <img src="./src/assets/images/desktop-preview.webp" alt="Shopping Cart App Preview" width="600">
  <p>Una aplicación moderna de carrito de compras con React, TypeScript y Tailwind CSS</p>

  ![React](https://img.shields.io/badge/react-19.0.0-61DAFB)
  ![TypeScript](https://img.shields.io/badge/typescript-5.7.2-3178C6)
  ![Tailwind CSS](https://img.shields.io/badge/tailwind-4.0.15-38B2AC)
  ![Vite](https://img.shields.io/badge/vite-6.2.0-646CFF)
</div>

## Descripción
Shopping Cart App es una aplicación web que permite explorar un catálogo de productos, filtrarlos por categoría y gestionar un carrito de compras. Con una interfaz minimalista y responsiva, incluye modo claro/oscuro y un estado global manejado con Context API y reducers.

🔗 **Demo en vivo:** [shopping-cart-app-weld.vercel.app](https://shopping-cart-app-chi-drab.vercel.app/)

## Características
- 🛒 Gestión completa del carrito: añadir, eliminar, incrementar y decrementar productos
- 🔍 Filtrado de productos por categoría y otras propiedades
- 🌗 Tema claro/oscuro con soporte para las preferencias del sistema
- ⭐ Valoraciones de productos con estrellas
- 🎨 Interfaz moderna, responsiva y minimalista
- 🧩 Componentes reutilizables (Dropdown, StarRating, tarjetas y más)
- 📝 Código totalmente tipado con TypeScript

## Tecnologías Utilizadas
- ⚛️ **React 19** - Para la interfaz de usuario
- 📝 **TypeScript** - Para tipado estático y mejor mantenimiento del código
- 💅 **Tailwind CSS 4** - Para estilos modernos y responsivos
- 🔄 **Context API + useReducer** - Para la gestión del estado global
- ⚡ **Vite** - Para el desarrollo y empaquetado rápido
- 🎯 **React Icons** - Para los iconos de la interfaz

## Estructura del Proyecto
```
src/
├── assets/           # Imágenes y recursos estáticos
├── components/       # Componentes de React organizados por funcionalidad
│   ├── header/       # Header, Logo, CartButton, CartDrawer, ThemeButton
│   ├── main/         # Componentes principales
│   │   └── products/ # ProductList, ProductCard, ProducFilter
│   ├── footer/       # Componentes del pie de página
│   └── ui/           # Componentes reutilizables (Dropdown, StarRating)
├── context/          # Contextos de React
│   ├── cart/         # CartContext, CartProvider y useCart
│   └── filter/       # FilterContext, FilterProvider y useProductFilter
├── hooks/            # Custom hooks
│   └── useTheme.tsx  # Hook para gestionar el tema claro/oscuro
├── mocks/            # Datos de ejemplo (productsApiResults.json)
├── reducers/         # Reducers para gestión del estado
│   └── cartReducer.ts
├── types/            # Definiciones de tipos TypeScript
│   ├── cart.types.ts
│   └── types.ts
└── utils/            # Funciones utilitarias
    └── utils.ts
```

## Instalación y Uso
### 1️⃣ Clonar el repositorio
```bash
git clone https://github.com/IbrahimAlmeyda/shopping-cart-app.git
cd shopping-cart-app
```

### 2️⃣ Instalar dependencias
```bash
pnpm install
```
> 📝 **Nota**: El proyecto usa **pnpm** (`pnpm-lock.yaml`), pero también puedes usar `npm install`. Se requiere Node.js v18 o superior.

### 3️⃣ Ejecutar en desarrollo
```bash
pnpm dev
```
La aplicación estará disponible en `http://localhost:5173/`

### 4️⃣ Otros comandos
```bash
pnpm lint      # Revisa el código con ESLint
pnpm build     # Comprueba tipos y genera el build de producción
pnpm preview   # Sirve el build de producción localmente
```

## Guía de Uso
- **Añadir productos**: haz clic en "Añadir al carrito"; si el producto ya está, su cantidad se incrementa
- **Gestionar el carrito**: abre el icono del carrito, ajusta cantidades con "+" y "-", elimina productos con la papelera o vacía todo el carrito
- **Filtrar productos**: usa el dropdown de categorías para ver solo el tipo de producto que buscas
- **Cambiar el tema**: usa el botón de tema del encabezado para alternar entre modo claro y oscuro

## Buenas Prácticas Implementadas
- ✅ **Arquitectura modular** - Componentes y lógica organizados por funcionalidad
- ✅ **Context API + useReducer** - Estado global predecible para el carrito y los filtros
- ✅ **Custom hooks** - Separación de lógica de negocio y presentación
- ✅ **TypeScript** - Tipado estricto para prevenir errores en tiempo de desarrollo
- ✅ **Componentes reutilizables** - Props tipadas y diseño modular para facilitar el mantenimiento
- ✅ **Tema con variables CSS** - Modo oscuro implementado con variables de tema en `src/index.css`
- ✅ **Optimización de rendimiento** - Uso de memoización donde aporta valor

## Mejoras Futuras
- 💳 **Checkout** - Flujo de pago y resumen de compra
- 💾 **Persistencia del carrito** - Guardar el carrito en localStorage
- 🌐 **API real** - Reemplazar los datos mock por un backend
- 🔍 **Búsqueda de productos** - Búsqueda por texto además de los filtros
- 🧪 **Tests unitarios** - Implementación de pruebas para garantizar calidad
- 🌍 **Internacionalización** - Soporte para múltiples idiomas

## Licencia
Este proyecto está bajo la licencia MIT.

---

<div align="center">
  <p>Desarrollado con ❤️ por <a href="https://github.com/IbrahimAlmeyda">Ibrahim Almeyda</a></p>
</div>
