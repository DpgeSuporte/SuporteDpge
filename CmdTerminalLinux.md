### INSTALAÇÃO DO ANYDESK

sudo apt update

sudo apt -y upgrade

curl -fsSL https://keys.anydesk.com/repos/DEB-GPG-KEY|sudo gpg --dearmor -o /etc/apt/trusted.gpg.d/anydesk.gpg

echo "deb http://deb.anydesk.com/ all main" | sudo tee /etc/apt/sources.list.d/anydesk-stable.list

sudo apt update

sudo apt install anydesk


### INSTALAÇÃO DO GOOGLE CHROME

sudo apt update
sudo apt upgrade

wget --version
sudo apt install wget

wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb

OBSERVAÇÃO: Corrija os erros de instalação do Chrome. Se qualquer erro for exibido durante a instalação, digite sudo apt-get install -f e pressione a tecla ↵ Enter para repará-lo.


### REMOVENDO O Google Chrome

sudo apt-get remove --purge google-chrome

### INSTAÇÃO DO LibreOffice

sudo add-apt-repository -y ppa:libreoffice/ppa
sudo apt-get update
sudo apt-get install libreoffice
sudo apt-get install libreoffice-gnome
sudo apt-get install libreoffice-l10n-pt-br

### REMOVENDO O LibreOffice - 1

sudo apt-get remove libreoffice
sudo apt-get autoremove

### REMOVENDO O LibreOffice - 2

sudo apt-get remove --purge libreoffice*
sudo apt-get clean
sudo apt-get autoremove

### REMOÇÃO DO CHROME NO LINUX UBUNTU

sudo apt-get remove google-chrome.*
sudo apt-get --purge remove google-chrome.*
sudo apt-get update

### PERMISSÃO NA PASTA

chmod 777 -R nomedapasta/

### MAPEAR A PASTA DE REDE NO LINUX - DPGE

gedit /etc/fstab
#### Observação: Alterar o USERNAME e SENHA

//172.16.64.23/cascavel /home/dpge/cascavel cifs user,rw,uid=1000,gid=1000,nounix,iocharset=utf8,file_mode=0777,dir_mode=0777,username=dpge,password=dpgece,domain=dpge 0 0

# INGRESSAR MAQUINA LINUX NO AD

#### 1 – VERIFICAR SE ESTA VISUALIZANDO O NOSSO DOMÍNIO (defensoria.ce.def.br)
nslookp defensoria.ce.def.br

#### 2 – ADICIONAR O REPOSITÓRIO DA APLICAÇÃO NO LINUX

sudo add-repository ppa:emoraes25\cid

#### 3 – DEPOIS RODAR O COMANDO 

apt-update

#### 4 – AGORA FAZER A INSTALAÇÃO DA APLICAÇÃO

sudo apt install cid cid-gtk

#### 5 – AO MOMENTO DA INSTALAÇÃO IRA APARECER UMA TELA DE (Configurando
Autenticação via Kerberos) VOÇE IRA COLOCAR O NOSSO DOMINIO
(DEFENSORIA.CE.DEF.BR) TODO EM CAIXA ALTA E SELECIONAR OK

#### 6 – APOS A INSTALAÇÃO, DAR O COMANDO 

sudo cid-gtk

#### 7 – IRA APARECER UMA TELA PARA FAZER A CONFIGURAÇÃO DO DOMÍNIO, CLIQUE
EM (Join the domain).

#### 8 - EM SEGUIDA, FAZER OS SEGUINTES PREENCHIMENTOS PARA INGRESSAR NO DOMINIO

#### Domain – defensoria.ce.def.br
#### Organizational Unit – Computadores
#### User – Administrator
#### Password – C)t1n0697
#### Mode – Default

#### 9 – APOS INGRESSAR NO DOMINIO, ENTRE COM O SEU RESPECTIVO USUARIO PARA VALIDAR, ENTRE NO TERMINAL E COLOQUE O SEGUINTE COMANDO 

#### - APOS VALIDAR A MAQUINA, ESTARÁ PRONTA !

#### OBS – FAVOR ANTES DE TUDO ALTERAR SE NECESSARIO O NOME DA MAQUINA, PARA QUE O ANALISTA POSSA ORGANIZAR NA ARVORE DO AD, DEVIDO COM O SEU SETOR
sudo cid status

###

