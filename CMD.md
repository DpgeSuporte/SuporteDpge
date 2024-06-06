# Comandos uteis no CMD do Windows

### Este comando exibe a capacidade de cada módulo de memória RAM instalado.
wmic memorychip get capacity

## Informações sobre o Disco Rígido (HD) ou SSD

### Este comando lista os modelos dos discos rígidos ou SSDs instalados no seu sistema.
wmic diskdrive get model

### Este comando mostra o tamanho dos discos rígidos ou SSDs instalados.
wmic diskdrive get size

### Este comando mostra SERIAL dos discos rígidos ou SSDs instalados
wmic diskdrive get serialnumber

## Informações sobre a Placa Mãe

### Este comando exibe informações sobre a placa mãe, incluindo o produto, fabricante, versão e número de série.
wmic baseboard get product,Manufacturer,version,serialnumber


## Informações sobre a Placa de Vídeo

### Este comando mostra o nome da placa de vídeo instalada no seu sistema.
wmic path win32_videocontroller get name

## Informações sobre da Bios 

### Este comando mostra o serial da Bios.
wmic bios get serialnumber

