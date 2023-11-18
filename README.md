**Configurações de ambiente no Linux**

**Pré-requisitos**

* **Linux (Fedora 38) instalado** :computer:
* **Gerenciador de pacotes (dnf) instalado** :package:
* **Git instalado** :octopus:

**Passo a passo**

**Passo 1- Mover Templates :house:**

```
# Mover a pasta Templates para a pasta home 

sudo mv ~/Templates/ ~/

# Faça o merge da pasta Templates com a já existente :recycle:

rsync -a ~/Templates/ ~/Templates/
```

**Passo 2- Instalar Oh My Zsh :rainbow:**

```
# Instale o zsh :shell:

sudo dnf install zsh

# Instale o Oh My Zsh

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

**Passo 3- Mudar tema :file_folder:**

```
# Abra o arquivo .zshrc 

nano ~/.zshrc

# Adicione a seguinte linha ao final do arquivo :heavy_check_mark:

ZSH_THEME="agnoster"
```

**Passo 4- Instalar autosuggestions rainbow:**


Instale o plugin de autosuggestions usando o Oh My Zsh 

git clone [https://github.com/zsh-users/zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions

Habilite o plugin :heavy_check_mark:

nano ~/.zshrc

Adicione a seguinte linha ao final do arquivo :heavy_check_mark:

plugins=(... zsh-autosuggestions ...)


**Passo 5- Instalar gh :computer: :octopus:**

```
# Instale o GH 

sudo dnf install gh
```

**Passo 6- Mover o pacman :ruler:**

```
# Mova o arquivo pacman para a pasta .config :folder_open:

sudo mv ~/pacman ~/.config/
```

**Passo 7- Preferências de terminal :eye:**

```
# Configure o tamanho do terminal e o background transparente 

gnome-terminal --preferences

# Altere o tamanho do terminal para 110x30 

Tamanho da janela: 110x30

# Ative o background transparente 

Background transparente: Sim
```                         ___

                          ___
                      .-'   `'.
                     /         \
                     |         ;
                     |         |           ___.--,
            _.._     |0) = (0) |    _.---'`__.-( (_.
     __.--'`_.. '.__.\    '--. \_.-' ,.--'`     `""`
    ( ,.--'`   ',__ /./;   ;, '.__.'`    __
    _`) )  .---.__.' / |   |\   \__..--""  """--.,_
   `---' .'.''-._.-'`_./  /\ '.  \ _.--''````'''--._`-.__.'
         | |  .' _.-' |  |  \  \  '.               `----`
          \ \/ .'     \  \   '. '-._)
           \/ /        \  \    `=.__`'-.
           / /\         `) )    / / `"".`\
     , _.-'.'\ \        / /    ( (     / /
      `--'`   ) )    .-'.'      '.'.  | (
             (/`    ( (`          ) )  '-;    
            
  ( (                ( (                 ( (                
   ) )                ) )                 ) )               
.........           .........         .........           
|       |]         |       |]         |       |]                
\       /           \       /         \       /              
 `-----'             `-----'           `-----'  
           





