# Bugs identificados – SauceDemo

1. Checkout con carrito vacío
   - Impacto: Alto
   - Precondición: Carrito vacío
   - Resultado actual: Compra procesada
   - Screenshot: `screenshots/checkout_empty.png`

2. Formulario acepta caracteres inválidos
   - Impacto: Medio
   - Precondición: Campos obligatorios
   - Resultado actual: Permite avanzar
   - Screenshots:
     - `screenshots/data_form_1.png`
     - `screenshots/data_form_2.png`
     - `screenshots/data_form_3.png`

3. Filtros
   - Impacto: Medio
   - Precondición: Usar un filtro
   - Resultado actual: Cambio de precios, productos y orden ilógico
   - Screenshots:
     - `screenshots/filter_1.png`
     - `screenshots/filter_2.png`
     - `screenshots/filter_3.png`
     - `screenshots/filter_4.png`

4. Productos
   - Impacto: Medio
   - Precondición: Seleccionar un producto
   - Resultado actual: No coinciden los precios del producto en el catálogo y en el detalle
   - Screenshots:
     - `screenshots/product_price_1.png`
     - `screenshots/product_price_2.png`


# Sugerencias de mejora – SauceDemo

1. Permitir seleccionar cantidad de productos en el carrito
   - Screenshot: `screenshots/qty.png`

2. Validar los campos del formulario para aceptar solo datos correctos

3. Mejorar la interfaz del carrito para mayor claridad visual e íconos alineados
   - Screenshot: `screenshots/UI.png`
