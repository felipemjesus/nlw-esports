# NLW eSports

## Ambiente

Criação do container docker com a imagem Node LTS

Portas liberadas:
- Web: 5173
- Server: 3333
- Mobile: 19000

Obs: ao executar o comando será criado o container e já vai entrar no dele.
```
docker run -it -u "node" -v `pwd`:`pwd` -w `pwd` -p 3333:3333 -p 5173:5173 -p 19000:19000 -p 5555:5555 --name nlw-esports node:lts bash
```

Start no container, após criado.
```
docker start nlw-esports
```

Entrar do container, após criado.
```
docker exec -it nlw-esports bash
```
