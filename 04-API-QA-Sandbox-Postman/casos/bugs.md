## \[DummyJSON] Precio como string (simulado para portfolio)

**Severidad:** Media  

**Endpoint:** GET /products/1  

**Precondiciones:** Sin auth. Internet OK.  

**Pasos para reproducir:**

1. En Postman abrir "Get product by id (DummyJSON)" → Send.

2. Observar el campo `price` en el cuerpo de la respuesta.

**Esperado:** `price` sea numérico (number) y > 0.  

**Obtenido:** (Simulado) `price` viene como string `"109.95"`.  

**Evidencias:** `evidencias/respuesta\_ejemplo.txt`  

**Notas:** Caso creado a efectos demostrativos para el portfolio; en sistemas reales se reporta como inconsistencia de tipo de dato.




