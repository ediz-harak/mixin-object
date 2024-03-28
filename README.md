# Instalação

### Observação

Deixei este detalhe registrado porque me custou tempo para descobrir.


Rode os comandos abaixo na pasta do projeto:

```
go mod init modulo
go get .
```


# Build

Depois de qualquer alteração no código, recompile:

```
go build main.go
```


# Execução

```
./main
```


# Demonstração

[Demonstração principal](https://youtu.be/QVEsWWBr-l0)

Depois de gravar essa demonstração, fiz mais duas: uma cobrindo casos fora do fluxo básico, e outra sobre gravação de valores com espaços aparados no nome do produto e formatação geral.

[Segunda parte](https://youtu.be/P1CCSaFhsw4)

[Terceira parte](https://youtu.be/oCYcXkwUZ4Y)

# Coleção de requisições

Para testar sem escrever cliente, uso uma coleção pronta de requisições. A ferramenta precisa do agente instalado na máquina.

Importe o arquivo `postmanCollection.json` da raiz do repositório.

**Atenção**: o endereço do servidor na coleção está fixado em `http://127.0.0.1:8081`. As rotas de leitura respondem direto nesse endereço; a rota de criação também funciona pelo navegador, mas exige um formulário que não faz parte deste projeto — e que é simples de montar, se você quiser.