**Configurações de ambiente no Linux**

**Pré-requisitos**

* Linux (Fedora 38) instalado
* Gerenciador de pacotes (dnf) instalado
* Git instalado

**Passo a passo**

1. **Mover a pasta Templates**

```
# Mova a pasta Templates para a pasta home

sudo mv ~/Templates/ ~/

# Faça o merge da pasta Templates com a já existente

rsync -a ~/Templates/ ~/Templates/
```

2. **Instalar o zsh e o Oh My Zsh**

```
# Instale o zsh

sudo dnf install zsh

# Instale o Oh My Zsh

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

3. **Alterar o tema para agnoster**

```
# Abra o arquivo .zshrc

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo

ZSH_THEME="agnoster"
```

4. **Instalar o plugin de autosuggestions**


# Abra o terminal

zsh

# Instale o plugin de autosuggestions usando o Oh My Zsh

git clone [https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions

# Habilite o plugin

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo

plugins=(... zsh-autosuggestions ...)


5. **Instalar o GH**

```
# Instale o GH

sudo dnf install gh
```

6. **Mover o arquivo pacman**

```
# Mova o arquivo pacman para a pasta .config

sudo mv ~/pacman ~/.config/
```

7. **Configurar o tamanho do terminal e o background transparente**

**Abra as preferências do terminal:**

```
gnome-terminal --preferences
```

**Altere o tamanho do terminal para 110x30**

```
Tamanho da janela: 110x30
```

**Ative o background transparente**

```
Background transparente: Sim
```

**Salve as alterações.**

**Pronto!**

**Print do terminal:**

image: [https://github.com/Gabrielcafens/ConfToLinux/assets/95833512/76287d0a-cab3-4d45-92dc-d8f8414c8394](https://github.com/Gabrielcafens/ConfToLinux/assets/95833512/76287d0a-cab3-4d45-92dc-d8f8414c8394)
