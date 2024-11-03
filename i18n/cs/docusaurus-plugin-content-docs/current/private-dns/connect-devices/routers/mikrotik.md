---
title: MikroTik
sidebar_position: 6
---

Routery MikroTik využívají open source operační systém RouterOS, který poskytuje služby směrování, bezdrátových sítí a firewallu pro domácí a malé kancelářské sítě.

## Konfigurace DNS-over-HTTPS

1. Přístup k routeru MikroTik:
   - Otevřete webový prohlížeč a přejděte na IP adresu routeru (obvykle `192.168.88.1`)
   - Případně můžete použít Winbox pro připojení k routeru MikroTik
   - Zadejte uživatelské jméno a heslo správce
2. Import kořenového certifikátu:
   - Stáhněte si nejnovější balíček důvěryhodných kořenových certifikátů: [https://curl.se/docs/caextract.html](https://curl.se/docs/caextract.html)
   - Přejděte na _Soubory_. Klikněte na tlačítko _Nahrát_ a vyberte stažený balíček certifikátů cacert.pem
   - Přejděte na _Systém_ → _Certifikáty_ → _Import_
   - V poli _Název souboru_ vyberte nahraný soubor certifikátu
   - Klikněte na _Importovat_
3. Konfigurace DNS-over-HTTPS:
   - Přejděte na _IP_ → _DNS_
   - V části _Servery_ přidejte následující servery AdGuard DNS:
     - `94.140.14.49`
     - `94.140.14.59`
   - Nastavte _Allow Remote Requests_ na _Yes_ (to je pro fungování DoH zásadní)
   - Do pole _Použít server DoH_ zadejte adresu URL soukromého serveru AdGuard DNS: https://d.adguard-dns.com/dns-query/\*\*\*\*\*\*\*\`
   - Klikněte na _OK_
4. Vytvořte záznam statického DNS:
   - V _Nastavení DNS_ klikněte na  _Statický_
   - Klikněte na _Přidat nový_
   - Nastavte _Název_ na d.adguard-dns.com
   - Nastavte _Typ_ na A
   - Nastavte _Adresu_ na `94.140.14.49`
   - Nastavte _TTL_ na 1d 00:00:00
   - Zopakujte postup a vytvořte identickou položku, ale s _Adresou_ nastavenou na `94.140.14.59`
5. Zakázání služby Peer DNS u klienta DHCP:
   - Přejděte na _IP_ → _DHCP Client_
   - Dvakrát klikněte na klienta používaného pro připojení k internetu (obvykle na rozhraní WAN)
   - Zrušte zaškrtnutí políčka _Používat Peer DNS_
   - Klikněte na _OK_
6. Propojte svou IP.
7. Testování a ověřování:
   - Možná bude nutné restartovat router MikroTik, aby se všechny změny projevily
   - Vymažte mezipaměť DNS prohlížeče. Pomocí nástroje, jako je [https://www.dnsleaktest.com](https://www.dnsleaktest.com/), můžete zkontrolovat, zda jsou vaše požadavky DNS nyní směrovány skrze AdGuard

## Použijte panel správce routeru

Pokud váš router Keenetic nepodporuje konfiguraci DNS-over-HTTPS nebo DNS-over-TLS, použijte tyto pokyny:

1. Otevřete panel správce routeru. Lze k němu přistupovat skrze adresy `192.168.1.1` nebo `192.168.0.1`.
2. Zadejte uživatelské jméno správce (obvykle je to admin) a heslo routeru.
3. Otevřete _Webfig_ → _IP_ → _DNS_.
4. Vyberte možnost _Servery_ a zadejte jednu z následujících adres DNS serveru.
   - IPv4: `94.140.14.49` a `94.140.14.59`
   - IPv6: `2a10:50c0:0:0:0:0:ded:ff` a `2a10:50c0:0:0:0:0:dad:ff`
5. Uložte nastavení.
6. Propojte svou IP adresu (nebo vyhrazenou IP adresu, pokud máte předplatné Team).

- [Vyhrazené IP adresy](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [Propojené IP adresy](/private-dns/connect-devices/other-options/linked-ip.md)