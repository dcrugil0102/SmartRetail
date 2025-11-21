## 🧪 Documentación de pruebas (QA posibles para el usuario)

En esta sección se describen pruebas funcionales que puede realizar un usuario final para validar el correcto funcionamiento de SmartRetail IA. Son pruebas manuales, pensadas para comprobar el comportamiento del sistema desde la interfaz web.

### 1. Pruebas de autenticación y acceso

**Caso de prueba 1 – Login correcto**

-   **Objetivo:** Verificar que un usuario con credenciales válidas puede acceder al sistema.
-   **Pasos:**
    1. Acceder a la URL de la aplicación.
    2. Introducir correo y contraseña válidos.
    3. Pulsar en “Iniciar sesión”.
-   **Resultado esperado:**  
    El sistema redirige al **dashboard** y muestra los datos principales del negocio.

**Caso de prueba 2 – Login incorrecto**

-   **Objetivo:** Verificar que el sistema gestiona credenciales erróneas.
-   **Pasos:**
    1. Introducir correo o contraseña incorrectos.
    2. Pulsar “Iniciar sesión”.
-   **Resultado esperado:**  
    Se muestra un mensaje de error y el usuario permanece en la pantalla de login.

---

### 2. Pruebas de gestión de productos

**Caso de prueba 3 – Crear un producto**

-   **Objetivo:** Comprobar que se puede registrar un nuevo producto en el inventario.
-   **Pasos:**
    1. Desde el dashboard, ir a “Productos”.
    2. Pulsar “Nuevo producto”.
    3. Rellenar nombre, categoría y stock inicial.
    4. Guardar.
-   **Resultado esperado:**  
    El nuevo producto aparece en el listado con los datos introducidos.

**Caso de prueba 4 – Editar un producto**

-   **Objetivo:** Verificar que se puede actualizar la información de un producto.
-   **Pasos:**
    1. En la lista de productos, seleccionar un producto existente.
    2. Pulsar “Editar”.
    3. Modificar, por ejemplo, el stock óptimo.
    4. Guardar.
-   **Resultado esperado:**  
    El producto se actualiza correctamente y los nuevos datos se muestran en la tabla.

**Caso de prueba 5 – Eliminar un producto**

-   **Objetivo:** Comprobar el borrado de productos.
-   **Pasos:**
    1. Seleccionar un producto de prueba.
    2. Pulsar “Eliminar” y confirmar.
-   **Resultado esperado:**  
    El producto deja de aparecer en el listado.

---

### 3. Pruebas de registro e importación de ventas

**Caso de prueba 6 – Registrar una venta manualmente**

-   **Objetivo:** Verificar que una venta puede registrarse desde la interfaz.
-   **Pasos:**
    1. Ir a la sección “Ventas”.
    2. Pulsar “Añadir venta”.
    3. Seleccionar producto, cantidad y fecha.
    4. Guardar.
-   **Resultado esperado:**  
    La venta aparece en el historial y se actualiza el stock del producto.

**Caso de prueba 7 – Importar ventas desde CSV**

-   **Objetivo:** Validar la carga de datos de ventas mediante archivo CSV.
-   **Pasos:**
    1. Acceder a “Ventas” → “Importar CSV”.
    2. Seleccionar un archivo CSV con formato válido.
    3. Confirmar la importación.
-   **Resultado esperado:**  
    Las ventas del archivo se incorporan al sistema y se reflejan en el dashboard.

---

### 4. Pruebas de predicción y dashboard

**Caso de prueba 8 – Visualizar predicciones**

-   **Objetivo:** Comprobar que el usuario puede ver las predicciones de demanda.
-   **Pasos:**
    1. Desde el dashboard, acceder al módulo de predicciones.
    2. Seleccionar un producto con datos de ventas.
    3. Solicitar predicción.
-   **Resultado esperado:**  
    Se muestran gráficos y valores previstos para el periodo seleccionado (semanal o mensual).

**Caso de prueba 9 – Actualización del dashboard**

-   **Objetivo:** Verificar que el dashboard refleja cambios tras nuevas ventas.
-   **Pasos:**
    1. Anotar las cifras actuales del dashboard (ventas, stock, etc.).
    2. Registrar nuevas ventas de un producto.
    3. Volver al dashboard o recargar la página.
-   **Resultado esperado:**  
    Las métricas y gráficos se actualizan con los datos nuevos.

---

### 5. Pruebas de alertas de stock

**Caso de prueba 10 – Alerta por stock bajo**

-   **Objetivo:** Comprobar la aparición de alertas cuando el stock baja del mínimo.
-   **Pasos:**
    1. Establecer un stock óptimo para un producto.
    2. Registrar ventas hasta que el stock actual sea inferior al stock óptimo.
    3. Ir al dashboard o sección de alertas.
-   **Resultado esperado:**  
    El sistema muestra una alerta indicando riesgo de rotura de stock para ese producto.

---

### 6. Pruebas de exportación y cuenta de usuario

**Caso de prueba 11 – Exportar informe**

-   **Objetivo:** Validar que se puede generar un informe para análisis externo.
-   **Pasos:**
    1. Ir a la sección de informes o dashboard.
    2. Pulsar “Exportar” (PDF o CSV).
-   **Resultado esperado:**  
    Se descarga un archivo con los datos de ventas, inventario o predicciones.

**Caso de prueba 12 – Cerrar sesión**

-   **Objetivo:** Verificar que la sesión puede cerrarse correctamente.
-   **Pasos:**
    1. Abrir el menú de usuario.
    2. Pulsar “Cerrar sesión”.
-   **Resultado esperado:**  
    El sistema cierra la sesión y redirige a la pantalla de login.
