# Passo-a-passo para criação, atualização e sincronização de repositório no GitHub



### 1. Criação do repositório

- Acessar a plataforma do GitHub, e no ícone do usuário selecionar "your repositories";
- Clicar "new" para criar o novo repositório;
- Preencher nome e descrição do repositório, defini-lo como público ou privado e adicionar arquivo README (opcional).



### 2. Download do repositório para a máquina de trabalho

- Entrar no repositório criado e no botão "Code" escolher um dos modos disponíveis de clonagem do repositório: HTTPS, SSH, CLI;
- Usando o modo HTTPS neste exemplo, copiar o link apresentado na referida opção;
- Dentro do diretório da máquina preparado para receber o repositório a ser baixado, clicar com o botão direito do mouse e selecionar "GitBash here";
- Na janela de comando do Git, dar o comando "git clone _link HTTPS copiado_" ;
- Acessar o repositório com o comando "cd _nome do repositório_";
- Usar comando como "ls" e "git status" para verificar a situação no diretório.



### 3. Trabalhos no diretório da máquina

- Realizar normalmente os trabalhos de criação e edição de arquivos a serem feitos no diretório e salvá-los.



### 4. Sincronização com repositórios local e remoto

- Uma vez finalizadas as alterações no diretório de trabalho, dar um "git status" e verificar que o Git acusa as alterações que foram realizadas mas ainda não foram adicionadas ao nível de "stage" para serem posteriormente comitadas;
- Para adicionar as alterações ao nível de "stage", usar o comando "git add -A" ou "git add .";
- Um novo "git status" premite ver que o Git passa a considerar as alterações no controle de versão;
- Para comitar as alterações: "git commit -m _"mensagem descritiva das alterações"_" ;
- Por último, para enviar o último commit para a nuvem (repositório remoto): "git push origin main".