Configuración zona

Para realizar la configuración de una nueva zona creamos un archivo llamado db.example.com. 
Rellenamos el archivo con los datos que queremos que tenga esta zona como el nameserver a utilizar su SOA y su ip. 
Una vez rellenado accedemos al archivo named.conf.local y añadimos el nombre de nuestra zona así como el tipo y el lugar del archivo de configuración de la zona.  
  
Para comprobar el funcionamiento de la zona primero reiniciamos el servicio de Bind9. 
Una vez reiniciado nos conectamos a nuestro contenedor cliente y realizamos un ping a nuestra dirección de la zona en mi caso example.com  
  
Si la zona funciona el resultado del ping debería devolver la ip que nosotros le asignamos. 
Para más compobaciones puede añadir a la zona un registro txt y realizamos un dig txt y nos debería devolver el registro.
