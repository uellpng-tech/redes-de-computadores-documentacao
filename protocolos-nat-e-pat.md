# Protocolos: NAT e PAT

## NAT

O protocolo NAT (Network Address Translation) é um protocolo que traduz endereços IP privados em endereços IP públicos. O protocolo NAT serve como intermediário entre as redes LAN (Local Area Network) e a internet, assim atuando como um tradutor de rede local para internet. O objetivo para criração do protocolo NAT surge da necessidade de evitar que os IPs do mundo acabassem rápido, tendo em vista que o protocolo IPV4 (Internet Protocol Version 4,protocolo utilizado para identificação de dispositivos em uma rede) tem limite de cerca de 4,3 Bilhoẽs de endereços. Além do protocolo NAT traduzir ele também esconde os IPs reais dos computadores da rede LAN, dificultando ataques diretos da internet.

## PAT

O protocolo PAT (Port Address Translation) também conhecido como NAT overload, é uma evolução do NAT. Ele permite que vários dispositivos de uma rede LAN acessem a internet usando um único endereço IP público, o PAT é muito necessário por essa funcionalidade pois o NAT tradicional utiliza IPs públicos para cada computador, isso é caro pelo fato de que IPS públicos são caros e escassos, O PAT atuou resolucionando esse problema de forma genial utilizando portas de comunicação para criar canais exclusivos para cada aparelho dentro de um IP público.