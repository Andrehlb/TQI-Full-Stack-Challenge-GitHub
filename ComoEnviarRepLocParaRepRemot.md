​											**Repositório do Bootcamp TQI Full Stack, pela Dio.me**

![image](https://user-images.githubusercontent.com/100593932/178079208-c419c9e5-ee54-4853-b081-c17a54f4a494.png)

​	Como fazer a criação de um repositório próprio, referente às atividades desenvolvidas no Bootcamp TQI Full Stack pela Dio.me, como parte do desafio de projeto de criação, atualização e sincronização de repositório remoto com repositório local.

 

**Como fazer criação, atualização e sincronização de repositório remoto no GitHub com repositório local via GitBash?**

 

​	Para o bom desenvolvimento destas atividades, além de engajamento e vontade de aprender, faz-se a recomendação de que se tenha noções básicas de Git/GitHub, pelo curso da Dio.me que podem ser obtidas neste link: [Introdução ao Git e GitHub](https://web.dio.me/play)

​	Por que isto? Para facilitar o entendimento de que o Git é um sistema de controle de versão distribuído e o GitHub é um portal social e colaborativo, que serve ao versionamento de código, assim como forma de alocar arquivos em estado de commit ("commitados"), além de aprender sobre a instalação do Git e o uso do GitBash como terminal apropriado para executar os comandos adequados para "empurrar" ou fazer o "push" do repositório local (que está na máquina) para o GitHub ou vice-versa.

 

**Sumário deste projeto**

**1) Ter o Git devidamente instalado**

**2) Criar um novo repositório**

**3) Clonagem do repositório criado**

**4) Criar pasta no repositório local**

**5) Envio dos objetos no repositório local para o repositório remoto no GitHub**

**6) Empurrando objetos commitados para o repositório remoto do GitHub** 

 Etapas que devem ser seguidas para a criação de um repositório no GitHub:

 **1) Ter o Git devidamente instalado**

A instalação pode ser obtida pelo download, nos links disponibilizados a seguir, de acordo com o sistema operacional usado para as atividades de versionamento de código:

