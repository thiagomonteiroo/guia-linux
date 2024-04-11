# GUIA LINUX - COMANDOS BÁSICOS

### Teclas coringas
tab - completar comando

sudo - executar comandos como **administrador**

man - consultar **man**ual da ferramenta

-h - menu de ajuda de opções 

### Comandos de manipulação de diretório
ls - **listar** diretório 

cd - **trocar** de diretório

cat - **ler** arquivo

mv - **mover** / **renomear** arquivo

cp - **copiar** arquivo

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

---

## Processos e Daemons 

>Os processos são criados em sua maioria na abertura de aplicativos comuns, sejam de programas do usuário ou do próprio sistema operacional 

>Daemons são processos "especiais" que rodam em segundo plano, com o propósito de servir outros programas

#### Exemplos de processos: Firefox, Chrome, Photoshop
#### Exemplos de daemons: MySQL, Tor, Apache

## Gerenciamento de processos
ps - **listar** processos 

kill- eliminar processo por **PID**(id do processo)

killall - eliminar processos pelo **nome**

## Gerenciamento de daemons
service - interface de gerenciamento de daemons

systemctl - interface de gerenciamento de daemons em sistemas que usam systemctl

---

# Comandos geralmente utilizados

## Utilitarios de rede 
>sudo ss -tulpn // 

### Examples

```text
gobuster dir -u https://mysite.com/path/to/folder -c 'session=123456' -t 50 -w common-files.txt -x .php,.html
```
