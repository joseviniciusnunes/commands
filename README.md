# Comandos úteis


## Ver todos erros do device
```bash
adb logcat -s '*:E'
```

## Ver todos erros do react native no device
```bash
adb -s emulator-5554 logcat -s ReactNative:V ReactNativeJS:V
```

## Abrir emulador sem deixar o terminal aberto
```bash
adb start-server
nohup ./emulator @device_name -no-snapshot-load &
```
## Criar banco de dados MySql-5.7 pelo docker
```bash
docker run --name mysql8 --restart=always -p 3306:3306 -v mysql8:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -d mysql:8
```
## Criar mongo
```bash
docker run -p 27017:27017 -v mongodbdata:/data/db --name=mongodb mongo:latest
```

## Criar banco de dados pelo docker
```bash
sudo docker exec ce92fce16244 mysql -u root -proot -e "CREATE SCHEMA teste ;"
```
## Executar comando sh alpine
```bash
docker exec -it [my-container-name] /bin/sh
```

## ver camadas da imagem
```bash
docker history --human --format "{{.CreatedBy}}: {{.Size}}" hello-word
```

