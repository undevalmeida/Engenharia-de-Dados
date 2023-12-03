# Tutorial Docker

1. Abra o Docker Desktop. (Baixe [Aqui](https://www.docker.com/products/docker-desktop/) se não tiver).
2. Digite o seguinte comando em seu terminal: ```docker run -dp 80:80 docker/getting-started```
3. Abra seu navegador para <http://localhost>
4. Divirta-se!

## Primeiros Passos

### O comando que você acabou de executar 

Parabéns;! Você iniciou o contêiner para este tutorial! Vamos primeiro explicar o comando que você acabou de executar. Caso você tenha esquecido, aqui está o comando:

```
docker run -d -p 80:80 docker/getting-started
```

Você notará algumas bandeiras sendo usadas. Aqui estão mais algumas informações sobre eles:

* -d - executar o contêiner no modo separado (em segundo plano)
* -p 80:80 - mapear a porta 80 do host para a porta 80 no contêiner
* docker/getting-started - a imagem a ser usada

> #### Dica Profissional  
> Você pode combinar sinalizadores de caractere único para encurtar o comando completo. Como exemplo, o comando acima poderia ser escrito como:
>```
> docker run -dp 80:80 docker/getting-started
>```


### O que é um container?
Agora que você executou um contêiner com sucesso, vamos nos perguntar o que é um contêiner? Simplificando, um contêiner é outro processo em sua máquina que foi isolado de todos os outros processos na máquina host. Esse isolamento aproveita [namespaces de kernel e cgroups](https://medium.com/@saschagrunert/demystifying-containers-part-i-kernel-space-2c53d6979504), recursos que estão no Linux há muito tempo. O Docker trabalhou para tornar esses recursos acessíveis e fáceis de usar.