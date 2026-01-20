# Technical Lab – LabSec Solutions

Tento repozitář dokumentuje testovací lab pro ověření základní
síťové a bezpečnostní konfigurace mezi virtuálními stroji
v interní síti LAN1. Cílem je vytvořit portfolio-ready dokumentaci
pro technické znalosti v oblasti IT a GRC.

## Použité systémy
- Ubuntu Server
- Ubuntu Desktop
- Windows 11 (host)
- Interní síť: LAN1 (VirtualBox Internal Network)
- Nástroje: SSH, SCP, Apache2, UFW, Wireshark

## Obsah repozitáře

| Soubor | Popis |
|--------|-------|
| `network_setup.md` | Základní konfigurace sítě a test ping |
| `ssh_tests.md` | Test SSH přihlášení mezi Desktopem a Serverem |
| `file_transfer.md` | Přenos souborů pomocí SCP |
| `web_server.md` | Test dostupnosti Apache web serveru |
| `firewall.md` | Kontrola stavu firewallu (UFW) |
| `wireshark.md` | Zachycení ICMP provozu pomocí Wireshark |
| `Screenshots/` | Snímky obrazovky dokazující jednotlivé testy |

## Struktura labu
- Ubuntu Server: 2 GB RAM, IP 192.168.100.10
- Ubuntu Desktop: 4 GB RAM, IP 192.168.100.20
- Windows 11: host, používá NAT a bridged adaptér pro internet
- Interní síť LAN1 propojuje VM pro testování komunikace

## Cíl
- Ověřit základní síťovou konektivitu
- Testovat vzdálený přístup a přenos souborů
- Kontrolovat stav firewallu
- Zachytit síťový provoz pro diagnostiku
- Vytvořit dokumentaci vhodnou pro portfolio a GRC

## Jak používat repozitář
1. Otevřít jednotlivé `.md` soubory pro detailní popis testů.  
2. Snímky obrazovky jsou umístěny ve složce `Screenshots/`.  
3. Každý test obsahuje:
   - Použitý příkaz
   - Výsledek
   - Důkaz (screenshot)
   - Závěr

---

