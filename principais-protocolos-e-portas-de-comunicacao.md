# Principais protocolos de rede e portas de comunicação

## Portas de comunicação

As portas de comunicação são portas utilizadas para comunicação de dados sendo eles entrando ou saindo. As portas de comunicação seguem um conceito bem simples, cada porta tem sua função e númeração, elas servem para entrada e saida de dados possibilitando a manipulação do tráfego de dados através de multiplos programas, oque permite o tráfego simultaneo sem confundir suas comunicações. 

Existem várias portas de comunicação que seguem uma divisão. As portas vão de 0 até 65.535, elas seguem uma divisão bem simples, sendo as portas baixas (0 até 1023) que são as mais comuns usadas para  protocos e serviços e as portas altas (1024 até 65.535) que são portas destinadas as respostas aos clientes.

## Protocolos

Os protocolos são conjuntos de regras e padrões. Os protocolos são responsáveis de estabelecer a forma de como os dados se comportam, garantindo que a comunicação aconteça de forma correta, resumindo cada protocolo tem uma função específica, um bom exemplo é o HTTP que é responsável pela comunicação entre navegadores e servidores web. 

## Portas principais

Apesar de existir diversas portas algumas são mais utilizadas. As portas principais são as portas mais comuns e que são mais utilizadas, por tanto é necessário lembrar dessas portas:

- FTP 20/21: O FTP é um protocolo responsável por transferência de arquivos, a porta 20 é a de tranferência e a porta 21 é a porta de controle.

- SSH 22: O SSH é um protocolo que é responsável por dar acesso remoto ao terminal, possibilita acessar o terminal de uma máquina autorizada.

- TELNET 23: O TELNET é responsável pelo acesso remoto do terminal também, porém a diferência do SSH para o TELNET é que o SSH não tem criptografia, oque permite que qualquer pessoa com acesso a rede possa ver, já o TELNET tem criptografia.

- SMTP 25/587: O protocolo SMTP é responsável pelo envio e recebimento de E-mail, a porta 25 é responsável por envio de E-mail em servidores e a 587 é responsável pelo envio de e-mail por cliente, usando autenticação e criptografia.

- DNS 53: O DNS é responsável por traduzir domínio para IP ou IP para domínio, básicamente associa domínios aos seus IPs oque faz com que os dispositivos se comuniquem com os servidores.
 
- DHCP 67: O DHCP é um protocolo que distribui as configurações de IP, ele básicamente distribui todas as configurações para que o dispositivo tenha acesso a rede, ele da IP, mascara de rede, dns tudo que é necessário para utilizar a rede.

- TFTP 69: O TFTP é o protocolo de tranferência de arquivos simples, ele básicamente serve geralmente para trasnferir arquivos de configuração de equipamentos.

- FINGER 79: Protocolo de tranferência de informações dos usuários conectados a rede.

- HTTP 80: Protocolo de transferência de mídia, tudo que é mídia (foto, vídeo, áudio...) ele é responsável por tranferir.

- POP 110: O protocolo POP segue a mesma linha do SMTP, a diferência entre eles são que o POP baixa o E-mail e apaga do servidor e ele não envia E-mail.

- NTP 123: O protocolo NTP é responsável por sincronização de data e hora.

- IMAP 143: O protocolo IMAP é responsável por receber E-mails no servidor e sincronizar eles entre vários dispositivos.

- SNMP 161/162: O protocolo SNMP é responsável por gerenciar as conexões de rede.

- HTTPS 443: O HTTPS é a mesma coisa que o HTTP, porém com criptografia, possibilitando a segurança dos dados.