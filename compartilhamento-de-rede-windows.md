# Compartilhamento de Rede no Windows

## Renomeação de máquina

A renomeação da máquina nesse caso é muito importante por questões de organização. A mudança de nome do computador é importante para identificação do usuário dentro do compartilhamento, o Windows por padrão nomeia a máquina com "DESKTOP" e uma sequência alfanúmerica, isso dificulta a identificação quando a intenção é o compartilhamento de uma unidade. O processo de renomeação vária ligeiramente dependendo da versão do Windows, esse passo a passo serve para as versões atuais porém é pensada para o Windows 10, o processo é bem simples:

1. Abrimos o explorador de aquivos e com botão direito na aba "Este Computador" escolhemos a opção "Propriedades" ou podemos usar o atalho windows+pausebreak.

2. Na aba propriedades no canto inferior direito clicamos no link em destaque na cor azul "Alterar configurações".

3. Dentro da aba alterar configurações no canto direito inferior clicamos em "alterar".

4. Na aba do alterar escolhemos o nome sem caracteres especiais apenas letras, e em seguida confirmamos a alteração.

## Criação de grupos de trabalho (Workgroup)

No Windows o compartilhamento de rede funciona de diversas maneiras, porém a maneira usada nesse resumo funciona através de grupos oque melhora na facilidade de gerenciar permissões. Na criação dos grupos basta seguir um passo a passo bem simples e práticamente igual ao ultimo apresentado, como alertado o processo vária um pouco de acordo com a versão do Windows, esse processo é pensado para o Windows 10:

1. Abrimos o explorador de aquivos e com botão direito na aba "Este Computador" escolhemos a opção "Propriedades" ou podemos usar o atalho windows+pausebreak.

2. Na aba propriedades no canto inferior direito clicamos no link em destaque na cor azul "Alterar configurações".

3. Dentro da aba alterar configurações no canto direito inferior clicamos em "alterar".

4. Na aba do alterar na caixa "Membro de" colocamos o nome do grupo de trabalho, em seguida confirmamos a alteração.

Os grupos são criados dessa maneira, o seu computador vai enxergar apenas os computadores que participam do mesmo grupo escolhido anteriormente.

## Criação de unidade de compartilhamento na rede

Essa parte é opcional, pois para compartilhar algo na rede basta conceder o acesso ao grupo, porém é muito importante o particionamento por questões de organização. O particionamento funciona de uma maneira um pouco mais complicada, porém como o foco é a criação de uma partição de compartilhamento isso é bem simples, o particionamento isola uma parte do seu ssd ou hd oque possibilita separar uma parte para algo específico, isso delimita o acesso dos dados que estão em um particionamento para o outro, isso cria certa segurança e ajuda na organização. Para criação de uma partição existem várias formas porém no Windows na interface gráfica seguimos um simples passo a passo:

1. Com o botão direito clicamos na logo do Windows e escolhemos a opção de "Gerenciamento de discos".

2. Na aba gerenciamento de discos vemos as patições disponiveis nos seus discos e cada disco, dentro do disco desejado clicamos com o botão direito no disco local (C:) e escolhemos a opção "Diminuir Volume".

3. Dentro da aba diminuir volume escolhemos na terceira opção "Digite o espaço a diminuir em MB" o tamanho da unidade de compartilhamento em MB, na primeira opção está indicando o tamanho total antes da diminuição do disco, oque pode servir para a base da diminuição.

4. Depois de escolher o tamanho basta cricar em diminuir para confirmar a mudança.

5. Na aba gerenciamento de discos aparecera o novo particionamento, clicamos com o botão direito e escolhemos a opção de "Novo Volume Simples" 

6. Dentro da aba novo volume simples vamos dar formato a partição, caso não a nenhum requisito especial basta avançar para confirmar a finalização da criação da unidade de compartilhamento.

Criando essa unidade podemos obter acesso a ela pela aba do explorador de arquivos "Este Computador".

> A criação de partições pode ser um risco muito grande para quem não tem expêriencia, é recomendado obter conhecimento previo em questão a esse tema ou seguir um tutorial para assim conseguir efetuas a criação de partições sem grandes problemas.

## Configurações de compartilhamento para arquivos e unidades de memoria

Para podermos compartilhar os arquivos ou a unidade no grupo é bem simples. O compartilhamento através dos grupos no Windows funciona concedendo acesso ao arquivo, pasta ou unidade desejada, a unidade de memoria criada anteriormente é um otimo exemplo para explicar como configuramos algo para compartilhar na rede, esse passo a passo serve para qualquer coisa que queira adicionar ao compartilhamento de rede. Para compartilhar uma unidade é bem simples:

1. No explorador de arquivos entramos na aba "Este Computador".

2. Dentro da aba este computador clicamos com o botão direito na unidade de memoria criada anteriormente e escolhemos a opção "Conceder acesso a".

3. Dentro dessa aba vamos na opção "Compartilhamento Avançado".

4. Dentro da opção compartilhamento avançado de inicio colocamos o nome do compartilhamento e o limite de números de usuários simultâneos.

5. Nessa mesma aba podemos ver um botão no lado esquero "Permissões", dentro dessas permissões podemos escolher quem tem acesso e quais permissões podem ter perante ao arquivo/unidade compartilhada.

6. Para finalizar a operação basta clicar em aplicar e fechar a aba.

Esse passo a passo serve para qualquer coisa que queira compartilhar na rede.

## Como acessar os compartilhamentos

Para acessar os compartilhamentos é bem simples. Para poder ter acesso aos compartilhamentos o seu computador tem que ter permissão de descoberta de rede, essa permissão possibilita com que possamos ver os outros computadores que estão precentes na rede, na configuração de alguns desses passos o windows vai pedir essa permissão, basta aceitala que você terá acesso aos computadores que estão no seu grupo através da aba "Rede" no explorador de arquivos. Com tudo pronto basta seguir o passo a passo para acessar os arquivos compartilhados:

1. No explorador de arquivos entramos na aba "Rede".

2. Na aba rede escolhemos o usuário que desejamos para acessar os arquivos compartilhados e com dois cliques entramos na aba de acesso.

3. Ao escolher o usuário na aba de acesso colocamos ou o e-mail e senha do usuário escolhido ou o usuário e senha do Windows dele, ambos dependem da configuração do usuário cujo o compartilhamento é o desejado.

4. Com a senha e o usuário podemos marcar na caixinha localizada no canto esquerdo se desejamos lembrar a senha, assim podemos ter acesso rápido ao compartilhamento do usuário.

5. Ao clicar em "ok"acessamos todos os arquivos compartilhados pelo usuário para o grupo.

