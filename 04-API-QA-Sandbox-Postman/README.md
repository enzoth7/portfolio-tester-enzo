# API QA – Sandbox con Postman (Lite)

## 🎯 Objetivo
Practicar pruebas de API con Postman validando status, estructura y campos clave usando **DummyJSON**, **Postman Echo** y **JSONPlaceholder**.

## 🧰 Cómo ejecutar
1. Importar la **colección** y el **environment** (si los tenés).
2. Abrir cada request y presionar **Send**.
3. Ejecutar la carpeta **DummyJSON** con **Runner** para ver Passed/Failed.

## ✅ Alcance (requests principales)
- DummyJSON: `GET /products`, `GET /products/1`, `POST /products/add`, `PUT /products/1`, `GET /products/99999` (negativo)
- Postman Echo: `GET /get?color=red&size=42`
- JSONPlaceholder: `POST /posts`

## 🔎 Qué validé
- **Códigos**: 200/201/204 (éxito), 404 (negativo)
- **Estructura**: listas con `id`, `title`/`name`, `price`
- **Tests en Postman**: checks de status, lista no vacía, campos presentes

## 📁 Estructura
/postman/ (colección y environment)  
├─ API-QA-Collection.json  
├─ api-sandbox.postman_environment.json  
/casos/  
├─ test-cases.xlsx (TC-01 a TC-06)  
├─ bugs.md  
/evidencias/  
├─ runner_screenshot.png  
├─ tc-05_echo_get.png  
├─ tc-06_not_found.png  
└─ respuesta_ejemplo.txt

## 🧪 Casos de prueba (resumen)
- **TC-01** GET /products → 200, lista con ≥1 item, `id/title/price`
- **TC-02** GET /products/1 → 200, `id=1`, `title` string, `price` number > 0
- **TC-03** POST /products/add → 200/201, devuelve `id`, refleja campos
- **TC-04** PUT /products/1 → 200, `price` actualizado
- **TC-05** GET /get?color=red&size=42 → 200, `args` reflejan params
- **TC-06** GET /products/99999 → 404 (negativo)

## 🐞 Bugs (demo)
Ver `casos/bugs.md` (1 bug simulado con evidencia).

## ⚠️ Notas
APIs públicas de demo; datos pueden variar. Sin autenticación.













