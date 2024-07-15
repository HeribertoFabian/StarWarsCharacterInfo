# StarWars Character API

## Descripción del Proyecto

El proyecto **StarWars Character API** es una aplicación basada en MuleSoft que permite recuperar información de personajes del universo de StarWars desde la SWAPI (Star Wars API) y exportarlos en formato CSV. Esta aplicación proporciona una interfaz de API REST para recuperar todos los personajes o filtrarlos por género.

## Funcionalidades

1. **Recuperar Todos los Personajes**:
   - Endpoint: `/api/v1/characters`
   - Método: `GET`
   - Descripción: Recupera la información de todos los personajes de StarWars y la exporta en formato CSV.

2. **Filtrar Personajes por Género**:
   - Endpoint: `/api/v1/characters?gender={gender}`
   - Método: `GET`
   - Descripción: Recupera la información de los personajes de StarWars filtrados por género (Male, Female, unknown, n/a) y la exporta en formato CSV.
   - Parámetro de Consulta:
     - `gender`: El género de los personajes a filtrar. Los valores permitidos son `Male`, `Female`, `unknown`, y `n/a`.

## Estructura del Proyecto

El proyecto se estructura en varios archivos de configuración y flujos de MuleSoft:

1. **starwars-characters-api-main.xml**:
   - Contiene la configuración principal del proyecto y los flujos principales para manejar las solicitudes de la API.

2. **console-flow.xml**:
   - Contiene el flujo para la consola de APIkit, que proporciona una interfaz interactiva para probar la API.

3. **RAML (starwars-characters-api.raml)**:
   - Define la especificación de la API, incluyendo los endpoints, métodos, parámetros y respuestas esperadas.

4. **Ejemplos (samples/)**:
   - Contiene ejemplos de respuestas en formato JSON y CSV para facilitar la documentación y las pruebas.

5. **Bateria de pruebas (postman/)**
   - El proyecto incluye archivos postman para realizar las pruebas en caso que no se quiera usar la consola

