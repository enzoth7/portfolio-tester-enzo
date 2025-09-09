# Bugs identificados – Copay

## 1. Reserva de asiento bloqueada tras recargar la página

  - **Impacto**: Alto

  - **Precondición**: Seleccionar un asiento en el bus y recargar la página

  - **Pasos para reproducir**:

1. Ir al sitio de Copay y seleccionar un viaje (origen, destino, fecha ida y fecha vuelta)
  
2. Seleccionar un horario de salida.

3. Elegir un asiento y avanzar hacia la compra.

4. Antes de confirmar la compra, recargar la página.
   
5. Volver a hacer todos los pasos hasta la elección del asiento.
    
6. Buscar elegir el mismo asiento

 - **Resultado esperado**: El asiento debería liberarse automáticamente si el usuario no confirma la compra.

 - **Resultado actual**: El asiento queda marcado como reservado, obligando al usuario a elegir otro.

 - **Evidencia**: `screenshots/copay_inicio.png`, `screenshots/copay_horario.png`, `screenshots/copay_asiento.png`, `screenshots/copay_asiento_bug.png`

---

## 2. Sugerencias de mejora – Copay

1. Liberar automáticamente los asientos no confirmados si el usuario recarga la página o abandona el flujo de compra.

2. Implementar un temporizador visible (ejemplo: “tenés 5 minutos para confirmar tu reserva”) para que el usuario sepa cuánto tiempo tiene antes de que el asiento se libere.  




