# Racker 2026 - Astro

Sitio corporativo moderno para **racker.cl**, pensado para reemplazar WordPress con una base más rápida, mantenible y lista para producción en el hosting actual.

## Stack
- Astro
- CSS custom moderno
- Sitio estático listo para build

## Cómo levantar en local
```bash
npm install
npm run dev
```

## Cómo compilar
```bash
npm run build
```

El resultado quedará en la carpeta `dist/`.

## Cómo subir al hosting actual
### Opción simple
1. Ejecuta `npm run build` en tu máquina.
2. Sube el contenido de `dist/` al directorio `public_html/` del hosting.
3. Configura el dominio para que apunte a ese contenido.
4. Mantén SSL activo desde DirectAdmin.

### Si quieres mantener formularios
El ejemplo usa `formsubmit.co` como placeholder. Debes cambiar:
```html
action="https://formsubmit.co/tu-correo@dominio.cl"
```

También puedes reemplazarlo por:
- un endpoint Node.js usando `Setup Node.js App`
- un servicio SMTP del hosting
- integración con API externa

## Qué debes reemplazar antes de producción
- Logo real de Racker
- Imágenes reales de proyectos y sistemas
- Texto comercial definitivo
- Email y teléfono finales
- Metadatos SEO por página
- Integración real del formulario

## Estructura
- `src/pages`: páginas del sitio
- `src/components`: cabecera, footer, hero y bloques reutilizables
- `src/styles/global.css`: estilos globales
- `src/data.ts`: contenido base del sitio
