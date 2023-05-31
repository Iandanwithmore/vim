# PERSONAL
## INSTALL DOCKER 
https://gitlab.com/bmcgonag/docker_installs
version: "3.8"
services:
  db:
    image: postgres:10.0
    container_name: pg10
    restart: always
    ports:
      - "5432:5432"
    environment:
      POSTGRES_USER: postgres
      POSTGRES_PASSWORD: postgres
      POSTGRES_DB: postgres
    volumes:
      - ./pg10_data:/var/lib/postgresql/data
  pgadmin:
    image: dpage/pgadmin4
    container_name: pgadmin4
    restart: always
    ports:
      - "5050:80"
    environment:
      PGADMIN_DEFAULT_EMAIL: pat@dev.corp
      PGADMIN_DEFAULT_PASSWORD: postgres
    volumes:
      - ./pgadmin_data:/var/lib/pgadmin

volumes:
  pg10_data:
  pgadmin_data:
  
## TMUX
https://github.com/tmux-plugins/tpm
## bluetooh fail
https://askubuntu.com/questions/1254404/ubuntu-20-04-lts-bluetooth-connection-failed
## vim base on 
https://www.freecodecamp.org/news/vimrc-configuration-guide-customize-your-vim-editor/
## pbcopy 
https://ostechnix.com/how-to-use-pbcopy-and-pbpaste-commands-on-linux/
## theme
https://github.com/catppuccin/gnome-terminal
## QMK 
keyboard YOU NEED TO RESTART
https://docs.qmk.fm/#/newbs_getting_started
# WORK
## VENTOY 
Use for Boot USB
## keys
https://keepassxc.org/download/#linux
## .ssh/config 
https://gist.github.com/rahularity/86da20fe3858e6b311de068201d279e3
### ARTATLAS     
```
Host github.com_artatlasperu
    HostName github.com
    User git
    IdentityFile ~/.ssh/github-artatlas-pat
  
#HOME
Host github.com_pat-devcorp
    HostName github.com
    User git
    IdentityFile ~/.ssh/github-pat-devcorp
```
