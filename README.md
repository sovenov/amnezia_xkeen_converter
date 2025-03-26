Конвертация конфига Amnezia Xray (amnezia_for_xray.json) в VLESS URL и в Xkeen (04_outbounds.json)

Создано с помощью DeepSeek R1, с использованием "https://corvus-malus.github.io/XKeen-Config-Generator/".
Работает офлайн в браузере. Можно скачать и пользоваться локально.

Ссылка на index.html: https://sovenov.github.io/amnezia_xkeen_converter/

Также для "05_routing.json" есть генератор конфигов: https://xray-routing-generator.netlify.app/


<details>
<summary>Раскрыть пример конфига amnezia_for_xray.json для первого инпута</summary>
{
    "inbounds": [
        {
            "listen": "127.0.0.1",
            "port": 22869,
            "protocol": "socks",
            "settings": {
                "udp": true
            }
        }
    ],
    "log": {
        "loglevel": "error"
    },
    "outbounds": [
        {
            "protocol": "vless",
            "settings": {
                "vnext": [
                    {
                        "address": "115.42.69.228",
                        "port": 443,
                        "users": [
                            {
                                "encryption": "none",
                                "flow": "xtls-rprx-vision",
                                "id": "089e7783-2afc-4cd3-be3a-249ec7ebb499"
                            }
                        ]
                    }
                ]
            },
            "streamSettings": {
                "network": "tcp",
                "realitySettings": {
                    "fingerprint": "chrome",
                    "publicKey": "fgHqFBnFGHJFERTfzv_FfqERtq3qc_Dfqg42qA3qxHn",
                    "serverName": "www.vk.com",
                    "shortId": "523f456cf14c412e",
                    "spiderX": ""
                },
                "security": "reality"
            }
        }
    ]
}
</details>
