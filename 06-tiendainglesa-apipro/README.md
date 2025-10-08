\# 🧪 Proyecto 06 – Tienda Inglesa API (Pro)



\## 🎯 Objetivo

Automatizar pruebas sobre endpoints reales de la web de Tienda Inglesa, validando comportamiento, estructura JSON y tiempos de respuesta.

Se utilizó Postman para el diseño de las pruebas y Newman para la ejecución automatizada con reporte.



\## ⚙️ Configuración

\*\*Variables de entorno\*\*

\- `baseUrl`: https://www.tiendainglesa.com.uy/supermercado/busqueda

\- `searchTerm`: huevos

\- `sort`: statprice+asc

\- `brand`: %5B%22Zaini%22%5D



\*\*Scripts\*\*

\- \*Pre-request Script\*: rota automáticamente el `searchTerm` y garantiza que `baseUrl` esté definido.

\- \*Tests (Post-response)\*: valida código 200, formato JSON y existencia de campos de producto.



\## 🧩 Estructura



```

├── /postman/

│ └── 06-Tienda-Inglesa-APIPro.postman\_collection.json

│ └── TiendaInglesa\_Pro.postman\_environment.json

│ └──/newman/

│ └──│ └── 06-Tienda-Inglesa-APIpro-2025-10-08-14-57-41-653-0.html

│

├── /casos/

│ └── testcases.xlsx

│

├── /evidencias/

│ ├── Envioronment.png

│ ├── Newman.png

│ ├── Post\_response.png

│ └── Postman\_console\_scripts.png

│ └── Postman\_interceptor.png

│

└── README.md

```





\## 🚀 Ejecución en Newman

newman run "06-Tienda-Inglesa-APIPro.postman\_collection.json" -e "TiendaInglesa\_Pro.postman\_environment.json" -r htmlextra





\## 📊 Resultados

* Todas las requests respondieron con código 200 y formato JSON válido.
* El endpoint principal /busqueda devolvió datos de productos reales.
* Se detectó que el framework GeneXus utiliza requests intermedias sin arrays visibles (documentado como hallazgo técnico).



\## 🧠 Aprendizajes



Identificación de endpoints dinámicos en un sitio real (GeneXus).



Diferenciación entre requests de inicialización y de datos.



Automatización de pruebas con Postman + Newman.



Generación de reportes automáticos HTML.











































