# Repositório de Aula

Download pode ser feito via git clone em cada submódulo, ou download do repositório inteiro:

```bash
git clone https://github.com/Draylon/ppgca_aula_repo
cd ppgca_aula_repo
git submodule update --init --recursive
```

## Update direto dos submódulos:

Como atualizar todos os submodulos locais automaticamente:

```bash
git submodule update --remote --merge
```

### Update nos submódulos para push:

Ao fazer uma alteração em um submódulo, executar na raíz:

```bash
git add <submodulo>
git commit -m "msg"
git push
```


### Versionamento de branch dentro do submodulo:

```bash
cd <submodulo>
git checkout <branch>
cd ..
git config -f .gitmodules submodule.<submodulo>.branch <branch>
```

https://docs.google.com/forms/d/e/1FAIpQLSd40cSpCtWBvc0DhgSjZAOwbqr4eh0SpKzKa4reBnBTDnBDvQ/viewform?usp=dialog
