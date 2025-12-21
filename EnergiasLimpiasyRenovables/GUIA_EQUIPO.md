# Guía de Trabajo en Equipo con Git 🚀

Esta guía es para ayudar al equipo a mover los cambios desde el desarrollo hasta producción de forma segura.

---

## 👩‍💻 Para la compañera de QA (Calidad)

Tu misión es probar los cambios que hizo **DEV** (rama `RH`) antes de que lleguen a todos.

### Paso 1: Traer los últimos cambios
Abre tu terminal en la carpeta del proyecto y ejecuta:

```bash
git fetch origin
```
*(Esto actualiza tu lista de ramas sin modificar tus archivos aún)*

### Paso 2: Cambiar a la rama de DEV
Para probar lo que hizo tu compañero, muévete a su rama:

```bash
git checkout RH
```
*(Si te da error, asegúrate de haber hecho el paso 1)*

### Paso 3: Probar
1.  Abre el archivo `index.html` en tu navegador (o usa `npx serve .` si tienes Node).
2.  Verifica que todo se vea bien y funcione.

### Paso 4: Aprobar
Si todo está bien, avisa al equipo: **"¡Rama RH aprobada!"**.
Si hay errores, avisa a DEV para que los arregle.

---

## 🚀 Para la compañera de PROD (Despliegue)

Tu misión es llevar los cambios aprobados de `RH` a la rama principal (`main`).

### Paso 1: Ir a la rama principal
Asegúrate de estar en `main`:

```bash
git checkout main
```

### Paso 2: Actualizar tu main
Por si acaso alguien más subió algo, actualízate primero:

```bash
git pull origin main
```

### Paso 3: Fusionar los cambios (Merge)
Ahora trae los cambios de la rama `RH` a `main`:

```bash
git merge RH
```
*(Esto mezclará el código. Si Git te pide un mensaje, solo guarda y cierra)*

### Paso 4: Subir a la nube
Finalmente, envía el `main` actualizado al repositorio remoto:

```bash
git push origin main
```

¡Listo! El proyecto está actualizado para todos. 🎉
