# Comandos úteis


## Ver todos erros do device
``bash
adb logcat -s '*:E'
``

## Ver todos erros do react native no device
``bash
adb -s emulator-5554 logcat -s ReactNative:V ReactNativeJS:V
``

## Abrir emulador sem deixar o terminal aberto
``bash
adb start-server
nohup ./emulator @device_name -no-snapshot-load &
``

## Criar banco de dados pelo docker
``bash
sudo docker exec ce92fce16244 mysql -u root -proot -e "CREATE SCHEMA teste ;"
``
## Executar comando sh alpine
``bash
docker exec -it srv-captain--api-perito.1.dwcp0907g7z2hcwnzbctn7een /bin/sh

