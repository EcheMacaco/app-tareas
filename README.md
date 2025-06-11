# App Tareas

Aplicación React para la gestión de tareas.

## Instalación

Ejecuta en la terminal:

```
npm install
```

## Ejecución en modo desarrollo

```
npm start
```

## Ejecutar pruebas (tests)

```
npm test
```

## Generar build de producción

```
npm run build
```

## Automatización de pruebas y publicación (CI/CD)

Este proyecto utiliza GitHub Actions para automatizar el proceso de pruebas y publicación en npm.

- El workflow se encuentra en `.github/workflows/publish.yaml`.
- Se ejecuta automáticamente al crear un nuevo release en GitHub.
- Primero instala dependencias y ejecuta los tests.
- Si los tests pasan y el release es en la rama `master`, publica el paquete en npm usando el token `npm_token` configurado en los secrets del repositorio.

Puedes personalizar el workflow editando el archivo mencionado.

---

Para más información, revisa los scripts en `package.json` y el archivo de workflow.