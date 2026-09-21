# Rúbrica de evaluación de aspirantes — Posgrados

Página web para diligenciar la rúbrica de admisión de posgrados de la Facultad de Ciencias de la Salud. Calcula el puntaje en vivo y registra cada evaluación como una fila en Google Sheets.

## Cómo funciona

- `index.html` es la pantalla (se publica con GitHub Pages).
- El registro lo hace una aplicación web de Google Apps Script (`Code.gs`) que escribe en el Google Sheet. **`Code.gs` no se sube a este repositorio público**: vive en Apps Script.
- Para guardar, quien evalúa escribe una clave de acceso que solo conoce el equipo. La clave se guarda en las propiedades del proyecto de Apps Script, no en el código.

## Configuración

En `index.html`, pegar la URL de la aplicación web de Apps Script (termina en `/exec`) en:

```js
const API_URL = '';
```

Puntajes, niveles y rangos de decisión se editan en `Code.gs` (bloque `RUBRICA`); la pantalla se ajusta sola.

## Datos personales

Este repositorio no contiene datos de aspirantes. No compartir el Google Sheet públicamente.
