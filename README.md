# openapi-apitest

Test de description d'un webservice au format OpenAPI


## Génération de site web

Test de génération d'un siteweb à partir des spécification openapi en yaml.

### Avec redocly

```bash
docker run --rm -p 8080:80 \
  -e SPEC_URL=https://raw.githubusercontent.com/openapitools/openapi-generator/master/modules/openapi-generator/src/test/resources/2_0/petstore.yaml \
  redocly/redoc
```

### Avec swagger-ui

```bash
docker run --rm -p 8080:8080 \
  -e URL=https://raw.githubusercontent.com/openapitools/openapi-generator/master/modules/openapi-generator/src/test/resources/2_0/petstore.yaml \
  swaggerapi/swagger-ui
```
