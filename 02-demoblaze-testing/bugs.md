# Bugs identificados – Demoblaze

## 1. Checkout permite avanzar con datos inválidos
- **Impacto**: Alto
- **Precondición**: Carrito con productos cargados
- **Resultado actual**: El checkout permite finalizar la compra con campos incompletos o inválidos
- **Resultado esperado**: El sistema debería validar los campos y no permitir avanzar sin información correcta
- **Evidencia**: `screenshots/checkout1.png`, `screenshots/checkout2.png`

---

## 2. Formulario de contacto acepta caracteres inválidos
- **Impacto**: Medio
- **Precondición**: Ingresar datos en los campos obligatorios (nombre, email, mensaje)
- **Resultado actual**: Se aceptan caracteres inválidos (ejemplo: símbolos en el campo email)
- **Resultado esperado**: Los campos deberían validar la información ingresada antes de enviarla
- **Evidencia**: `screenshots/contact.png`

---

## 3. Botones de paginación no funcionan correctamente
- **Impacto**: Medio
- **Precondición**: Intentar navegar entre páginas de productos
- **Resultado actual**: Los botones no cargan los productos o no responden como corresponde
- **Resultado esperado**: Deberían cargar los productos asociados a cada página
- **Evidencia**: `screenshots/buttons.png`

---

## 4. Video de inicio no funciona
- **Impacto**: Bajo
- **Precondición**: Ingresar a la página principal
- **Resultado actual**: El video no se reproduce
- **Resultado esperado**: El video debería cargarse y reproducirse automáticamente o al hacer clic
- **Evidencia**: `screenshots/video.png`

---

# Sugerencias de mejora – Demoblaze

1. Reemplazar la palabra **“Cart”** por un ícono de carrito para mayor claridad visual
   - Evidencia: `screenshots/cart.png`

2. Eliminar las **barras laterales** visibles en las imágenes de los productos
   - Evidencia: `screenshots/images.png`

3. Descartar o corregir la funcionalidad de **registrar usuario** (actualmente no funciona)
   - Evidencia: `screenshots/user.png`

4. Permitir seleccionar la **cantidad de productos** directamente desde el catálogo o carrito
   - Evidencia: `screenshots/productquantity.png`

5. Corregir el **slider de imágenes** en la página de inicio (no cambia correctamente)
   - Evidencia: `screenshots/images.png`
