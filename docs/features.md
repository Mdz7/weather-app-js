# Características y Endpoints

La aplicación procesa diferentes variables meteorológicas clave para renderizar la interfaz de usuario de forma dinámica.

## Parámetros de la API de Clima
A continuación se detallan los datos técnicos requeridos por nuestro módulo de JavaScript para procesar correctamente la respuesta del servidor de OpenWeather:

| Parámetro | Tipo | Descripción | Obligatorio |
| :--- | :--- | :--- | :--- |
| `q` | String | Nombre de la ciudad a consultar (ej. "San Salvador"). | Sí |
| `appid` | String | Token de autenticación personal (API Key). | Sí |
| `units` | String | Sistema métrico (`metric` para Celsius, `imperial` para Fahrenheit). | No |
| `lang` | String | Idioma de las descripciones climáticas (ej. `es`). | No |

!!! note "Consejo de Optimización de Rendimiento"
    Para mantener un rendimiento adecuado y evitar sobrecargar la cuota gratuita de la API, se recomienda almacenar temporalmente las consultas exitosas en el `localStorage` del navegador por un lapso de 10 minutos antes de permitir una nueva petición idéntica.

## Características Principales
- **Geolocalización Automática:** Consulta el clima local con un solo clic.
- **Persistencia de Datos:** Recuerda la última ciudad buscada entre sesiones.
- **Diseño Adaptable:** Interfaz optimizada mediante Flexbox y CSS Grid para dispositivos móviles y de escritorio.