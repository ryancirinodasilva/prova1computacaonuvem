# Prova 1 de Computação em Nuvem
Nome: Ryan Cirino Da Silva
RA: c6f7900d066d066b12e0e

## O que fiz

Executei uma paágina web em um contêiner Docker chamado loja.
Usei a imagem nginx:alpine e a porta 8081 do ambiente.

## Verficação do contêiner

Cole aqui a saída do comando docker ps: 
root@ubuntu:~$ docker ps
CONTAINER ID   IMAGE          COMMAND                  CREATED          STATUS          PORTS                                     NAMES
361b4dff2613   nginx:alpine   "/docker-entrypoint.…"   53 seconds ago   Up 53 seconds   0.0.0.0:8081->80/tcp, [::]:8081->80/tcp   loja

## Teste da página

Cole aqui a resposta do comando curl http://localhost:8081:
root@ubuntu:~$ curl http://localhost:8081
<!DOCTYPE html>
html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Loja</title>
</head>
<body>
<h1>Loja no ar</h1>
</body>
</html>

## Explicação

Com minhas palavras, qual é a diferença entre a imagem nginx:alpine
e o contêiner loja? Para que serviu o mapeamento 8081:80

A imagem ngix:alpine é uma imagem modelo, o contêiner Loja é a instancia rodando efetivamente

O mapeamento 8081:80 é 8081 -> porta do host, ou seja da minha maquina. Já a 80 é a porta do contêiner. 
Na pratica eu referencio a porta 8081 do meu host para a porta 80 do contêiner.


## Informações adicionais

### Usamos o killer coda para realizar essa atividade segue link:
https://killercoda.com/

Após entrar faça o login (recomendo o SSO do GitHub)
Campo Playgrounds; Ubuntu 24.04.
Para fazer essa atividade usamos o Ubuntu 24.04.

Obs: O tempo para realizar a atividade é de exatamente 60 min.

Deixei o log do meu Terminal, Ele está nomeado como Log do Ubuntu

No index.html temos o HTML do site da loja
 
E o arquivo Instrucao tem o arquivo que copiamos da prova, é as mesma presentes no Log do Ubuntu
