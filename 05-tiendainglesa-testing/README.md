\# 🛒 Tienda Inglesa API Testing



\## 🎯 Objetivo

Explorar y probar endpoints reales de la web \*\*Tienda Inglesa\*\* utilizando \*\*Postman\*\* e \*\*Interceptor\*\*, validando su disponibilidad, formato y rendimiento.



---



\## 🧰 Herramientas

\- Postman (App de escritorio)  

\- Postman Interceptor (Extensión Chrome)  

\- Chrome DevTools  



---



\## 🔍 Actividades realizadas

1\. Identificación de endpoints reales a través de DevTools e Interceptor.  

2\. Captura automática de requests con Postman Interceptor.  

3\. Validación de estado (`200 OK`), tipo de respuesta (`application/json`) y tiempos de respuesta (< 800 ms).  

4\. Creación de tests automáticos en Postman (post-response scripts).  

5\. Documentación de casos de prueba y evidencias.



---



\## ⚙️ Notas técnicas

> Algunos endpoints del sitio usan el método \*\*POST\*\* para devolver información, cumpliendo la misma función que un `GET`.  

> No se requiere autenticación ni manipulación de datos del servidor.



---



\## 📂 Estructura del proyecto

05-Tienda-Inglesa-Api/

│

├── postman/

│ ├── 05-Tienda-Inglesa.postman\_collection.json

├── casos/

│ ├── testcases.xlsx

├── evidencias/

│ ├── Endpoints.png

│ ├── Interceptor debug session.png

│ ├── Test scripts.png

│ └── Postman interceptor.png

└── README.md



---



\## ✏️ Conclusión

Se identificaron y validaron correctamente endpoints reales del sitio \*\*Tienda Inglesa\*\*.  

El proyecto demuestra el uso de \*\*Postman Interceptor\*\* para capturar APIs sin documentación y la ejecución de \*\*tests automatizados\*\* para validar respuesta, formato y performance.



---





