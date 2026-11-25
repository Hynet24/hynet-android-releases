<p align="center">
  <img src="assets/hynet-blueprint.jpg" width="100%" alt="Hynet для Android и Android TV. Логотип Hydra на синем техническом чертеже">
</p>

# Hynet для Android и Android TV

Клиент на базе Xray для подключения к личным серверам по защищённым протоколам.

**[Скачать APK](https://github.com/Hynet24/hynet-android-releases/releases/latest)** · [Все релизы](https://github.com/Hynet24/hynet-android-releases/releases) · [Сайт Hynet](https://hynet.click)

## Быстрый старт

1. Откройте последний релиз и скачайте файл `Hynet-*.apk` из раздела **Assets**.
2. Откройте APK. Если Android попросит разрешить установку из этого источника, подтвердите её в системных настройках.
3. Откройте Hynet, нажмите **Добавить сервер** и импортируйте ссылку подписки или отдельный ключ.

В приложении новые версии доступны через **Настройки → Проверить обновления**.

## Возможности

- **Подписки и ключи.** Импорт по ссылке, из буфера обмена или через QR на устройствах с камерой.
- **Hydra.** Проверяет серверы внутри активной подписки и переключается на рабочий при сбое.
- **Маршрутизация.** Поддерживает правила подписки, настройку DNS и выбор приложений, трафик которых пойдёт через VPN.
- **Android TV.** Горизонтальная раскладка и управление пультом.

## Технические сведения

| Параметр | Значение |
| --- | --- |
| Система | Android 8.0+ (API 26), включая Android TV |
| Архитектуры | `arm64-v8a`, `armeabi-v7a`, `x86_64`, `x86` |
| Протоколы | VLESS¹, VLESS², VLESS³, VMess¹, VMess², Shadowsocks, Trojan, Hysteria² |
| Варианты подключения (зависят от конфигурации) | TLS, XHTTP, REALITY, XTLS, gRPC REALITY, `xtls-rprx-vision`, CDN |
| Автообновления | [Метаданные актуального релиза](https://github.com/Hynet24/hynet-android-releases/releases/latest/download/update.json) |
| Целостность APK | SHA-256 указан в `update.json` каждого опубликованного релиза |

В Windows вычислить SHA-256 скачанного файла можно в PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 .\Hynet-*.apk
```

Сверьте результат со значением `sha256` в `update.json` того же релиза.
