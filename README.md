# Lista de 100 Comandos Importantes do Git <img align="center" alt="git" height="40" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg" />

## Introdução
Este documento fornece uma lista de 100 comandos essenciais do Git, cada um com uma breve descrição de sua função. Git é um sistema de controle de versão distribuído amplamente utilizado para rastrear mudanças no código-fonte durante o desenvolvimento de software.

## Comandos Básicos

1. `git init` - Inicializa um novo repositório Git.
2. `git clone <url>` - Clona um repositório existente de uma URL.
3. `git add <arquivo>` - Adiciona um arquivo ao índice (staging area).
4. `git commit -m "mensagem"` - Confirma as mudanças no índice com uma mensagem.
5. `git status` - Mostra o status atual do repositório.
6. `git log` - Exibe o histórico de commits.
7. `git diff` - Mostra as diferenças entre os arquivos modificados e o último commit.
8. `git branch` - Lista todas as branches no repositório.
9. `git checkout <branch>` - Muda para a branch especificada.
10. `git merge <branch>` - Mescla a branch especificada na branch atual.

## Comandos de Branch

11. `git branch <nome-da-branch>` - Cria uma nova branch.
12. `git branch -d <nome-da-branch>` - Deleta uma branch.
13. `git branch -m <nome-antigo> <nome-novo>` - Renomeia uma branch.
14. `git branch -a` - Lista todas as branches, incluindo as remotas.
15. `git branch -r` - Lista todas as branches remotas.

## Comandos de Remoto

16. `git remote` - Lista os repositórios remotos configurados.
17. `git remote add <nome> <url>` - Adiciona um novo repositório remoto.
18. `git remote remove <nome>` - Remove um repositório remoto.
19. `git remote rename <nome-antigo> <nome-novo>` - Renomeia um repositório remoto.
20. `git remote set-url <nome> <nova-url>` - Altera a URL de um repositório remoto.

## Comandos de Fetch e Pull

21. `git fetch` - Busca as mudanças dos repositórios remotos sem mesclar.
22. `git pull` - Busca e mescla as mudanças do repositório remoto na branch atual.
23. `git fetch --all` - Busca as mudanças de todos os repositórios remotos.
24. `git pull --rebase` - Rebaseia as mudanças ao invés de mesclar.

## Comandos de Push

25. `git push` - Envia os commits da branch local para o repositório remoto.
26. `git push -u <remoto> <branch>` - Define a upstream da branch local para o repositório remoto.
27. `git push --force` - Força o envio, sobrescrevendo a branch remota.
28. `git push --tags` - Envia todas as tags locais para o repositório remoto.
29. `git push <remoto> :<branch>` - Deleta uma branch remota.

## Comandos de Rebase

30. `git rebase <branch>` - Rebaseia a branch atual na branch especificada.
31. `git rebase --continue` - Continua o rebase após resolver conflitos.
32. `git rebase --abort` - Aborta o rebase e retorna ao estado anterior.
33. `git rebase -i <commit>` - Realiza um rebase interativo a partir do commit especificado.

## Comandos de Stash

34. `git stash` - Guarda as mudanças não confirmadas para uso posterior.
35. `git stash apply` - Aplica as mudanças do stash mais recente.
36. `git stash pop` - Aplica e remove o stash mais recente.
37. `git stash list` - Lista todos os stashes.
38. `git stash drop` - Remove um stash específico.

## Comandos de Tag

39. `git tag` - Lista todas as tags.
40. `git tag <nome>` - Cria uma nova tag.
41. `git tag -a <nome> -m "mensagem"` - Cria uma tag anotada.
42. `git tag -d <nome>` - Deleta uma tag local.
43. `git push <remoto> <tag>` - Envia uma tag para o repositório remoto.
44. `git push <remoto> --tags` - Envia todas as tags para o repositório remoto.
45. `git tag -l "padrão"` - Lista tags que correspondem ao padrão.

## Comandos de Log e Histórico

46. `git log --oneline` - Exibe o histórico de commits em uma linha.
47. `git log --graph` - Exibe um gráfico do histórico de commits.
48. `git log -p` - Mostra as mudanças de cada commit.
49. `git log --author="autor"` - Filtra os commits por autor.
50. `git log --since="data"` - Mostra os commits desde uma data específica.
51. `git log --until="data"` - Mostra os commits até uma data específica.

## Comandos de Aliases

