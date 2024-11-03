---
title: PlayStation PS4/PS5
sidebar_position: 4
---

Herní konzole nepodporují šifrovaný DNS, ale jsou vhodné pro nastavení veřejného AdGuard DNS nebo soukromého AdGuard DNS prostřednictvím propojené IP adresy.

Je pravděpodobné, že váš router podporuje používání šifrovaných serverů DNS, takže na něm můžete kdykoli nakonfigurovat soukromý AdGuard DNS a připojit k němu herní konzoli.

[Jak nakonfigurovat router](/private-dns/connect-devices/routers/routers.md)

## Připojení k AdGuard DNS

Nakonfigurujte herní konzoli tak, aby používala veřejný server AdGuard DNS, nebo ji nakonfigurujte pomocí propojené IP adresy:

1. Zapněte konzoli PS4/PS5 a přihlaste se ke svému účtu.
2. Na domovské obrazovce vyberte ikonu ozubeného kola v horním řádku.
3. V nabídce _Nastavení_ vyberte _Síť_.
4. Vyberte _Nastavit připojení k Internetu_.
5. V závislosti na nastavení sítě vyberte možnost _Použít Wi-Fi_ nebo _Použít LAN_.
6. Vyberte možnost _Vlastní_ a poté vyberte možnost _Automatické nastavení IP adresy_.
7. Pro položku _Název hostitele DHCP_ vyberte možnost _Neurčovat_.
8. Pro _Nastavení DNS_ vyberte _Ručně_.
9. Do pole _DNS server_ zadejte jednu z následujících adres DNS serveru:
   - `94.140.14.49`
   - `94.140.14.59`
10. Pokračujte výběrem možnosti _Další_.
11. Na obrazovce _Nastavení MTU_ vyberte _Automaticky_.
12. Na obrazovce _Proxy server_ vyberte _Nepoužívat_.
13. Chcete-li otestovat nové nastavení DNS, vyberte možnost _Testovat připojení k Internetu_.
14. Jakmile je test dokončen a zobrazí se "Připojení k internetu: Úspěšné", uložte nastavení.

Bylo by vhodnější použít propojenou IP (nebo vyhrazenou IP, pokud máte předplatné Team):

- [Vyhrazené IP adresy](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [Propojené IP adresy](/private-dns/connect-devices/other-options/linked-ip.md)