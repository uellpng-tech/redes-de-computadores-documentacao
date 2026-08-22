# IP, Máscaras de rede e CIDR

## Máscara de Rede

A máscara de rede é um mêcanismo de organização das redes para a divisão de um endereço IP. A máscara de rede separa a rede e o host, isso possibilita com que o computador saiba quais dispositivos se encontram por perto na mesma rede local e quais se encontram em outro lugar, através da máscara de rede podemos descobrir quantas redes existem e quantos hosts existem apenas executando uma conta simples.

Através da conversão dos números 0 (octetos zeros) ou outros números (octetos mistos) ou o ultimo número para número binário podemos obter um resultado que será crucial para a construção da conta, através da quantidade de números 1 podemos descobrir quantas sub-redes existem e através da quantidade de números 0 podemos descobrir a quantidade de hosts:

`Máscara de rede = 255.255.255.224`

1. Para converter em número binário dividimos por 2 até o 254 (octeto misto) ser igual a 1 ou 0 pegando todos os restos da divisão;

`Número binário do ultimo número: 11100000`

2. Com o número binário contamos quantos 1 existem (no exemplo 3) e quantos 0 existem (no exemplo 5) e utilizamos ele como elevação para o número 2 (concluindo 2^3 e 2^5);

`Formula para descobrir o host = 2^5-2`<br>
`Formula para descobrir a sub-rede = 2^3`

3. Com as formulas em mãos basta resolvelas utilizando o número descoberto atráves da conversão binária e a junção de numeros 1 ou 0.

`Resultado de sub-redes = 8`
`Resultado de hosts = 30`

O menos dois só é utilizado quando queremos excluir a propria rede e o broadcast.

## CIDR

O CIDR é a abreviação de uma máscara de rede atráves da conversão da máscara para números binários. O CIDR foi criado para substituir o método de classes (A, B e C) ele utiliza o número de bits da conversão completa de uma máscara de rede para número binário, em resumo ele abrevia a máscara e adiciona ao IP o número de bits da máscara, assim tendo mais informações através do IP (192.168.10.0/27). A conta é bem simples:

`Máscara de rede = 255.255.255.224`

1. Pegando todos os números e dividindo cada octeto (os 255 e 224 separados por .) por 2 e pegando os restos temos o número binário completo da máscara de rede;

`Máscara de rede em binário = 11111111.11111111.11111111.11100000`

2. Para concluir a abreviação CIBR basta contar quantos números 1 existem.

`CIDR = /27`

Em resumo o CIDR para além de uma abreviação é um sistema que possibilita mais IPs diferente das classes que utilizavam IPs fixos, por exemplo uma empresa com 257 computadores deveria ter uma classe B que comporta 65.536 máquinas porque o sistema de classes era fixo, já o CIDR possibilita criar qualquer tamanho de rede que seja potência de 2.