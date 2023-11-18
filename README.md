**Configurações de ambiente no Linux :computer: :linux:**

**Pré-requisitos**

:computer: **Linux (Fedora 38)** instalado
:package: **Gerenciador de pacotes (dnf)** instalado
:git: **Git** instalado

**Passo a passo**

1. **Mover a pasta Templates :computer: :linux: :zsh: :git:**

```
# Mova a pasta Templates para a pasta home :computer: :linux:

sudo mv ~/Templates/ ~/

# Faça o merge da pasta Templates com a já existente :computer: :linux: :zsh: :git:**

rsync -a ~/Templates/ ~/Templates/
```

2. **Instalar o zsh e o OH MY ZSH :computer: :linux: :zsh:**

```
# Instale o zsh :computer: :linux:

sudo dnf install zsh

# Instale o OH MY ZSH :computer: :linux: :zsh:

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

3. **Alterar o tema para agnoster :computer: :zsh:**

```
# Abra o arquivo .zshrc :computer: :zsh:

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo :computer: :zsh:

ZSH_THEME="agnoster"
```

4. **Instalar o plugin de autosuggestions :computer: :zsh:**


# Abra o terminal :computer: :zsh:

zsh

# Instale o plugin de autosuggestions usando o Oh My ZSH :computer: :zsh:

git clone [https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions): [https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions

# Habilite o plugin :computer: :zsh:

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo :computer: :zsh:

plugins=(... zsh-autosuggestions ...)


5. **Instalar o GH :computer: :git:**

```
# Instale o GH :computer: :git:

sudo dnf install gh
```

6. **Mover o arquivo pacman :computer: :linux: :zsh: :git:**

```
# Mova o arquivo pacman para a pasta .config :computer: :linux: :zsh: :git:**

sudo mv ~/pacman ~/.config/
```

7. **Configurar o tamanho do terminal e o background transparente :computer: :terminal: :110x30: :transparent:**

**Abra as preferências do terminal:**

```
gnome-terminal --preferences
```

**Altere o tamanho do terminal para 110x30 :computer: :terminal: :110x30:**

```
Tamanho da janela: 110x30
```

**Ative o background transparente :computer: :terminal: :transparent:**

```
Background transparente: Sim
```

**Salve as alterações.**

**Pronto!:tada:**

**Print do terminal:**
![image](https://github.com/Gabrielcafens/ConfToLinux/assets/95833512/76287d0a-cab3-4d45-92dc-d8f8414c8394)


