# ID Magalu CLI
CLI para operações relacionadas aos resources do ID Magalu.

## Instalação do CLI
- Realizar download do arquivo de acordo com o sistema operacional na página [Releases](https://github.com/dadonasll/id-magalu-cli/releases);
- Renomear arquivo para `idm`;

### Linux
- Tornar o arquivo executável -> `chmod +x idm`
- (opcional) Tornar o arquivo executável de qualquer lugar movendo para a pasta bin -> `sudo mv idm /usr/bin`

### Windows
- (opcional) Tornar o arquivo executável de qualquer lugar movendo para a pasta `C:\Windows\System32`.


## Utilização
### Help
```
idm <command> -h

Ex:
idm -h
idm login -h
idm client -h
```

### Login
Para utilizar as features disponíveis é necessário primeiramente realizar o login através do comando:
```
idm login
```

### Clients
#### Listando Clients
O comando a seguir retorna a lista de clients que o usuário possui:
```
idm client list
```

#### Alterando clients
O seguinte comando altera as propriedades de um client:
```
idm client update --id xxx-xxx-x-xxx-xxxx --description "Description Updated" --redirect-uris "https://service.com"
```
Para saber a lista completa de atributos que é possível alterar basta consultar através do comando:
```
idm client update -h
```
