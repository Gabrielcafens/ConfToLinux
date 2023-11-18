**Configurações de ambiente no Linux**

**Pré-requisitos**

* Linux (Fedora 38) instalado
* Gerenciador de pacotes (dnf) instalado
* Git instalado

**Passo a passo**

1. **Mover a pasta Templates**

```
# Mova a pasta Templates para a pasta home :tada: :strawberry:

sudo mv ~/Templates/ ~/

# Faça o merge da pasta Templates com a já existente :sparkles: :fire:

rsync -a ~/Templates/ ~/Templates/
```

2. **Instalar o zsh e o Oh My Zsh**

```
# Instale o zsh :tada: :pirate:

sudo dnf install zsh

# Instale o Oh My Zsh :sparkles: :shield:

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

3. **Alterar o tema para agnoster**

```
# Abra o arquivo .zshrc :tada: :dog:

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo :sparkles: :magic_wand:

ZSH_THEME="agnoster"
```

4. **Instalar o plugin de autosuggestions**


# Abra o terminal :tada: :octopus:

zsh

# Instale o plugin de autosuggestions usando o Oh My Zsh :sparkles: :magic_wand:

git clone [https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions): [https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions

# Habilite o plugin :tada: :heart:

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo :sparkles: :magic_wand:

plugins=(... zsh-autosuggestions ...)


5. **Instalar o GH**

```
# Instale o GH :tada: :lightning:

sudo dnf install gh
```

6. **Mover o arquivo pacman**

```
# Mova o arquivo pacman para a pasta .config :tada: :dragon:

sudo mv ~/pacman ~/.config/
```

7. **Configurar o tamanho do terminal e o background transparente**

**Abra as preferências do terminal :tada: :cat::**

```
gnome-terminal --preferences
```

**Altere o tamanho do terminal para 110x30 :tada: :star:

```
Tamanho da janela: 110x30
```

**Ative o background transparente :sparkles: :sparkles:

```
Background transparente: Sim
```

**Salve as alterações.**

**Pronto! :tada: :partying_face:

**Print do terminal:**
![image](https://github.com/Gabrielcafens/ConfToLinux/assets/95833512/6ce714a6-aec4-412d-a8c4-2170e40c2f0b)


