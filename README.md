# Configuración remota de OmniNovel

La app lee este archivo como mucho cada 12 horas. Sirve para ser buen
ciudadano con las webs: si una web pide que se la deje de consultar, o que se
espacien las peticiones, se anota aquí y todas las instalaciones lo respetan
sin esperar a una actualización de la app.

Formato:

```json
{
  "version": 1,
  "sources": {
    "<id de la extensión>": {
      "pause": true,
      "message": "Texto que verá el lector (máx. 200 caracteres)",
      "novedades": false,
      "downloads": false,
      "minGapSeconds": 5
    }
  }
}
```

Todos los campos de cada fuente son opcionales. Sin entradas, no cambia nada.
