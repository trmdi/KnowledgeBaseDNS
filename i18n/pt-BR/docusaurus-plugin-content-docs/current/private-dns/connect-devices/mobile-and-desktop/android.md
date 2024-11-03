---
title: Android
sidebar_position: 2
---

Para conectar um dispositivo Android ao AdGuard DNS, primeiro adicione-o à _Dashboard_:

1. Vá para o _painel_ e clique em _Conectar novo dispositivo_.
2. No menu suspenso _Tipo de dispositivo_, selecione Android.
3. Nomeie o dispositivo.
   ![Conectando dispositivo \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/choose_android.png)

## Usando o Bloqueador de anúncios AdGuard (opção paga)

O aplicativo AdGuard permite que você use DNS criptografado, tornando-o perfeito para configurações do AdGuard DNS em seu dispositivo Android. Você pode escolher entre vários protocolos de Criptografia. Junto com a filtragem DNS, você também tem um excelente Bloqueador de anúncios que funciona em todo o seu sistema.

1. Instale [o aplicativo](https://adguard.com/adguard-android/overview.html) no dispositivo que você quer conectar ao AdGuard DNS.
2. Abra o aplicativo.
3. Toque no ícone de escudo na barra de menu na parte inferior da tela.
   ![Ícone do escudo \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step3.png)
4. Toque em _Proteção de DNS_.
   ![Proteção de DNS \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step4.png)
5. Selecione _Servidor DNS_.
   ![Servidor DNS \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step5.png)
6. Role para baixo até _Servidores personalizados_ e toque em _Adicionar servidor DNS_.
   ![Adicionar servidor DNS \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step6.png)
7. Copie um dos seguintes endereços DNS e cole-o no campo _Endereço do servidor_ no aplicativo. Se você não tem certeza, opte por _DNS-over-HTTPS_.
   ![DoH \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step7_1.png)
   ![Servidor DNS personalizado \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step7_2.png)
8. Toque em _Adicionar_.
9. O servidor DNS que você adicionou aparecerá na parte inferior da lista de _Servidores personalizados_. Para selecioná-lo, toque em seu nome ou no botão de opção ao lado. Toque em _Salvar e selecionar_.
   ![Selecionar servidor DNS \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step_9.png)
10. Toque em Salvar e selecionar.
    ![Salvar e selecionar \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_ab/android_step10.png)

Feito! Seu dispositivo foi conectado com sucesso ao AdGuard DNS.

## Usando o AdGuard VPN

Nem todos os serviços de VPN suportam DNS criptografado. No entanto, nossa VPN é compatível, então, se você precisar tanto de uma VPN quanto de um DNS privado, AdGuard VPN é a sua melhor opção.

1. Instale [o aplicativo AdGuard VPN](https://adguard-vpn.com/android/overview.html) no dispositivo que você quer conectar ao AdGuard DNS.
2. Abra o aplicativo.
3. Na barra de menu na parte inferior da tela, toque no ícone de engrenagem.
   ![Ícone de engrenagem \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_vpn/android_step3.png)
4. Abra _Configurações do aplicativo_.
   ![Configurações do aplicativo \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_vpn/android_step4.png)
5. Selecione _Servidor DNS_.
   ![Servidor DNS \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_vpn/android_step5.png)
6. Role para baixo e toque em _Adicionar um servidor DNS personalizado_.
   ![Adicionar servidor DNS \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_vpn/android_step6.png)
7. Copie um dos seguintes endereços DNS e cole-o no campo _Endereço dos servidores DNS_ no aplicativo. Se você não tem certeza, opte por DNS-over-HTTPS.
   ![DoH \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_vpn/android_step7_1.png)
   ![Servidor DNS personalizado \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_vpn/android_step7_2.png)
8. Toque em Salvar e selecionar.
   ![Adicionar servidor DNS \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_vpn/android_step8.png)
9. O servidor DNS que você adicionou aparecerá na parte inferior da lista de _Servidores DNS personalizados_.

Feito! Seu dispositivo foi conectado com sucesso ao AdGuard DNS.

## Configure o DNS privado manualmente

Você pode configurar seu servidor DNS nas configurações do seu dispositivo. Por favor, note que os dispositivos Android suportam apenas o protocolo DNS-over-TLS.

1. Vá para _Configurações_ → _Wi-Fi e Internet_ (ou _Rede e Internet_, dependendo da versão do seu sistema operacional).
   ![Configurações \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_manual/manual_step1.png)
2. Selecione _Avançado_ e toque em _DNS privado_.
   ![DNS privado \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_manual/manual_step2.png)
3. Selecione a opção _hostname do provedor de DNS privado_ e insira o endereço do seu servidor pessoal: `{Your_Device_ID}.d.adguard-dns.com`.
4. Toque em _Salvar_.
   ![DNS privado \*mobile\_border](https://cdn.adtidy.org/content/kb/dns/private/new_dns/connect/android_manual/manual_step4.png)
   Tudo pronto! Seu dispositivo foi conectado com sucesso ao AdGuard DNS.

## Configurando DNS simples

Se você preferir não usar software extra para configuração de DNS, pode optar por DNS não criptografado. Você tem duas opções: usar IPs vinculados ou IPs dedicados.

- [IPs dedicados](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [IPs vinculados](/private-dns/connect-devices/other-options/linked-ip.md)