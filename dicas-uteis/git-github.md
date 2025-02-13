# 1. Explorando o Git e GitHub 🌍

- o [Github](https://github.com/) é um site que permite que você crie repositórios públicos e privados, adicione e edite arquivos, e **compartilhe seus projetos com outras pessoas**.
- O [Git](https://git-scm.com/) é um sistema de controle de versão distribuído que permite gerenciar e compartilhar arquivos e projetos de forma eficiente.

## Quais motivos para usar o Git e GitHub?

- O git é uma ferramenta de controle de versão que permite que **você gerencie suas alterações** de forma eficiente e organizada.
- O git permite que você trabalhe em equipes, compartilhe seus projetos com outras pessoas e ajude a resolver conflitos de código.
- O github permite que você faça **backup de seus projetos e restaure se necessário**.
- O git permite que você rastreie as alterações feitas em seus projetos e faça backup de cada versão.
- O git permite que você gerencie seus projetos de forma eficiente, facilitando a colaboração e a resolução de conflitos.
- O git permite que você trabalhe com **repositórios públicos e privados**: facilitando a colaboração e a resolução de conflitos.
  site que permite que você gerencie seus projetos, compartilhe arquivos e trabalhe em equipes.

## Como escrever no commit?

- **Não existe um padrão de como escrever no commit**: mas recomendamos que você siga as convenções de escrita do seu projeto e que você use uma mensagem de commit que explique claramente o que foi feito;
- Simples e objetivas, **não coloque mais de 72 caracteres**;
- Uso de **verbo no infinitivo**: exemplo: adicionar, remover, etc;
- Não inclua comentários de código.
- **Evite usar termos técnicos**: exemplo: git, github, etc;

## Quando realizar um commit?

- Quando você **finalizar uma tarefa especifica** ou **resolver algum bug**: deixando claro o que foi feito em cada commit;
- Lembre-se de que o commit é o que você está confirmando, não o código;
- **Nunca realizar um commit de um código que você sabe que contém bugs**. O ideal é que o código esteja funcionando e tudo esteja bem.

## Como o git funciona?

- O controle de mudanças é feito através de **commits**. Cada commit é uma unidade de mudança que descreve o que foi feito em um determinado arquivo ou em um conjunto de arquivos.
- O git é **distribuído**: ou seja, cada commit é armazenado em um repositório remoto, como o github, e cada usuário tem permissão para enviar e receber commits.
- O git é **descentralizado**: ou seja, cada usuário tem permissão para enviar e receber commits, mas não tem permissão para modificar o repositório remoto.
- O git é **offline**: ou seja, o repositório local não precisa estar conectado a internet para ser usado.
- O git é **assíncrono**: ou seja, o repositório local pode ser usado enquanto não está conectado a internet.
- Além de ter um id (identificador único) para cada commit, cada commit também tem um **hash** que é uma representação única do conteúdo do commit.
- Possui um **histórico de commits** que é uma lista de todos os commits realizados no repositório.

## Comandos básicos do git

- **`git init`**: inicializa um novo repositório git.
- **`git clone`**: clona um repositório existente para criar um novo repositório.
- **`git add`**: adiciona arquivos ao stage.
- **`git add .`**: adiciona todos os arquivos no diretório atual ao stage.
- **`git commit`**: confirma as alterações no stage.
- **`git commit "m" \Nomes das mudanças/`**: confirma as alterações no stage com uma mensagem de commit.
- **`git push`**: envia as alterações para o repositório remoto.
- **`git pull`**: atualiza o repositório local com as alterações do repositório remoto.
- **`git log`**: exibe o histórico de commits.
- **`git diff`**: exibe as diferenças entre arquivos.
- **`git checkout`**: alterna entre branches.
- **`git branch`**: lista as branches existentes no repositório.
- **`git merge`**: combina as alterações de uma branch com outra.
- **`git rebase`**: reorganiza as alterações de uma branch em relação a outra.
- **`git reset`**: reseta o repositório para uma versão anterior.
- **`git status`**: exibe informações sobre o repositório.
- **`git remote`**: lista os repositórios remotos associados ao repositório local.
- **`git show`**: exibe informações detalhadas sobre um commit específico, incluindo as mudanças realizadas.
- **`git remote add`**: adiciona um repositório remoto ao repositório local.
- **`git remote rm`**: remove um repositório remoto do repositório local.
- **`git remote rename`**: renomeia um repositório remoto.
- **`git remote show`**: exibe informações sobre um repositório remoto.
- **`git tag`**: cria uma tag no commit atual.
- **`git tag -l`**: lista todas as tags existentes no repositório.
- **`git tag -d`**: remove uma tag.
- **`git tag -a [tag] -m [mensagem]`**: cria uma tag e adiciona uma mensagem ao commit.
- **`git config`**: exibe ou altera configurações do Git.
- **`git fetch`**: baixa as alterações do repositório remoto sem aplicá-las.
- **`git ls-files`**: lista os arquivos rastreados pelo Git.
- **`git rm`**: remove arquivos do repositório e do diretório de trabalho.

### Comandos avançados do git 🛜

- **`git bisect`**: encontra o commit que causou um problema.
- **`git blame [arquivo]`**: exibe o histórico de commits para cada linha de código.
- **`git cherry-pick [commit]`**: combina as alterações de uma branch com outra.
- **`git revert`**: reverte a última alteração.
- **`git revert -n`**: reverte a última alteração, mas não adiciona o commit ao histórico.
- **`git revert ID`**: reverte a alteração especificada pelo ID.
- **`git stash`**: armazena as alterações no stage e os restaura depois de uma operação.
- **`git submodule`**: gerencia os módulos do repositório.
- **`git worktree`**: gerencia os workspaces do repositório.
- **`git reflog`**: exibe o histórico das referências do Git (como HEAD e branches).
- **`git submodule`**: gerencia submódulos no repositório.
- **`git worktree`**: permite gerenciar múltiplos diretórios de trabalho associados ao repositório.

# Comandos Específicos do Git

- **`git stash apply`**: aplica o stash que está na área de trabalho.
- **`git stash drop`**: remove o stash que está na área de trabalho.
- **`git stash list`**: lista todos os stashes que estão na área de trabalho.
- **`git stash pop`**: aplica o stash que está na área de trabalho e remove o stash da área de trabalho.
- **`git stash save`**: salva o stash atual na área de trabalho.
- **`git stash show [stash]`**: exibe o stash que está na área de trabalho.
- **`git stash clear`**: remove todos os stashes da área de trabalho.

- Apply
O comando git stash apply espera um índice de um item na stash e o aplica ao repositório, porém, esse comando não remove o item da stash, ou seja, se após executar o comando git stash apply 1 você executar git stash list, o item referente ao índice 1 continuará na stash.

- Pop
O git stash pop faz exatamente a mesma coisa que o git stash apply, porém, além de aplicar o item da stash, ele também o remove de lá. Esse comando, sem nenhum parâmetro extra, vai aplicar o último item adicionado à stash, mas nós também podemos informar um índice para ele, como git stash pop 1.

- Drop
O git stash drop funciona exatamente como o pop, mas com uma simples diferença: ele apenas remove o item da stash, sem aplicá-lo em nosso repositório. Dessa forma, git stash drop remove o último item adicionado à stash, enquanto o git stash drop 1 remove da stash o item com índice 1.

## Histórico de Commits

- **`git log --follow [arquivo]`**: Exibe o histórico de commits de um arquivo específico, incluindo renomeações, permitindo rastrear mudanças ao longo do tempo.
- **`git log --stat`**: Exibe o histórico de commits de uma branch, mostrando informações sobre o número de arquivos modificados, linhas adicionadas e removidas.
- **`git log --oneline`**: Exibe o histórico de commits de uma branch em formato compacto, com uma linha por commit, mostrando o hash abreviado e a mensagem de commit.
- **`git log --graph`**: Exibe o histórico de commits de uma branch visualmente, com uma representação gráfica das ramificações do repositório.
- **`git log --format="formato"`**: Exibe o histórico de commits de uma branch, com a mensagem de commit formatada de acordo com o formato especificado.
- **`git log --decorate`**: Exibe o histórico de commits de uma branch, com anotações sobre referências (como branches e tags) nos commits.
- **`git log --oneline --decorate`**: Exibe o histórico de commits de uma branch em formato compacto, com informações sobre as referências, como branches e tags.
- **`git log --graph --decorate`**: Exibe o histórico de commits de uma branch visualmente, com as referências (branches, tags) decorando os commits.
- **`git log --oneline --graph --decorate`**: Exibe o histórico de commits de uma branch de maneira compacta e visual, incluindo a representação gráfica das ramificações e as referências (como branches e tags).

## Filtragem e Visualização Avançada

- **`git log --since="data"`**: Exibe commits a partir de uma data específica (ex: `git log --since="2024-01-01"`).
- **`git log --until="data"`**: Exibe commits até uma data específica (ex: `git log --until="2024-01-01"`).
- **`git log --author="nome"`**: Exibe commits feitos por um autor específico.
- **`git log -p`**: Exibe o histórico de commits com o diff completo de cada commit, mostrando as alterações feitas no código.
- **`git log --reverse`**: Exibe o histórico de commits de forma invertida, começando do commit mais antigo.

## Outros Comandos Úteis

- **`git log --abbrev-commit`**: Exibe o histórico de commits, mas com os hashes dos commits abreviados.
- **`git log --merges`**: Exibe apenas os commits de merge.
- **`git log --no-merges`**: Exibe todos os commits, exceto os de merge.
- **`git switch -c nova-funcionalidade`**: Cria uma nova branch e muda para ela.

### Git Branch

- **`git branch -m master main`**: Renomeia a branch `master` para `main`.
- **`git branch -d main`**: Deleta a branch `main`.
- **`git branch -D main`**: Deleta a branch `main` remotamente.
- **`git branch -a`**: Lista todas as branches locais e remotas.
- **`git branch -r`**: Lista todas as branches remotas.
- **`git branch -r -d origin/main`**: Deleta a branch `main` remota.

# O que é Head, Origin, Upstream, etc?

- **HEAD**: O **HEAD** é o ponteiro de referência para o commit ou a branch atual. Ele aponta para o último commit da branch onde você está no momento ou para o commit em um "detached HEAD state".
- **Origin**: O **origin** é o nome padrão dado ao repositório remoto de onde você clonou o projeto. É a versão principal do repositório, de onde você faz `git pull` e para onde você envia suas alterações com `git push`.
- **Upstream**: O **upstream** geralmente se refere ao repositório remoto de onde você originalmente clonou o projeto, mas pode ser qualquer repositório remoto de onde você busca alterações. Em um cenário com múltiplos repositórios remotos, o **upstream** pode ser configurado para o repositório original, enquanto o **origin** pode ser o repositório no qual você está trabalhando.
- **Branch**: Uma **branch** é uma ramificação do repositório. Ela permite que você trabalhe em diferentes versões do seu projeto simultaneamente. Ao criar uma nova branch, você cria uma cópia do estado atual do projeto, onde pode fazer alterações sem afetar a branch principal.
- **Commit**: Um **commit** é uma alteração registrada no repositório. Cada commit captura um estado do repositório em um momento específico, permitindo que você tenha um histórico de mudanças e possa voltar a versões anteriores, se necessário.
- **Merge**: Um **merge** é a ação de combinar duas branches. Quando você faz um `git merge`, o Git tenta unir as alterações feitas em diferentes branches. Se houver conflitos entre as mudanças, você precisará resolvê-los manualmente.
- **Pull**: Um **pull** é uma operação que consiste em baixar as alterações de um repositório remoto para o seu repositório local. Ele realiza um `git fetch` seguido de um `git merge` para combinar as mudanças remotas com sua branch local.
- **Push**: Um **push** é a operação de enviar as alterações que você fez localmente para um repositório remoto. Após fazer commits no seu repositório local, você usa `git push` para enviar essas alterações para o repositório remoto, tornando-as acessíveis para outros desenvolvedores.
- **Rebase**: O **rebase** é uma alternativa ao **merge**. Ele re-aplica os commits de uma branch em outra, reescrevendo o histórico. Ao invés de criar um novo commit de merge, o rebase "move" os commits da sua branch para o topo da branch base, tornando o histórico mais linear.
- **Stash**: O **stash** é uma maneira de salvar temporariamente mudanças não commitadas. Quando você está no meio de algo e precisa mudar de branch ou fazer outra tarefa, pode usar `git stash` para guardar essas mudanças. Mais tarde, você pode aplicar o que guardou com `git stash apply`.
- **Submodule**: Um **submódulo** é um repositório Git dentro de outro repositório Git. Usado quando você deseja incluir uma dependência externa ou outro projeto Git dentro do seu repositório, sem realmente mesclar os históricos de ambos. Submódulos têm seu próprio repositório, e o Git mantém a referência para ele.
- **Worktree**: Um **worktree** é um diretório que contém uma cópia de trabalho de uma branch de um repositório. Ele permite que você tenha múltiplas cópias do seu repositório, permitindo trabalhar em diferentes branches ao mesmo tempo, sem precisar de múltiplas clones completos do repositório.


# O que é fast forward?

- **Fast forward**: O **fast forward** é uma maneira de fazer um commit que não adiciona novas linhas de código, mas sim muda as linhas de código existentes. Ou seja um merge de um commit para o HEAD.

# Pull requests para open-source
- Pull requests são um mecanismo de colaboração para projetos open-source. Ele permite que você solicite a adição de novas funcionalidades ou correções de bugs ao seu projeto, sem precisar de ter acesso ao código-fonte do projeto.
- Quando você cria um pull request, o GitHub cria um branch de trabalho para o pull request. Isso permite que você trabalhe em uma cópia do branch principal, sem afetar o branch principal do repositório.
- Quando você envia o pull request, o GitHub verifica se há conflitos de merge. Se houver, você precisará resolver esses conflitos antes de enviar o pull request.
- Quando o pull request é aceito, o GitHub cria um commit no branch principal do repositório e atualiza a branch principal para apontar para o commit do pull request.
- O GitHub também permite que você revise e discuta o pull request antes de ser aceito. Isso permite que você garanta que o pull request esteja funcionando corretamente e que não há conflitos de merge.

# 📶 Github Pages

- Github Pages é um serviço de hospedagem de sites estáticos hospedados no GitHub. Ele permite que você crie um site estático e publicar ele para o mundo.
- Para criar um site estático, você precisa criar um arquivo `index.html` no diretório raiz do seu repositório.
- Você pode usar HTML, CSS e JavaScript para criar sites estáticos.
- Você pode hospedar seu site estático em um servidor de hospedagem de sites estáticos ou em um servidor de hospedagem de aplicativos.


# Referências 🔗
:pushpin: **Como fazer um bom README** - [Alura](https://www.alura.com.br/artigos/escrever-bom-readme)  
:pushpin: **Curso de Git e GitHub: dominando controle de versão de código** - [Alura](https://cursos.alura.com.br/course/git-github-dominando-controle-versao-codigo)  
:pushpin: **Documentação oficial do Git** - [Git SCM](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-O-B%C3%A1sico-do-Git)  
:pushpin: **Git push: enviando alterações locais para o remoto!** - [Blog da Trybe](https://blog.betrybe.com/git/git-push/)  
:pushpin: **Github Pages como usar?** - [Documentação oficial](https://docs.github.com/pt/pages/getting-started-with-github-pages/about-github-pages)  
:pushpin: **Informações do Git** - [Git SCM](https://git-scm.com/docs/git-reset/pt_BR)  
:pushpin: **Visualização do Git** - [Visualizing Git](https://git-school.github.io/visualizing-git/)


