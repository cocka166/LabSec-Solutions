# Risk Assessment – LabSec Solutions

| Asset | Hrozby | Zranitelnosti | Riziko | Návrh mitigace |
|-------|--------|---------------|--------|----------------|
| Ubuntu Server – OS | Malware, neautorizovaný přístup | Chybějící aktualizace | High | Pravidelné aktualizace, minimální instalace, UFW |
| Ubuntu Server – síť | MITM, ARP spoofing | Nesprávné firewall pravidla | High | UFW povolit jen SSH, monitoring provozu Wiresharkem |
| Ubuntu Desktop – OS | Phishing, malware | GUI + nepotřebné služby | Medium | Minimalizovat služby, antivir, firewall |
| Windows 11 Host | Malware, ransomware | Uživatelský přístup | High | Antivirus, izolace VM, snapshots |
| LAN1 interní síť | Odposlech, neautorizovaný přístup | Chybějící segmentace | High | Pouze interní VM, NAT pro internet, Wireshark analýza |
| Konfigurační soubory | Změna, smazání | Nezálohované soubory | High | Zálohování, verzování, kontrola integrity |
| Log Files | Smazání, manipulace | Nepřehledné logy | Medium | Centralizace logů, pravidelné kontroly |
| Firewall Rules | Nesprávná konfigurace | Chybné pravidla | High | Testy, dokumentace, audit |
| Installed Packages | Zastaralé, nebezpečné balíčky | Chybějící aktualizace | Medium | Minimální instalace, pravidelné aktualizace |
| Backups | Chybějící | Žádné zálohy | High | Zálohovat konfigurační soubory a data, test restore |
