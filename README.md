## git init

## git clone

## git status

## git add .

## git commit -a -m "....."

## - USADO PARA MOVER OU RENOMEAR
git mv

## - remove arquivo ou diretorio
git rm / git rm -r 

## - volta tudo ao estado inicial
git reset -- hard <repo>

## - VOLTA O ARQUIVO AO ESTADO INICIAL
git checkout <arquivo>

## - CRIA UMA BRANCH E TROCA AO MESMO TEMPO
git checkout -b <nome_branch>

## - TROCA PARA A BRANCH ESCOLHIDA
git checkout <nome_branch>

## - mescla branchs
git merge

## - DESFAZ E SALVA AS IMPLEMENTACOES PARA SER RECUPERADAS DEPOIS
git statsh

## - MOSTRA AS STASHS CRIADAS
git statsh list

## - RECUPERA A STASH
git stash apply <numero-stash>

## - MOSTRA AS ALTERAÇÕES FEITAS NAS STASHS
git stash show -p <numero_stash>

## - exclui a statsh
git stash drop <numero_stash>

## - limpa todas as statsh
git stash clear 

## - cria uma tag
git tag -a 'nome' -m 'mensagem'

## - lista as tags criadas
git tag

## - DETALHA AS ALTERAÇÕES DAS TAGS
git show <nome_tag>

## - TROCA DE TAG
git checkout <nome_tag>

## - ENVIA A TAG PARA O REPOSITORIO
git push <repo> <nome_tag>

## - ENVIA TODAS AS TAGAS PARA O REPOSITORIO
git push <repo> --tags

## - DELETA UMA TAG
git tag -d <nome_tag>

## - ATUALIZA TODAS AS BRANCHS E TAGS DO REPOSITORIO PARA O LOCAL
git fetch

## - BAIXA TODAS AS BRANCH
git fetch -a

## - verifica os remote
 git remote -v

## - remove o remote com repositorio
git remote rm <repo>

## - verifica os modulos
git submodule

## - adiciona o repositorio modulo
git submodule add <repo>

## - push no module
git push --recurse-submodules=on-demand 

## - DIFERENÇA DA BRANCH ATUAL PARA A BRANCH REMOTA
git diff

## - DIFERENÇA DE DOIS ARQUIVOS
git diff <arquivo_a> <arquivo_b>

## - log resumido de tudo o que aconteceu
git shortlog

## - Faz com que o arquivo não seja rastreado pelo git
git update-index --assume-unchanged <file>

## - Desfaz o comando acima
git update-index --no-assume-unchanged <file>


##  - Para obter uma lista de arquivos / arquivos que são assume-unchanged execute isso em um shell unix:
git ls-files -v | grep '^h'

## - ou em um PowerShell:
git ls-files -v | Select-String -CaseSensitive '^h'

