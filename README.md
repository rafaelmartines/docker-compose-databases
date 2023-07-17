# Docker Compose Databases

Conjunto de YAMLs para subir contêineres de banco de dados com persistência.

## PostgreSQL

Entrar na pasta pgsql e criar uma pasta com o nome `db-data` no mesmo diretório.

```shell
mkdir db-data
```

Crie um arquivo .env a partir do arquivo .env.example

```shell
cp .env.example .env
```

Por padrão a versão da imagem do postgresql está marcada para baixar a ultima disponivel no Docker Hub, ajuste de acordo com a necessidade.

E então na linha de comando digitar:

```shell
docker-compose up -d
```

Dados de conexão padrão:
```txt
Host: localhost
Porta: 5432
Banco: postgres
Usuário: admin
Senha: admin
```
