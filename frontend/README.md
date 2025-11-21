# SmartRetail IA – Frontend

Frontend oficial de **SmartRetail IA**, una plataforma SaaS orientada a pymes que permite predecir demanda, optimizar inventarios y visualizar métricas clave mediante inteligencia artificial.  
Esta aplicación web está desarrollada con **Next.js**, **TypeScript** y **TailwindCSS**.

---

### 🚀 Tecnologías utilizadas

-   **Next.js 16** – Framework React con SSR/ISR
-   **React 19**
-   **TypeScript**
-   **TailwindCSS** – Estilado rápido y responsive
-   **Fetch** – Comunicación con el backend
-   **Recharts** – Gráficos del dashboard
-   **Zustand** – Estado global
-   **Shadcn/UI** – Componentes UI reutilizables

---

### 🧭 Flujo de usuario (User Flow)

El siguiente esquema representa el recorrido típico de un usuario dentro de SmartRetail IA, desde el inicio de sesión hasta el uso de las principales funcionalidades del sistema.

#### 📝 Descripción del flujo

1. **Inicio de sesión**
   El usuario introduce sus credenciales; el sistema valida y genera una sesión.

2. **Dashboard**
   Se muestran métricas clave: ventas, historial, rotación y accesos rápidos.

3. **Gestión de productos**
   CRUD de productos, categorías y stock actual.

4. **Registro e importación de ventas**
   El usuario inserta ventas manualmente o importa un CSV.

5. **Predicciones de demanda**
   El sistema ejecuta el motor de IA y muestra previsiones futuras.

6. **Alertas inteligentes**
   El usuario recibe avisos sobre riesgo de rotura o exceso de stock.

7. **Exportación de informes**
   El usuario puede descargar información en PDF o CSV.

8. **Perfil de usuario / Roles**
   Configuración de cuenta, permisos y cierre de sesión.

---

### [🧪 Documentación de pruebas (QA posibles para el usuario)](QA_TESTING.md)

### ✅ Criterios de aceptación generales

-   La aplicación no debe mostrar errores inesperados durante las pruebas.
-   Las operaciones básicas (login, gestión de productos, registro de ventas y visualización de predicciones) deben completarse sin fallos.
-   Los mensajes de error deben ser claros cuando el usuario introduce datos incorrectos.
-   La interfaz debe ser usable tanto en escritorio como en dispositivos móviles (dentro del alcance del MVP).

---

## 📦 Instalación

Clona el repositorio y entra en el directorio:

```bash
git clone https://github.com/mcuamed570/SmartRetail.git
cd SmartRetail/frontend
npm install
npm run dev
```
