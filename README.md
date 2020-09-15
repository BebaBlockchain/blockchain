# Blockchain Core Backend
Blockchain platform , beba platform powered by this code.


# PreRequisitos

Systema Windows 10
2 RAM Core i3 (Minimo)
Open PORT Configuration 

- Install Git
- Install Composer
- Install Node JS
- Install Babel 
- Install NodeMon

Otorgar PERMISOS Full a Carpeta del Nodo


# Uso Como Servidor Independiente 

- Clonar de https://github.com/ChrisQbit/Nodo-Maestro-Criptomoneda.git
- npm install

Si hay problemas en el comando anterior IMPORTANTE - borrar carpeta de node modules y correr de nuevo el comando - npm install

Si tenemos problemas con los comandos en CMD de Windows 
npm install --save-dev cross-env
2.2 - En el package json poner cross-env antes del HTTP_PORT

Una vez con todo componente instalado en el servidor accedemos via CMD (Command Line) a la ruta de nuestro nodo
example:
C:/ruta_al_nodo/MASTER_NODO/





# RUNNING NODE / CORRIENDO NODO MAESTRO
Para que el nodo comience a trabajar, Corremos el comando creado via YARN
/MASTER_NODO>yarn start

*****La consola mostrara lo siguiente y el NODO ESTA LISTO y en funcionamiento en el Puerto:3000
Service HTTP:3000 listening...
Service ws:5000 listening...
[ws:socket] connected.





# ABRIR WEBSOCKET / OPEN WEBSOCKET
Es posible agrehar websocket para conexion entre puntos de nodos, para abrir un websocket acceda a la consola a la ruta del NODO y ejecute el comando:
/MASTER_NODO>yarn start:2  


***$ cross-env HTTP_PORT=3001 P2P_PORT=5001 PEERS=ws:localhost:5000 babel-node ./service/index
Service HTTP:3001 listening...
Service ws:5001 listening...
[ws:socket] connected.
