
## MANUAL
clone to the repository
```bash
 git clone git clone "https://github.com/parthivkumarnikku/terminal.git" && cd terminal
```
copy the file to your required directory
```bash
cp custom_zsh_prompt.sh ~/.custom_zsh_prompt.sh
```
Install oh-my-zsh
```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

```
After installation, add the following plugins in the ~/.zshrc file to enhance autocompletion:
```bash
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)

```
Add the following lines to your .zshrc file:
```bash
# Enable command auto-completion
autoload -U compinit
compinit
```
- Make sure to install the zsh-autosuggestions and zsh-syntax-highlighting plugins if you haven't done so
Install zsh-autosuggestions:
```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.zsh/zsh-autosuggestions
echo "source ~/.zsh/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ~/.zshrc

```
Install zsh-syntax-highlighting:
```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.zsh/zsh-syntax-highlighting
echo "source ~/.zsh/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc

```
add the following line to your native ~/.zshrc
```bash
echo "source /home/${USER}/.custom_zsh_prompt.sh" >> ~/.zshrc
```
Apply changes

```bash
source ~/.zshrc

```
