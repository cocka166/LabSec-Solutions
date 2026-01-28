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

| Fáze Labu | Popis aktivity | Dokumentace |
| :--- | :--- | :--- |
| **1. Network Setup** | Nastavení statických IP adres a rozhraní | [Protokol zde](./network_setup.md) |
| **2. Network Connectivity** | Testy dostupnosti a ICMP komunikace | [Protokol zde](./network_tests.md) |
| **3. SSH Access** | Konfigurace a ověření vzdálené správy | [Protokol zde](./ssh_tests.md) |
| **4. File Transfer** | Zabezpečený přenos dat mezi uzly (SCP) | [Protokol zde](./file_transfer.md) |
| **5. Web Server** | Nasazení Apache a kontrola HTTP provozu | [Protokol zde](./web_server.md) |
| **6. Firewall (UFW)** | Hardening serveru a definice pravidel | [Protokol zde](./firewall.md) |
| **7. Traffic Analysis** | Analýza paketů v reálném čase (Wireshark) | [Protokol zde](./wireshark.md) |

---

## 🛡️ GRC Compliance Checklist (Ukázka)
V rámci labu byly aplikovány tyto kontrolní mechanismy:
- [x] **Identifikace aktiv:** Definována statická IP schémata.
- [x] **Řízení přístupu:** SSH omezeno a testováno.
- [x] **Ochrana sítě:** Firewall (UFW) aktivován a nastaven na principu "Default Deny".
- [x] **Monitoring:** Protokolování síťových toků pomocí Wireshark.

## 📸Důkazní materiály
Snímky obrazovky prokazující úspěšné provedení testů naleznete v adresáři `/screenshots`. Odkazy na konkrétní screenshoty jsou také přímo v jednotlivých `.md` souborech.

---
*Tento lab slouží jako evidence technických dovedností pro účely profesního portfolia.*
