# Sample Docker Image for ACR 
## Build
```bash
docker build . -t phpinfo
docker tag phpinfo mydreg-microsoft.azurecr.io/samples/phpinfo
```


## Login to ACR
```bash
docker login mydreg-microsoft.azurecr.io -u mydreg -p //O=AFs+5GwjHHUmP1Tg7Itn7+NubW3P
```


## Push to ACR
```bash
docker push mydreg-microsoft.azurecr.io/samples/phpinfo
```


## Pull from ACR
```bash
docker pull mydreg-microsoft.azurecr.io/samples/phpinfo
```


## Run Image
```bash
docker run -p 8080:80 mydreg-microsoft.azurecr.io/samples/phpinfo
```


Point your browser to http://localhost:8080
