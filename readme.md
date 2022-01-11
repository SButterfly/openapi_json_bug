How to reproduce:
1. clone `git clone `
2. cd openapi_json_bug
3. generate output file
```bash
docker run --rm -v "${PWD}:/local" openapitools/openapi-generator-cli:latest generate \
    -i /local/openapi/conf.yaml \
    -g openapi \
    -o /local/openapi_out
```
4. Open openapi_out/openapi.json
