# Comandos docker

## Browserless

> Comando docker para o uso do browserless em um servidor

```bash
docker run \
    -e "TOKEN=4D83A1B9A15FE8C3498F998E954DB" \
    -e "CONNECTION_TIMEOUT=-1" \
    -e "PREBOOT_CHROME=true" \
    -e "DEFAULT_IGNORE_HTTPS_ERRORS=true" \
    -p 3050:3000 \
    --restart always \
    -d --name browserless browserless/chrome:1-chrome-stable
```