52. `git config --global alias.<atalho> '<comando>'` - Cria um atalho para um comando Git.
53. `git config --global alias.st 'status'` - Exemplo de alias para `git status`.
54. `git config --global alias.co 'checkout'` - Exemplo de alias para `git checkout`.
55. `git config --global alias.br 'branch'` - Exemplo de alias para `git branch`.
56. `git config --global alias.ci 'commit'` - Exemplo de alias para `git commit`.

## Comandos de Configuração

57. `git config --global user.name "nome"` - Define o nome do usuário.
58. `git config --global user.email "email"` - Define o email do usuário.
59. `git config --global core.editor "editor"` - Define o editor de texto padrão.
60. `git config --global merge.tool "ferramenta"` - Define a ferramenta de merge.
61. `git config --global alias.<atalho> "comando"` - Cria um alias para um comando.

## Comandos de Reset e Revert

62. `git reset --hard` - Reseta o índice e o diretório de trabalho para o último commit.
63. `git reset --soft` - Reseta apenas o índice, mantendo as mudanças no diretório de trabalho.
64. `git reset HEAD <arquivo>` - Remove um arquivo do índice.
65. `git revert <commit>` - Reverte um commit específico.
66. `git revert --no-commit <commit>` - Reverte um commit sem criar um novo commit.

## Comandos de Clean

67. `git clean -f` - Remove arquivos não rastreados do diretório de trabalho.
68. `git clean -fd` - Remove diretórios e arquivos não rastreados.
69. `git clean -n` - Mostra o que seria removido, sem realmente remover.
70. `git clean -x` - Remove arquivos ignorados por .gitignore.

## Comandos de Cherry-Pick

71. `git cherry-pick <commit>` - Aplica as mudanças de um commit específico na branch atual.
72. `git cherry-pick --continue` - Continua o cherry-pick após resolver conflitos.
73. `git cherry-pick --abort` - Aborta o cherry-pick e retorna ao estado anterior.

## Comandos de Diff

74. `git diff <branch1> <branch2>` - Mostra as diferenças entre duas branches.
75. `git diff <commit1> <commit2>` - Mostra as diferenças entre dois commits.
76. `git diff --staged` - Mostra as diferenças entre o índice e o último commit.
77. `git diff --cached` - Mostra as diferenças entre o índice e o último commit.
78. `git diff <arquivo>` - Mostra as diferenças em um arquivo específico.

## Comandos de Submodule

79. `git submodule add <url> <caminho>` - Adiciona um submódulo.
80. `git submodule update` - Atualiza todos os submódulos.
81. `git submodule init` - Inicializa os submódulos no repositório.
82. `git submodule deinit <caminho>` - Desinicializa um submódulo.
83. `git submodule sync` - Sincroniza URLs dos submódulos.

## Comandos de Blame

84. `git blame <arquivo>` - Mostra quem modificou cada linha do arquivo.
85. `git blame -L <início>,<fim> <arquivo>` - Mostra as modificações em um intervalo específico de linhas.
86. `git blame <commit> <arquivo>` - Mostra o histórico de um arquivo até um commit específico.

## Comandos de Archive

87. `git archive -o <arquivo.zip> HEAD` - Cria um arquivo zip do repositório no estado atual.
88. `git archive --format=tar HEAD | tar -x -C <diretório>` - Extrai o repositório para um diretório específico.

## Comandos de Bisect

89. `git bisect start` - Inicia a busca binária para encontrar um commit com erro.
90. `git bisect bad` - Marca o commit atual como ruim.
91. `git bisect good <commit>` - Marca um commit específico como bom.
92. `git bisect reset` - Reseta a busca binária.

## Comandos de Grep

93. `git grep <padrão>` - Pesquisa por um padrão no repositório.
94. `git grep -n <padrão>` - Pesquisa por um padrão e mostra os números das linhas.
95. `git grep --count <padrão>` - Conta o número de ocorrências do padrão.

## Outros Comandos

96. `git show <commit>` - Mostra os detalhes de um commit específico.
97. `git shortlog` - Mostra um resumo dos commits por autor.
98. `git describe` - Mostra uma descrição baseada em tags e commits.
99. `git reflog` - Mostra o histórico de referências da HEAD.
100. `git fsck` - Verifica a integridade e a validade do sistema de arquivos Git.

## Conclusão
Estes são alguns dos comandos mais importantes do Git que podem ajudar a gerenciar seus projetos de desenvolvimento de software de maneira eficiente. Para mais detalhes sobre cada comando, consulte a documentação oficial do Git.
