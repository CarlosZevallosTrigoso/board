# Notas

Tablero de notas estático. Dos archivos, sin backend.

## Estructura

- `index.html` — vista pública, lee y renderiza `messages.json`
- `messages.json` — array de mensajes, cada uno con `text` y `date`

## Publicar una nota

1. Abrir `messages.json` en github.com (ícono del lápiz)
2. Agregar un objeto al **inicio** del array:

```json
[
  {
    "text": "Tu mensaje aquí.",
    "date": "2026-03-13T15:30:00"
  },
  ...
]
```

3. Commit. GitHub Pages se actualiza en ~30 segundos.

## Formato de fecha

`YYYY-MM-DDTHH:MM:SS` en hora local. Ejemplo: `2026-03-13T15:30:00` = 13 de marzo de 2026, 3:30 p.m.

## Borrar todo

Reemplazar el contenido de `messages.json` con:

```json
[]
```

## Borrar una nota específica

Eliminar el objeto correspondiente del array. Cuidar que las comas entre objetos queden bien (sin coma después del último objeto).
