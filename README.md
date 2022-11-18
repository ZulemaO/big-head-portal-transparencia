# big-head-portal-transparencia
Proyecto para la Secretaría de Contraloría del Estado de Hidalgo para la Dirección General de Políticas de Transparencia y Anticorrupción. 

Manual Técnico para su despliegue en Windows 
1.	Requerimientos técnicos 
Es necesario para correr dicha aplicación los siguientes requerimientos técnicos ya instalados dentro servidor/equipo dependiendo el sistema operativo para el sistema: 
•	Node.js en su última versión. (Preferentemente la versión '18.12.1'). 
•	NPM en su ultima versión. (Preferentemente la versión '8.19.2'). 
•	MongoDB Compass en su ultima versión.  (Preferentemente la versión 
'1.33.1'). 
•	Consola de comando de preferencia (Preferentemente Windows Powershell actualizada). 
•	IDE de preferencia (Visual Studio Code , configurado en js, actualziado). 
 
2.	Clonar repositorio 
Clonar el repositorio de Github: https://github.com/TheGeneralisimo/big-headportal-transparencia 
  
3.	Configuración de big-head en Node.js 
Dentro de la consola de uso de node.js o cualquier consola de desarrollo, instalar el siguiente recurso npm con el comando: “npm i big-head” 
  
4.	Configuración de URI MongoDBCompass 
Dentro del panel de administración de MongoDBCompass realizar una conexión con el siguiente URI: 
“mongodb+srv://admin:contraloria2022@cluster0.rrkgbin.mongodb.net/?retryWrites =true&w=majority” 
Donde se alberga la base de datos en un cluster en línea.  
  
En caso de existir un error en la conexión del cluster, se proporciona el usuario:admin y las password:contraloria2022 
 
5.	Configuración de base de datos MongoDBCompass 
Dentro del repositorio “big-head-portal-transparencia” está presente en documento JSON los registros de ruta de información en el archivo “data.json” que debe ser cargado tras la conexión exitosa dentro de la base de Mongo. 
  
 
6.	Documentación de big-head 
Dicho proyecto se basa en el paquete big-head para la creación de un panel de control de información. Favor de visualizar en el sitio https://www.npmjs.com/package/big-head para mayor documentación.  
  
7.	Configuración de apied_piper_server  
En caso de algún error, duda, favor de revisar la documentación en el sitio https://www.npmjs.com/package/big-head para mayor documentación. 
Dentro del portafolio “apied_piper_server” entrar a la carpeta “\big-head-portaltransparencia\apied_piper_server\config” , y seleccionar el archivo “global.config” para realizar las configuraciones correspondientes al uso del puerto establecido por el backend del api. Al igual que usuarios de administradores, creación de usuarios, cambio de servidores de bases de datos.  
  
8.	Configuración de console (big-head console)  
En caso de algún error, duda, favor de revisar la documentación en el sitio https://www.npmjs.com/package/big-head para mayor documentación. 
Dentro 	del 	portafolio 	“console” 	entrar 	a 	la 	carpeta 	“\big-head-portal-
transparencia\console\config” , y seleccionar el archivo “global.config” para realizar las configuraciones correspondientes al uso del puerto establecido por el frontend del panel.  
  
9.	Despliegue de apied_piper_server 
En caso de algún error, duda, favor de revisar la documentación en el sitio https://www.npmjs.com/package/big-head para mayor documentación. 
Dentro de la carpeta “apied_piper_server” ya configurada, se debe ejecutar desde terminal el comando “npm start”. En caso de existencia de algún error dentro de la actualización de los “node_modules” favor de eliminar la carpeta “node_modules” ya configurada al igual que el archivo “package.lock.json”; posteriormente debe ejecutar la reinstalación de las dependencias con el comando “npm install” 
10.	Despliegue de console 
En caso de algún error, duda, favor de revisar la documentación en el sitio https://www.npmjs.com/package/big-head para mayor documentación. 
Dentro de la carpeta “console” ya configurada y el server apied_piper_server corriendo, se debe ejecutar desde terminal el comando “npm start”. En caso de existencia de algún error dentro de la actualización de los “node_modules” favor de eliminar la carpeta “node_modules” ya configurada al igual que el archivo “package.lock.json”; posteriormente debe ejecutar la reinstalación de las dependencias con el comando “npm install” 
 
