# Git + GitHub
## Como Utilizar na Prática

<strong>Git:</strong> é um sistema de controle de versões distribuído, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo.

<strong>GitHub:</strong> é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git. Ele permite que programadores, utilitários ou qualquer usuário cadastrado na plataforma contribuam em projetos privados e/ou Open Source de qualquer lugar do mundo.

1. Baixar e instalar o Git;
2. Abrir o gitBash na pasta de origem do arquivo que deseja fazer o versionamento;

### Primeiro Commit:
#### Linhas de Comando:
1. <code>git init</code>: inicializa o repositório local;
2. <code>git add 'nome do arquivo'</code>: adiciona o arquivo a área de Stage;
3. <code>git status</code>: checa o status e se o arquivo foi adicionado;
4. <code>git commit -m "mensagem desejada"</code>: envia o arquivo adicionado para um repositório local;

   *O GitHub esta mudando o Branch principal de Master para Main e se você o a empresa optar por fazer a mundança entre as branches use o seguinte comando: git branch -m "main";

5. Acesse sua conta no GitHub(suponho que já tenha uma), clique no sinal de '+' no canto superior direito e seleciona a opção de criar um novo repositório. Após criado o novo repositório copie a Url e volte para o GitBash;
6. <code>git remote add origin 'URL copiada'</code>: faz a conexão entre o repositório local e o repositório remoto;
7. <code>git push -u origin main</code>: envia o commit criado para o repositório remoto;

### Versionamento de Arquivos:
1. Abra o GitBash na pasta de origem
2. <code>git add.</code>: envia as modificações feitas para a área de Stage;
3. <code>git commit -m "mensagem desejada"</code>: manda o arquivo para o repositório local;
4. <code>git push origin main</code>: envia o arquivo para o repositório remoto.

### Branch
    Use um branch para isolar o trabalho de desenvolvimento sem afetar outros branches no repositório. 
    Cada repositório tem um branch padrão e pode ter vários outros branches.
    Você pode fundir um branch em outro branch usando uma solicitação pull
1. <code>git checkout -b "nome da branch"</code>: sai da branch Main ou Master e cria uma branch com o nome escolhido.
2. <code>git add.</code>: envia as modificações feitas para a área de Stage;
3. <code>git commit -m "mensagem desejada"</code>: manda o arquivo para o repositório local;
4. <code>git push origin 'nome da branch criada'</code>: envia a branch para o repositório remoto
5. <code>git checkout main</code>: volta para a branch main;
6. <code>git merge "nome da branch"</code>: unifica a branch que foi bifurcada;
7. <code>git push origin main</code>: envia o arquivo para o repositório remoto.

### Clonando um Repositório para sua Máquina
* Abrir o GitBash na pasta para onde deseja copiar o repositório e em seguida dar o comando:
  git clone 'link do arquivo que deseja clonar'

Atualizar um repositório clonado:
    Abrir o GitBash dentro da pasta já clonada e dar o comando:
    <code>git pull</code>


