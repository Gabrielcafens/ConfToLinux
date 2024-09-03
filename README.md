# Script de Automação para Configuração do Ambiente no Linux (Ubuntu)

Este script automatiza a configuração do ambiente no Linux (Ubuntu) com as seguintes ferramentas:
- Zsh e Oh My Zsh
- Git e GitHub CLI
- GitHub Desktop
- Configurações de terminal personalizadas

## Pré-requisitos
- Linux (Ubuntu) instalado :computer:
- Gerenciador de pacotes (dnf) instalado :package:
- Git instalado :octopus:

```bash
echo "Iniciando as configurações de ambiente no Linux..."
```
# Passo 1 - Mover Templates :house:
echo "Movendo a pasta Templates para a pasta home..."
```bash
sudo mv ~/Templates/ ~/
```
echo "Fazendo merge da pasta Templates..."
```bash
rsync -a ~/Templates/ ~/Templates/
```
# Passo 2 - Instalar Oh My Zsh :rainbow:
echo "Instalando o Zsh..."
```bash
sudo apt install zsh -y
```
echo "Instalando Oh My Zsh..."
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
# Passo 3 - Mudar tema :file_folder:
echo "Alterando tema do Zsh para agnoster..."

sed -i 's/ZSH_THEME=".*"/ZSH_THEME="agnoster"/' ~/.zshrc

# Passo 4 - Instalar Autosuggestions :rainbow:
echo "Instalando o plugin zsh-autosuggestions..."
```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/custom/plugins/zsh-autosuggestions
```
echo "Habilitando o plugin zsh-autosuggestions..."
sed -i 's/plugins=(/plugins=(zsh-autosuggestions /' ~/.zshrc

# Passo 5 - Instalar GitHub CLI :octopus:
echo "Instalando GitHub CLI (gh)..."
```bash
sudo apt install gh -y
```
# Passo 6 - Instalar GitHub Desktop :ruler:
echo "Instalando GitHub Desktop..."

# Obtenha a chave GPG e adicione o repositório do GitHub Desktop
wget -qO - https://apt.packages.shiftkey.dev/gpg.key | gpg --dearmor | sudo tee /usr/share/keyrings/shiftkey-packages.gpg > /dev/null
sudo sh -c 'echo "deb [arch=amd64 signed-by=/usr/share/keyrings/shiftkey-packages.gpg] https://apt.packages.shiftkey.dev/ubuntu/ any main" > /etc/apt/sources.list.d/shiftkey-packages.list'

# Atualize e instale o GitHub Desktop
```bash
sudo apt update && sudo apt install github-desktop -y
```
# Mova o arquivo pacman para a pasta .config :folder_open:
echo "Movendo o arquivo pacman para ~/.config..."
sudo mv ~/pacman ~/.config/

# Adicione ~/.config/pacman ao .zshrc
echo "Configurando pacman no Zsh..."
echo "source ~/.config/pacman" >> ~/.zshrc

# Passo 7 - Preferências de terminal :eye:
echo "Configurando preferências do terminal..."

# Conceda permissão de execução ao arquivo pacman
```bash
sudo chmod +x ~/.config/pacman 
```
# Configure o tamanho do terminal e o background transparente
gconftool-2 --set /apps/gnome-terminal/profiles/Default/use_custom_default_size --type bool true
gconftool-2 --set /apps/gnome-terminal/profiles/Default/default_size_columns --type int 110
gconftool-2 --set /apps/gnome-terminal/profiles/Default/default_size_rows --type int 30
gconftool-2 --set /apps/gnome-terminal/profiles/Default/use_custom_background --type bool true
gconftool-2 --set /apps/gnome-terminal/profiles/Default/background_darkness --type float 0.8

echo "Configurações aplicadas com sucesso! Reinicie o terminal para ver as mudanças."


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
           





