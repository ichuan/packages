# tmux

## Example procedure

```bash
# (optional) dep libs
sudo apt-get install -y autogen automake libevent-dev libncurses5-dev

# download source
wget https://github.com/tmux/tmux/releases/download/2.9a/tmux-2.9a.tar.gz -O - | tar -xzf -

# compile
cd tmux-2.9a && ./configure && make

# make deb
sudo checkinstall
```
