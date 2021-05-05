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
