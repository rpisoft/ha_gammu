# Home Assistant – Gammu SMS sender (Add-on)
![Home Assistant](https://img.shields.io/badge/-Home%20Assistant-41BDF5?style=flat&logo=homeassistant&logoColor=white)
![Gammu](https://img.shields.io/badge/Gammu-000000?style=flat&logo=)
![AI](https://img.shields.io/badge/AI-0078D7?style=flat&logo=artificial-intelligence&logoColor=white)

This repository contains the Home Assistant add-on **GAMMU text SMS**, was created with the help of AI to complement the excellent Home Assistant software, making smart homes easier and more enjoyable for everyone.

## Usage
1. Go to Settings → Add-ons → Add-on Store → Repositories.
2. Add the repository URL: https://github.com/rpisoft/ha_gammu
3. Open the add-on configuration and save your device
   
``` bash
   /dev/ttyUSB0 e.g. /dev/serial/by-id/usb-HUAWEI_MOBILE_HUAWEI_MOBILE-if00-port0
```
4. Start the add-on.
5. Add to configuration.yaml
```yaml
rest_command:
  send_sms:
    url: "http://localhost:5000/send_sms"
    method: POST
    content_type: "application/json"
    payload: '{"number": "{{ number }}", "message": "{{ message }}"}'
```

### Supported Architectures
![aarch64](https://img.shields.io/badge/arch-aarch64-purple)  ![amd64](https://img.shields.io/badge/arch-amd64-blue)  ![armv7](https://img.shields.io/badge/arch-armv7-green)  

### License
MIT

---
My Other Projects
---
- [HA Openvpn client](https://github.com/rpisoft/ha_openvpn)