Downloads: [Windows](https://git-scm.com/download/win) | [macOS](https://git-scm.com/download/mac) | [Linux/Unix](https://git-scm.com/download/linux)

 **2) Criar um novo repositório**

 Na Figura 1 pode-se observar os locais indicados pelas setas para o procedimento de criação do repositório remoto diretamente no site do GitHub, neste link: [Create a New Repository (github.com)](https://github.com/new) 

![image](https://user-images.githubusercontent.com/100593932/178079320-303932a4-82c3-4927-84e8-cf73f20d9024.png)

**Figura 1. página do GitHub para a criação de um novo repositório, de cima para baixo, as setas indicam o nome a ser dado ao repositório, o status público (se assim for decidido) e a inserção de um arquivo README.**

**3) Clonagem do repositório criado**

 Após criar o repositório, ir na aba <>Code e do lado direito clicar em Code e copiar o link HTTPS (Figura 2). Na máquina, deve-se criar uma pasta 📂 para receber o conteúdo clonado do repositório remoto do GitHub. Nete caso foi criada a pasta 📂 TQI_Full_Stack_Challenge.

![image](https://user-images.githubusercontent.com/100593932/178079363-1f7c97fd-11da-4dcb-977a-46250c692c4d.png)

 **Figura 2. Aba <>Code, com o acesso ao link HTTPS a ser copiado para a clonagem a partir do repositório remoto para o local.**

 A clonagem tem por objetivo desenvolver a capacidade de gerenciar o repositório criado no GitHub e conectá-lo ao repositório local. Para ser feita a clonagem no repositório local (na máquina) usou-se o terminal GitBash. Para tal procedimento deve-se usar o comando:

`git clone <link HTTPS do repositório criado, copiado anteriormente>`

​	Após teclar [ENTER] o resultado será como observado na Figura 3. Pode-se observar o apontamento da clonagem ("Cloning into") e a porcentagem do total de objetos agora alocados no repositório local (Figura 3).

![image](https://user-images.githubusercontent.com/100593932/178079422-fafab1e6-d790-4bdb-997f-dd9138569d2e.png)

**Figura 3. Terminal GitBash com a execução de comando para clonagem de repositório e a mensagem do resultado deste procedimento.**

**4) Criar pasta no repositório local**

​	Após a clonagem, foi criada uma nova pasta interna à pasta do repositório que conterá um arquivo texto (*.txt ou *.md), e que seus significados são explicados no processo de noções básicas de Git/GitHub do curso introdutório mencionado anteriormente. Neste caso, o nome da pasta 📂 é TQI-Full-Stack-Challenge-GitHub.

​	Após criar uma nova pasta 📂, dentro da pasta do repositório local, a mesma é identificada pelo GitHub (Figura 4) como observado no destaque em vermelho feito pela IDE associada ao terminal GitBash. Na mensagem que o terminal disponibiliza é possível ja antever o próximo passo, o de usar o comando add para inclusão e posterior commitação do arquivo. Os comandos usados para identificação do conteúdo (diretório) e da situação do repositório local foram:

`git ls`
`git status`

![image](https://user-images.githubusercontent.com/100593932/178079445-fd547897-18f9-40ad-979d-f4630d76eb68.png)

**Figura 4. Estado "untracked" identificado para o arquivo, na pasta criada no repositório local.**

**5) Envio dos objetos do repositório local para o repositório remoto no GitHub**

​	O envio de objetos (arquivos, pastas, imagens), que estão no repositório local para o remoto no GitHub é sistemático. Primeiro, foi feito o envio para o controle de versionamento, ainda no repositório local, usando-se o comando add (Figura 5). Neste caso usou-se o comando de forma que enviasse todo o conteúdo de uma só vez, portanto o comando usado foi:

`git add .`

​	Outros comandos add com a mesma função poderiam ser usados, como: git add -A ou git add * ou git add **. A mensagem que aparece no terminal (Figura 5) é referente a quebra de linha, não interferindo no procedimento.

![image](https://user-images.githubusercontent.com/100593932/178079471-6a0f836e-1221-4de9-b691-c23de89214e8.png)

**Figura 5. Uso do comando add.**

  O procedimento feito acima (Figura 5) somente adicionou o objeto, no caso o arquivo, no repositório local, como pode ser observado pelo status do arquivo de extensão *.md (Figura 6), aonde o terminal retorna com a informação de que o arquivo, saiu da condição "untracked" (Figura 4) para situação stage (Figura 6) e que está pronto para ser commitado, o que significa dizer que o arquivo está pronto para ser transferido para o repositório remoto.

![image](https://user-images.githubusercontent.com/100593932/178079499-c1cea23d-c418-430e-8bd8-404157b5de0f.png)

**Figura 6. Status stage do arquivo criado, pronto para ser commitado (estado commit).**

​	Nesta próxima etapa será feito o "commit" do arquivo *.md e o seu envio do repositório local para o repositório remoto no GitHub. Por que e de que modo tem que "commitar"?

​	Primeiro se faz o commit para tirar o arquivo do estado stage e torná-lo apto para ser versionado no repositório remoto, para depois ser feito todo este ciclo novamente, para deixá-lo no formato adequado para novo versionamento. Para realizar o "commit", no GitBash usa-se o comando com mensagem entre aspas:

`git commit -m "[inserir menagem referente ao que será feito com o objeto de envio]"`

​	Após o "commit" do arquivo, pode-se observar que a main e o sha do arquivo (ver processo sha em introdução ao Git e GitHub) no repositório local foi criado e a quantidade de itens é apresentada (Figura 7). Uma verificação do status é feita pelo comando git status, que mostra que não há mais objetos em situação "untracked" ou "stage", mas agora em estado "commit"'. Também é possível observar que o terminal do Gitbash mostra a mensagem da próxima etapa, empurrar tudo que foi "commitado" para o repositório remoto, usando-se o comando push (Figura 7).

![image](https://user-images.githubusercontent.com/100593932/178079513-2044c5f5-ab2f-4435-9ec4-b5d939c13c64.png)

**Figura 7. Uso do comando commit e o Status dos objetos no repositório local.**

**6) Empurrando objetos commitados para o repositório remoto do GitHub** 


 Então, foi feito um commit local e agora será feito um push para empurrar os objetos para o repositório remoto no GitHub. O comando usado foi:

`git push origin main`

 Neste caso origin é uma convenção e main se refere ao status do local no repositório que pode variar, para master, por exemplo, este assunto é abordado no curso introdutório ao Git e GitHub da Dio.me mencionado anteriormente. O resultado observado no terminal do GitBash é a porcentagem de conversão do número total de objetos e o apontamento para o local HTTPS que estará os objetos commitados (Figura 8).

![image](https://user-images.githubusercontent.com/100593932/178079529-20625af3-03ff-4681-8e06-d73310ae1c26.png)

**Figura 8. Uso do comando push para empurrar objetos commitados para o repositório remoto no GitHub.**

​	Assim, o objetivo deste projeto (desafio) foi a criação de repositório remoto no GitHub, por meio da ferramenta terminal GitBash, e também a atualização e sincronização que permite organizar de forma estruturada e sistemática (de acordo com a preferência do usuário) os objetos de interesse.

​	Este aprendizado e a possiblidade de apresentá-lo na forma de relatório/artigo é muito gratificante.

​	Desde já agradeço a atenção de todos e o apoio,

 

André Luiz Barbosa.
