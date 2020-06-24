# Git-e-Github

## Desfazer alterações

```
git checkout .
```

## Fork

### Setar um Upstream

```
$ git remote -v
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
```

```
git remote add upstream REPOSITORY
```

Para atualizar seu fork com o upstream:

```
git fetch upstream
git pull upstream
```

## Adicionar origem Remota

```
git remote add origin https://github.com/user/repo.git
```

## Restaurar arquivo modificado para o que está versionado

```
git restore ARQUIVO
```

## Limpar Untracked files

```
git clean -f
```

### Caso seja o arquivo ".DS_Store"

```
find . -name '.DS_Store' -type f -delete
```

## Desfazer add 

```
git reset CAMINHO_DO_ARQUIVO/ARQUIVO
git reset --hard
```

## Desfazer commit

```
git revert ID_COMMIT 
```

ID_COMMIT pode ser obtido pelo com comando:

```
git log
```

## Clone Branch

```
git checkout -b <nome-do-seu-branch-local> origin/<nome-do-branch-remoto>
```

## Remover Branch

Local:
```
git branch -d BRANCH_NAME
```
Local com merge pendente:
```
git branch -D BRANCH_NAME
```

Remoto:
```
git push origin --delete BRANCH_NAME
```

## Rodar os testes novamente no Github

```
rp test
```
