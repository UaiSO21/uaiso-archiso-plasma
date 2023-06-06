# Profile do Plasma UaiSO para o Archiso

Esse é o repositório do profile para o archiso do Plasma com o Calamares

É aqui que guardammos o profile com todas as instruções para gerar a ISO do UaiSO de forma aberta.

Quando falamos de forma aberta é que aqui nesse profile os repositórios são públicos.

Você vai precisar de pouca coisa para gerar uma ISO.

### Criando os diretórios de nosso ambiente

```
mkdir -p ~/Build/iso
mkdir -p ~/Build/uaiso-work-plasma
```
### Instalando o Archiso
```
sudo pacman -S archiso qemu-desktop openssl openssl openssl
```
### Clonando o Profile do UaiSO do Plasma
```
git clone https://github.com/UaiSO21/rchiso-uaiso-plasma.git ~/Build/uaiso-archiso-plasma
```
### Gerando a ISO do Plasma
```
sudo mkarchiso -v -w ~/Build/uaiso-work-plasma -o ~/Build/iso ~/Build/uaiso-archiso-plasma 
```
