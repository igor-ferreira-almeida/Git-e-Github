# Git-e-Github

## Desfazer alterações

```
git checkout .
```

## Limpar Untracked files

```
git clean -f
```

## Desfazer add 

```
git reset CAMINHO_DO_ARQUIVO/ARQUIVO
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
