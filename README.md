#### Forked from https://github.com/bsord/tetris

## Getting Started
Running the game:
### Prebuilt Docker image (not easily editable)
```sh
docker run -d -p 80:80 --name tetris timothepoznanski/tetris
```
### Nginx Docker with volume mounts (easily edit)
```sh
mkdir ~/tetris
cd ~/tetris
git clone https://github.com/timothepoznanski/tetris .
docker run --name tetris -v /home/YOURUSERNAME/tetris/:/usr/share/nginx/html:ro -d -p 88:80 nginx
```

### Standalone Local
```sh
mkdir ~/tetris
cd ~/tetris
git clone https://github.com/timothepoznanski/tetris .
sudo cp * /usr/share/nginx/html
```
Once downloaded and place in a web server directory, open it in your browser

