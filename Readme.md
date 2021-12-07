# **DevSesame Control User App**

El proyecto se ha realizado en arquitectura hexagonal y con test. No se ha realizado el 100% del coverage pero para no alargar más el desarollo.
Podeis ver que he utilizado 

    - Mockery 
    - Mother
    - Command/Handler
    - PhpUnit
    - Codesniffer para tener codificacion PSR12
    - Doctrine ORM
    - Test Unitarios/Integrales/Funcionals
    - Fixtures
    - Docker

# **Prerquisitos**
Hay que acceder a la carpeta de app y realizar desde la consola: https://github.com/jamancebo/app-dev-sesame.git
Cuando se levante docker hay que crear una bd igual que la que realiza docker pero con el nombre de dev_sesame_test para los test


**_URLS_**

**Obtener usuario**
`http://localhost:8080/v1/user/{{id}}`

**Obtener todos los usuario**
`http://localhost:8080/v1/user`

**Crear usuario**
`http://localhost:8080/v1/user/`

**Actualizar usuario**
`http://localhost:8080/v1/user/`

**Eliminar usuario**
`http://localhost:8080/v1/user/`

**Obtener workEntry**
`http://localhost:8080/v1/workentry/{{id}}`

**Obtener todos los workEntry**
`http://localhost:8080/v1/workentry`

**Crear workEntry**
`http://localhost:8080/v1/workentry/`

**Actualizar workEntry**
`http://localhost:8080/v1/workentry/`

**Eliminar workEntry**
`http://localhost:8080/v1/workentry/`

Ejemplo de estructura para guardar un usuario
[
"id" => "e775b66c-5096-11ec-bf63-0242ac130112",
"createdAt" => "28/11/2023 00:00:00",
"updatedAt" => "29/12/2021 00:00:00",
"deletedAt" => null,
"name" => "Eduardo",
"email" => "edu@ori.com"
];

Ejemplo de estructura para guardar un workEntry
[
"id" => "337fe6aa-078f-45ee-943b-0ec504191cd8",
"userId" => "e775b66c-5096-11ec-bf63-0242ac130112",
"createdAt" => "28/11/2023 00:00:00",
"updatedAt" => "29/12/2021 00:00:00",
"deletedAt" => null,
"startDate" => "29/11/2021 15:00:00",
"endDate" => "29/11/2021 20:00:00"
];

**La aplicación tiene un token de seguridad. Este token se debe utilizar como Barear en las llamadas api que se realicen** 

**eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJyb2wiOiJhZG1pbiIsImV4cCI6MTgwNjMwNjUyMH0.-wz9SQstNzcX1QdzppCWwRzYvAOjba5XrbeQuGe44Nc**

**Para los tests**

**eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJyb2wiOiJhZG1pbiIsImV4cCI6MTgwNjMwNjUyMH0.T0EnxMFv95p-n-HTUEmRDlHAJD7YUzXqZpc9YDP2824**
