# Accesos seguros a databricks

## Databricks secret scopes

Ayuda a guardar credenciales de una forma segura y referenciadas a cuadernos, clusters o jobs. Es un servicio ofrecido por databricks

## Como implementarlo

Necesitamos añadir secretos a una key vault de Azure, luego creamos un secret scope de databricks y luego los referenciamos a un objeto, como un cluster o un nootbook.

### Creando un Azure Key Vault

![alt text](keyvault.png)

Creamos este nuevo recurso en Azure.

![alt text](conf.png)

Configuramos la key vault que se utilizara. Luego le damos a revisar y crear.

![alt text](secretos.png)

Nos vamos a la sección de secretos.

![alt text](confsecre.png)

Configuramos el secreto, el valor secreto fue el generado como token en la cuenta de almacenamiento *ver DataLakes (GestionUsoDatalakes.md)*

### Creando secret scope en databricks

Para encontrar el secret scope debemos escribir desde el home page en la url lo siguiente despues del url predeterminado

![alt text](url.png)

Luego podemos crear el secret scope aqui 

![alt text](secret.png)

Ahí nos pedira algunos datos que necesitamos como el dns name y el id del recurso, los podemos encontrar en properties en el recurso 

![alt text](propie.png)





