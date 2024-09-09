# Preparação de Ambiente

### Vamos preparar o ambiente para o desenvolvimento de aplicações


#### Neste ambiente iremos instalar os seguintes recursos:

- Máquina virtual (VirtualBox) 
- Distribuição Linux (UbuntuServer) 
- Nasm 
- Compilador da linguagem C 
- Configurar o ip e a porta de comunicação entre a máquina real e a virtual 
- Configurar o acesso via SSH entre o VSCode e o ServidorLinux 
- Instalar as extenções: Material Icon, Nasm, SSH e linguagem C/C++ 

#### Máquina Virtual (Virtualbox)

!["Logo VirtualBox"](Virtualbox_logo.png)


Máquina Virtual é uma ferramenta que permite a criação de novos "computadores" e a instalação de sistemas operacionais para estudo ou trabalho.

Para o nosso estudo iremos usar o Virtualbox, da Oracle.
Para instalar, basta fazer o download no link a seguir : 
  <a href="https://www.virtualbox.org/wiki/Downloads" target="_blank"> VirtualBox </a> 

  ##### Criando uma Máquina Virtual para o nosso estudo 

  - Configuração:

   >- Nome da Máquina: Servidor
   >- Memória: 4GB(4096)
   >- Processador: 2
   >- Disco: 100GB
   >- IP e Porta do Host:127.0.0.1 e 22
   >- IP e Porta do Convidado: 10.0.2.15 e 22


- Tela inicial de configuração
<img src=tela_inicial_de_configuracao.png width=500 height=250>

- Tela de configuração do Hardware
<img src=tela_de_configuracao_02.png width=500 height=250>

- Tela de configuração de Disco
<img src=tela_de_configuracao_03.png width=500 height=250>

- Tela de final configuração 
<img src=tela_de_configuracao_04.png width=500 height=250>

- Tela inicial de configuração de Rede
<img src=tela_de_configuracao_part2_05.png width=500 height=250>

- Tela de configuração de Portas e IP
<img src=tela_de_configuracao_part2_6.png width=500 height=250>

## Distribuição Ubuntu Server
<img src=logo.webp width=200 heght=200>

Para o nosso estudo iremos utilizar uma distriução Linux para servidores chamada Ubuntu.
Acompanhe o processo de instalação:

Faça o download aqui:
<a href= "https://ubuntu.com/download/server">Ubuntu Server</a>

#### Acompanhe a instalação

- Tela de inicio de instalação
<img src=07_instalacao.png width=500 height=250>

- Tela de idioma
<img src=08_idioma.png width=500 height=250>

- Tela de teclado
<img src=09_teclado.png width=500 height=250>

- Tela de tipo de instalação
<img src=10_instalacao.png width=500 height=250>

- Tela de configuração de rede
<img src=11_rede.png width=500 height=250>

- Tela de configuração de proxy
<img src=12_proxy.png width=500 height=250>

- Tela pacotes de atualização
<img src=13_atualizacao.png width=500 height=250>

- Tela de configuração de disco
<img src=14_disco.png width=500 height=250>

- Tela de layout de disco
<img src=15_layoutdisco.png width=500 height=250>

- Tela de configuração do usuario
<img src=16_usuario.png width=500 height=250>

- Tela de configuração de SSH
<img src=17_configuracaossh.png width=500 height=250>

- Tela de fim da instalação
<img src=18_fiminstalacao.png width=500 height=250>

#### Atualização do Sistema
Para a correta utilização do servirdor Ubuntu que acabamos de instalar, será nescessário realizar a atualização do sistema.

Execute o comando abaixo:

```
sudo apt update -y && sudo apt upgrade -y 
```
Reinicie o seu servirdor usando o comando abaixo: 

```
reboot
```

#### Instalação do compilador Nasm

O copilador NASM é uma ferramenta que nos permite programar em Assembly. Assim é possivel criar programas que manipulam dados que estão nos registradores do processador.

Para instalar o NASM no Ubuntu, usamos o comando: 

```
sudo apt install nasm -y
```

#### Instalação  do compilador da linguagem C

Em Linux, ocompilador da linguagem C é o GCC. Ele é uma ferramenta importante para o desenvolvimento de programas em C.

Para instalar use o comando: 

```
sudo apt install gcc -y
```

#### Conexão servidor e VSCode via SSH

Presisamos instalar uma extensão no VSCode para acessar o nosso servidor de forma remota.

!["Extensão SSH"](19_extensao_ssh.png)

Configuração do acesso remoto.

!["Configuração"](20_configurar_extensao.png)



