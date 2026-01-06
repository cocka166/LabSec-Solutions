# Network Setup – LabSec Solutions

Tento dokument popisuje základní síťovou konfiguraci lab prostředí
a ověření konektivity mezi virtuálními stroji.

**Použité systémy:**
- Ubuntu Server
- Ubuntu Desktop
- Interní síť: LAN1 (VirtualBox Internal Network)

---

## Ověření síťové konektivity (Ping)

Cílem je ověřit, že Ubuntu Desktop a Ubuntu Server spolu komunikují
v interní síti LAN1.

### Použitý příkaz (Ubuntu Desktop):

bash
ping 192.168.100.10
Výsledek
Ping byl úspěšný, což potvrzuje:

funkční interní síť LAN1

správně nastavené IP adresy

žádné blokování ICMP provozu

![Ping test](../Screenshots/ping_server.png)

Závěr
Základní síťová konektivita mezi virtuálními stroji v labu je funkční
