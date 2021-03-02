**Git**

### Comandos Úteis

```bash
  ## Buscar commit por mensagem
  $ git log --all --grep='<yout_message>'

  ## navegação entre commits
  ## Altera o head para do commit especifico
  $ git checkout <id_commit>

  ## Para voltar para o último commit
  $ git checkout master

  ## Criar nova branch
  $ git checkout -b <your-branch>

  ## Navegar entre branches
  $ git checkout <your_branch>

  ## Listar branch remotas
  $ git branch -a 

  ## Listar branch locais
  $ git branch

  ## listar conexões remotas do seu repositório
  $ git remote -v

  ## Forçar commit
  $ git push origin <branch> -f

  ## Remove commit desfazendo o staged
  $ git reset <id_commit> --soft

  ## Remove o commit desfazendo o staged e o modificações
  $ git reset <id_commit> --hard

  ## Outra forma de aplicar o reset
  ## Desfaz o ultimo commit feito
  $ git reset HEAD~1 --soft

```