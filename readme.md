Pasos Para instalar en el server desde cero


#Primero se instala el nvm (Node Version Manager), y se configura la 20 por defecto
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
source ~/.bashrc
nvm install 20

#se clona el repósitorio dentro del directorio home preferiblemente, y se instalan los paquetes de node
cd /home
git clone https://github.com/armando19993/dashboar-control-transmision.git trasmision
cd trasmision
npm install

#para probar que ya esta en linea debes correr esto
node server.js 
acceder en el navegador al ip del servidor + puerto 3000

ipServer:3000

si te da este error
![Error posible](image.png)

entonces lo que debes es crear con el siguiente comando un archivo llamado channels.json

nano channels.json 

y dentro solo poner

[]

y vuelves a probar el ipServer:3000

![Servidor Funcionando](image-1.png)

solo prueba creando 1 canal y dando en iniciar
