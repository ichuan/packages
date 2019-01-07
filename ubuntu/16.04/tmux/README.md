# tmux

## Example procedure

```bash
# (optional) dep libs
sudo apt-get install -y autogen automake libevent-dev libncurses5-dev

# download source
wget https://github.com/tmux/tmux/releases/download/2.8/tmux-2.8.tar.gz -O - | tar -xzf -

# compile
cd tmux-2.8 && ./configure && make

# make deb
sudo checkinstall
```
