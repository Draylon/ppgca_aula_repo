# Repositório de Aula

Download pode ser feito via git clone em cada submódulo, ou download do repositório inteiro:

```bash
git clone https://github.com/your-username/my_repos.git
cd my_repos
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