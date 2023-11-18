**Configurações de ambiente no Linux**

**Pré-requisitos**

* **Linux (Fedora 38) instalado** :computer:
* **Gerenciador de pacotes (dnf) instalado** :package:
* **Git instalado** :octopus:

**Passo a passo**

1. **Mover a pasta Templates**

```
# Mova a pasta Templates para a pasta home :house:

sudo mv ~/Templates/ ~/

# Faça o merge da pasta Templates com a já existente :recycle:

rsync -a ~/Templates/ ~/Templates/
```

2. **Instalar o zsh e o Oh My Zsh**

```
# Instale o zsh :shell:

sudo dnf install zsh

# Instale o Oh My Zsh :rainbow:

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

3. **Alterar o tema para agnoster**

```
# Abra o arquivo .zshrc :file_folder:

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo :heavy_check_mark:

ZSH_THEME="agnoster"
```

4. **Instalar o plugin de autosuggestions**



# Abra o terminal :computer:

zsh

# Instale o plugin de autosuggestions usando o Oh My Zsh :rainbow:

git clone [https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions

# Habilite o plugin :heavy_check_mark:

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo :heavy_check_mark:

plugins=(... zsh-autosuggestions ...)



5. **Instalar o GH**

```
# Instale o GH :octopus:

sudo dnf install gh
```

6. **Mover o arquivo pacman**

```
# Mova o arquivo pacman para a pasta .config :folder_open:

sudo mv ~/pacman ~/.config/
```

7. **Configurar o tamanho do terminal e o background transparente**

**Abra as preferências do terminal :computer::**

```
gnome-terminal --preferences
```

**Altere o tamanho do terminal para 110x30 :ruler:

```
Tamanho da janela: 110x30
```

**Ative o background transparente :eye:

```
Background transparente: Sim
```

**Salve as alterações.**

**Pronto! :heavy_check_mark:

**Print do terminal:**

![image](https://github.com/Gabrielcafens/ConfToLinux/assets/95833512/6c8f6cbd-8f29-400d-98da-42cc0ed3a57a)
