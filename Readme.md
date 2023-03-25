# LABORATORIO 7
## Integrantes
* Santiago Arévalo Rojas
* Juan Felipe Sánchez Pérez  

## Finalización CI/CD - Manejo de Data - ORM
## PARTE I. FINALIZACIÓN CI/CD
### Verificación App  
Iniciando el servicio y dirigiendonos a nuestra URL:  
<img src="https://user-images.githubusercontent.com/123812331/226107091-1dc8a35e-b730-47ee-9d93-cdb80d3ed805.png" width="60%" height="60%"/>  

### Troubleshooting - Activando logs  
Primero, luego de activar el servicio  y antes de ingresar a logs stream (secuencia de registro), nos indican que debemos activar los logs:
<img src="https://user-images.githubusercontent.com/123812331/226107762-89bdfcf7-40fb-43bd-a1fd-529e64a81071.png" width="60%" height="60%"/>  

Para ello, vamos a App Service Logs (Registros de App Service) y configuramos las siguientes opciones como se muestra em la imagen. Luego guardamos.  
<img src="https://user-images.githubusercontent.com/123812331/226108017-01f13452-d8d4-45bd-b2aa-0c162bcbd860.png" width="60%" height="60%"/>  
 
Al revisar los logs en log stream (secuencia de registros) se evidencian los posibles errores al intentar hacer login:  
<img src="https://user-images.githubusercontent.com/123812331/226108477-5281f5c5-1629-44cc-84bb-47bd9612634f.png" width="60%" height="60%"/>    

Clonamos el proyecto MyShuttle desde Azure DevOps:  
<img src="https://user-images.githubusercontent.com/123812331/226108741-5600c27b-2cd1-43ee-9455-4599ffa3d99d.png" width="60%" height="60%"/>    
Ingresamos con el correo electrónico de la universidad, y se clona el proyecto exitosamente.

### Continuous Integration - Activando la opción integración continua en el Pipeline.  
Editar el pipeline de nuestro proyecto, y en la opción "Triggers" activar la opción de integración continua:  
<img src="https://user-images.githubusercontent.com/123812331/226109140-a07e1e73-b170-42a7-90ac-30185668f51c.png" width="60%" height="60%"/>    

Ahora, en el menú de releases, creamos uno nuevo:
<img src="https://user-images.githubusercontent.com/123812331/226109384-a1905922-7039-46e7-8635-457411b217d2.png" width="60%" height="60%"/>

### Bugfixing - Solucionando un Bug  
El error lo vemos en las propiedades de la clase Data Access, así que ingresamos los datos correctos:  
<img src="https://user-images.githubusercontent.com/123812331/227722129-6057c377-0ca8-43de-857a-2d8bddae5f89.png" width="60%" height="60%"/>

Luego de subir los cambios al reopositorio remoto, en el portal de Azure, nos dirigimos a la aplicación web, configuraciones, y en la cadena de conexión creada, modificamos el valor, estableciendo en "falso" el uso de SSL.   
<img src="https://user-images.githubusercontent.com/123812331/227722352-f3115871-599b-48c0-8b8c-c466dc66d6eb.png" width="60%" height="60%"/>



