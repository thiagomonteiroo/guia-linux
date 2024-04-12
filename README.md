# GUIA LINUX - COMANDOS BÁSICOS

### Teclas coringas
tab - completar comando

sudo - executar comandos como **administrador**

man - consultar **man**ual da ferramenta

-h - menu de ajuda de opções 

| - joga a saida de um comando para outro

& - executa um comando em segundo plano

&& - executa uma cadeia de comandos

grep - filtro para entrada de textos

### Comandos de manipulação de diretório
ls - **listar** diretório 

cd - **trocar** de diretório

cat - **ler** arquivo

mv - **mover** / **renomear** arquivo

cp - **copiar** arquivo

mkdir - **criar** um diretório


### Programas interativos por linha de comando
nano - editor de texto simples

vi/vim - editor de texto avançado


### Utilitários de rede
ping - **pinga** IPs locais ou na internet

wget - **downloader** via linha de comando

nmcli - interface para o **NetworkManager**

ifconfig - **configurações** de interface de rede (alto nivel)

iw - **configurações** de placas de rede (baixo nivel) 

ss - **vizualizador** de informações da rede

<br>

## Processos e Daemons 

>Os processos são criados em sua maioria na abertura de aplicativos comuns, sejam de programas do usuário ou do próprio sistema operacional 

>Daemons são processos "especiais" que rodam em segundo plano, com o propósito de servir outros programas

#### Exemplos de processos: Firefox, Chrome, Photoshop
#### Exemplos de daemons: MySQL, Tor, Apache

## Gerenciamento de processos
ps - **listar** processos 

top - **monitor** de processos

kill- eliminar processo por **PID**(id do processo)

killall - eliminar processos pelo **nome**

## Gerenciamento de daemons
service - interface de gerenciamento de daemons

systemctl - interface de gerenciamento de daemons em sistemas que usam systemctl

<br>

# Comandos geralmente utilizados

## Utilitarios de rede 

### Ver portas abertas 
```text
sudo ss -tulpn
```

### Ver informaões de rede
```text
nmcli
```

### Scan de redes próximas
```text
sudo iw dev [interface de rede] scan
```

## Gerenciamento de processos e daemons

### Listar processos
```text
ps aux
```

### Procurar por um processo específico
```text
ps aux | grep [nome do processo]
```

### Eliminar um processo
```text
sudo killall [nome do processo]
```

### Ver status de um daemon
```text
sudo service [daemon] status
```

### Iniciar um daemon
```text
sudo service [daemon] start
```

### Desligar um daemon 
```text
sudo service [daemon] stop
```

## Manipulação de diretório

### Excluir um arquivo
```text
rm [arquivo] 
```

### Excluir um diretório
```text
rm -rf [diretório]
```

### Renomear um arquivo
```text
mv [arquivo] [arquivo-renomeado]
```

### Lista um diretório por completo
```text
ls -lah
```

### Voltar um diretório
```text
cd ..
```

### Ir para o diretório Home do usuário
```text
cd ~
```
