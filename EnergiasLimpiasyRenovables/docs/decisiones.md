# 📑 Registro de Decisiones - Proyecto Energías Limpias

## 👥 1. Ajuste de Equipo
Debido al retiro de una integrante, el equipo se reestructura a 2 personas. Para cumplir con el requisito de 4 secciones mínimas, la distribución es:

* **Integrante A (Líder):** Sección **Inicio** y **Nosotros**.
    * *Ramas:* `feature-inicio-nombreA` y `feature-nosotros-nombreA`.
* **Integrante B (Integrador):** Sección **Servicios** y **Productos**.
    * *Ramas:* `feature-servicios-nombreB` y `feature-productos-nombreB`.

## 📂 2. Estructura de Archivos (Fijada)
Se ha implementado una estructura modular para evitar conflictos de código:
* `/css/pages/`: Cada sección tiene su propio archivo `.css`.
* `/js/modules/`: Lógica separada por funcionalidades.
* `index.html`: Archivo base con secciones identificadas por ID.

## ⚙️ 3. Reglas de Git (Obligatorio para Calificación)
1. Prohibido trabajar directo en `main` o `DEV`.
2. Cada sección se desarrolla en su rama `feature-`.
3. El Integrador (Alumno B) es el único que realiza los Merges a `DEV` tras revisar el código.