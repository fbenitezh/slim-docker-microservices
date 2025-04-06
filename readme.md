
# PHP Docker microservices

Estructura de proyecto para orquestar microservicios Slim 4 con docker




## Certificados SSL

Para generar Certificados ssl utilizamos la herramienta mkcert que se puede instalar de la siguiente manera

### Mac OS

```bash
brew install mkcert
brew install nss # si usás Firefox
mkcert -install
```

### Linux

```bash
sudo apt install libnss3-tools
curl -JLO "https://github.com/FiloSottile/mkcert/releases/latest/download/mkcert-v1.4.4-linux-amd64"
chmod +x mkcert-v*-linux-amd64
sudo mv mkcert-v*-linux-amd64 /usr/local/bin/mkcert
mkcert -install

```

### Windows
Descargá mkcert y corré mkcert -install desde CMD o PowerShell.


### Generacion de Certificados

```bash
mkdir certs
cd certs
mkcert service-a.localtest.me service-b.localtest.me
```