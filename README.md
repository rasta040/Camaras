# SlickMercy
TG: SlickMercy 

# Termux 
Descarga termux de F-Droid

# instalacion 

termux-setup-storage

pkg install python

pkg install python-pip

pkg install git

pkg update && pkg upgrade

pip install colorama

pip install aiohttp

pip install art

cd storage/downloads

git clone https://github.com/SlickxMercy/SlickMercy

# Ejecutar codigos 
python HostSlick.py
este sirve para escanear puertos y obtener una lista de host (recuerden guarda el archivo como host.txt)

python MercyScan.py
sirve para escanear la listas del archivo llamado host.txt y hace comprobaciónes de credenciales, cuando el acceso es correcto se guardan snapshots en la carpeta llamada pics 
en el nombre de la imagen encontras la ip, usuario y contraseña 

# Puerto 
pueden cambiar el puerto para obtener camaras de distintos puertos
modificando la linea;
async def check_camera(ip, usernames, passwords, port=80):

recuerda que también lo debes hacer en HostSlick.py 
en la linea:
sock.connect((ip, 80))
