# Technical Lab – LabSec Solutions

Tento repozitář slouží jako technická dokumentace k simulaci interní sítě LAN1. Projekt demonstruje schopnost konfigurace síťových služeb, zabezpečení koncových bodů a analýzy síťového provozu – klíčové kompetence pro role v IT Security a GRC.

## Topologie sítě
Prostředí je postaveno na platformě VirtualBox v izolovaném segmentu.

* **Ubuntu Server (192.168.100.10):** Hostitel služeb Apache2 a SSH.
* **Ubuntu Desktop (192.168.100.20):** Klientská stanice a monitorovací uzel.
* **Segment LAN1:** Interní virtuální síť (bez přístupu zvenčí).

---

## Dokumentace testů a konfigurací

Kliknutím na odkaz se dostanete k detailnímu popisu, použitým příkazům a screenshotům.

| Fáze projektu | Popis aktivity | Dokumentace |
| :--- | :--- | :--- |
| **Příprava sítě** | Konfigurace rozhraní a statických IP adres | [network_setup.md](./Technical-Lab/network_setup.md) |
| **Konektivita** | Ověření dostupnosti uzlů v rámci LAN1 | [network_tests.md](./Technical-Lab/network_tests.md) |
| **Vzdálený přístup** | Konfigurace SSH a testování spojení | [ssh_tests.md](./Technical-Lab/ssh_tests.md) |
| **Přenos dat** | Bezpečné kopírování souborů přes SCP | [file_transfer.md](./Technical-Lab/file_transfer.md) |
| **Služby** | Nasazení Apache2 a test HTTP protokolu | [web_server.md](./Technical-Lab/web_server.md) |
| **Bezpečnost** | Nastavení firewallu UFW a hardening portů | [firewall.md](./Technical-Lab/firewall.md) |
| **Analýza** | Monitoring provozu a zachycení paketů | [wireshark.md](./Technical-Lab/wireshark.md) |
| **Zabezpečení** | Hardening SSH přístupu a konfigurace firewallu UFW | [ssh_access.md](./Technical-Lab/ssh_access.md) |
| **Správa služeb** | Diagnostika a oprava konfigurace webového serveru Nginx | [nginx_configuration.md](./Technical-Lab/nginx_configuration.md) |


---

## Důkazní materiály
Snímky obrazovky prokazující úspěšné provedení testů naleznete v adresáři `/screenshots`. Odkazy na konkrétní screenshoty jsou také přímo v jednotlivých `.md` souborech.

---
*Tento lab slouží jako evidence technických dovedností pro účely profesního portfolia.*
