
# 1. Explorando o Git e GitHub 🌍
 
- o [Github](https://github.com/) é um site que permite que você crie repositórios públicos e privados, adicione e edite arquivos, e **compartilhe seus projetos com outras pessoas**.
- O [Git](https://git-scm.com/) é um sistema de controle de versão distribuído que permite gerenciar e compartilhar arquivos e projetos de forma eficiente.

### Quais motivos para usar o Git e GitHub?

- O git é uma ferramenta de controle de versão que permite que **você gerencie suas alterações** de forma eficiente e organizada.
- O git permite que você trabalhe em equipes, compartilhe seus projetos com outras pessoas e ajude a resolver conflitos de código.
- O github permite que você faça **backup de seus projetos e restaure se necessário**.
- O git permite que você rastreie as alterações feitas em seus projetos e faça backup de cada versão.
- O git permite que você gerencie seus projetos de forma eficiente, facilitando a colaboração e a resolução de conflitos.
- O git permite que você trabalhe com **repositórios públicos e privados**, facilitando a colaboração e a resolução de conflitos.
 site que permite que você gerencie seus projetos, compartilhe arquivos e trabalhe em equipes.

### Como escrever no commit?

- **Não existe um padrão de como escrever no commit**, mas recomendamos que você siga as convenções de escrita do seu projeto e que você use uma mensagem de commit que explique claramente o que foi feito;
- Simples e objetivas, **não coloque mais de 72 caracteres**;
- Uso de **verbo no infinitivo**, exemplo: adicionar, remover, etc;
- Não inclua comentários de código.
- **Evite usar termos técnicos**, exemplo: git, github, etc;

### Quando realizar um commit?

- Quando você **finalizar uma tarefa especifica** ou **resolver algum bug**, deixando claro o que foi feito em cada commit;
- Lembre-se de que o commit é o que você está confirmando, não o código;
- **Nunca realizar um commit de um código que você sabe que contém bugs**. O ideal é que o código esteja funcionando e tudo esteja bem.

### Como o git funciona?

- O controle de mudanças é feito através de **commits**. Cada commit é uma unidade de mudança que descreve o que foi feito em um determinado arquivo ou em um conjunto de arquivos.
- O git é **distribuído**, ou seja, cada commit é armazenado em um repositório remoto, como o github, e cada usuário tem permissão para enviar e receber commits.
- O git é **descentralizado**, ou seja, cada usuário tem permissão para enviar e receber commits, mas não tem permissão para modificar o repositório remoto.    
- O git é **offline**, ou seja, o repositório local não precisa estar conectado a internet para ser usado.
- O git é **assíncrono**, ou seja, o repositório local pode ser usado enquanto não está conectado a internet.
- Além de ter um id (identificador único) para cada commit, cada commit também tem um **hash** que é uma representação única do conteúdo do commit.
- Possui um **histórico de commits** que é uma lista de todos os commits realizados no repositório.

## 1.1 comandos básicos do git

- **git init**: inicializa um novo repositório git.
- **git clone**: clona um repositório existente para criar um novo repositório.
- **git add**: adiciona arquivos ao stage.
- **git add .**: Adiciona todos os arquivos no diretório atual ao stage.
- **git commit**: confirma as alterações no stage.
- **git commit "m" \Nomes das mudanças/**: confirma as alterações no stage com uma mensagem de commit.
- **git push**: envia as alterações para o repositório remoto.
- **git pull**: atualiza o repositório local com as alterações do repositório remoto.
- **git log**: exibe o histórico de commits.
- **git diff**: exibe as diferenças entre arquivos.
- **git checkout**: alterna entre branches.
- **git branch**: lista as branches existentes no repositório.
- **git merge**: combina as alterações de uma branch com outra.
- **git rebase**: reorganiza as alterações de uma branch em relação a outra.
- **git reset**: reseta o repositório para uma versão anterior.
- **git status**: exibe informações sobre o repositório.
- **git remote**: lista os repositórios remotos associados ao repositório local.
- **git remote add**: adiciona um repositório remoto ao repositório local.
- **git remote rm**: remove um repositório remoto do repositório local.
- **git remote rename**: renomeia um repositório remoto.
- **git remote show**: exibe informações sobre um repositório remoto.
- **git tag**: cria uma tag no commit atual.
- **git tag -l**: lista todas as tags existentes no repositório.
- **git tag -d**: remove uma tag.

### Comandos avançados do git 🛜

- **git bisect**: encontra o commit que causou um problema.
- **git blame**: exibe o histórico de commits para cada linha de código.
- **git cherry-pick**: combina as alterações de uma branch com outra.
- **git revert**: reverte a última alteração.
- **git revert -n**: reverte a última alteração, mas não adiciona o commit ao histórico.
- **git revert ID**: reverte a alteração especificada pelo ID.
- **git stash**: armazena as alterações no stage e os restaura depois de uma operação.
- **git submodule**: gerencia os módulos do repositório.
- **git worktree**: gerencia os workspaces do repositório.


# Referencias 🔗

- [Git push: enviando alterações locais para o remoto!](https://blog.betrybe.com/git/git-push/);
- [Informações do Git](https://git-scm.com/docs/git-reset/pt_BR);
- [Documentação oficial do Git](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git).