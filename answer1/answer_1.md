# Ejercicio 1

Primero voy a crear el escenario para el ejercicio con:

Un replicaset:

![title](../images/hw1/replica.png)

Un service:

![title](../images/hw1/service.png)

Un ingress:

![title](../images/hw1/ingress.png)

Una vez tengo esto, he modificado mi fichero de host añadiendo que en localhost puede tener el DNS pau.students.lasalle.com

Una vez realizado este paso gracias al ingres controler podemos acceder a este host:

![title](../images/hw1/dns.png)

Para proporcionar el servicio HTTPS tenemos que crear un secret y pasarlo los certificados creados con OpenSSL:

![title](../images/hw1/secret.png)

Una vez tengo el secret, lo relaciono con el ingres

![title](../images/hw1/newingress.png)

Y ahora podemos acceder a https:
Validaremos que queremos entrar, y tendremos el contenido de nginx.

![title](../images/hw1/nosegura.png)

![title](../images/hw1/nginx.png)









