```yaml
# GIT INIT

# GIT CLONE

# GIT STATUS

# GIT ADD .

# GIT COMMIT -A -M "....."

# - USADO PARA MOVER OU RENOMEAR
GIT MV

# - REMOVE ARQUIVO OU DIRETÓRIO
GIT RM / GIT RM -R 

# - VOLTA TUDO AO ESTADO INICIAL
GIT RESET -- HARD <REPO>

# - VOLTA O ARQUIVO AO ESTADO INICIAL
GIT CHECKOUT <ARQUIVO>

# - CRIA UMA BRANCH E TROCA AO MESMO TEMPO
GIT CHECKOUT -B <NOME_BRANCH>

# - TROCA PARA A BRANCH ESCOLHIDA
GIT CHECKOUT <NOME_BRANCH>

# - MESCLA BRANCHES
GIT MERGE

# - DESFAZ E SALVA AS IMPLEMENTAÇÕES PARA SER RECUPERADAS DEPOIS
GIT STASH

# - MOSTRA AS STASHES CRIADAS
GIT STASH LIST

# - RECUPERA A STASH
GIT STASH APPLY <NUMERO-STASH>

# - MOSTRA AS ALTERAÇÕES FEITAS NAS STASHES
GIT STASH SHOW -P <NUMERO_STASH>

# - EXCLUI A STASH
GIT STASH DROP <NUMERO_STASH>

# - LIMPA TODAS AS STASHES
GIT STASH CLEAR 

# - CRIA UMA TAG
GIT TAG -A 'NOME' -M 'MENSAGEM'

# - LISTA AS TAGS CRIADAS
GIT TAG

# - DETALHA AS ALTERAÇÕES DAS TAGS
GIT SHOW <NOME_TAG>

# - TROCA DE TAG
GIT CHECKOUT <NOME_TAG>

# - ENVIA A TAG PARA O REPOSITÓRIO
GIT PUSH <REPO> <NOME_TAG>

# - ENVIA TODAS AS TAGS PARA O REPOSITÓRIO
GIT PUSH <REPO> --TAGS

# - DELETA UMA TAG
GIT TAG -D <NOME_TAG>

# - ATUALIZA TODAS AS BRANCHES E TAGS DO REPOSITÓRIO PARA O LOCAL
GIT FETCH

# - BAIXA TODAS AS BRANCHES
GIT FETCH -A

# - VERIFICA OS REMOTES
 GIT REMOTE -V

# - REMOVE O REMOTE COM REPOSITÓRIO
GIT REMOTE RM <REPO>

# - VERIFICA OS MÓDULOS
GIT SUBMODULE

# - ADICIONA O REPOSITÓRIO MÓDULO
GIT SUBMODULE ADD <REPO>

# - PUSH NO MÓDULO
GIT PUSH --RECURSE-SUBMODULES=ON-DEMAND 

# - DIFERENÇA DA BRANCH ATUAL PARA A BRANCH REMOTA
GIT DIFF

# - DIFERENÇA DE DOIS ARQUIVOS
GIT DIFF <ARQUIVO_A> <ARQUIVO_B>

# - LOG RESUMIDO DE TUDO O QUE ACONTECEU
GIT SHORTLOG

# - FAZ COM QUE O ARQUIVO NÃO SEJA RASTREADO PELO GIT
GIT UPDATE-INDEX --ASSUME-UNCHANGED <FILE>

# - DESFAZ O COMANDO ACIMA
GIT UPDATE-INDEX --NO-ASSUME-UNCHANGED <FILE>


#  - PARA OBTER UMA LISTA DE ARQUIVOS / ARQUIVOS QUE SÃO ASSUME-UNCHANGED EXECUTE ISSO EM UM SHELL UNIX:
GIT LS-FILES -V | GREP '^H'

# - OU EM UM POWERSHELL:
GIT LS-FILES -V | SELECT-STRING -CASESENSITIVE '^H'

#SERVE PARA ALTERAR UM COMMIT
#Isso abrirá um editor de texto com uma lista de commits. O HEAD~1 indica que você quer rebasear até o commit anterior ao HEAD (ou seja, o último commit).
git rebase -i HEAD~1


```
