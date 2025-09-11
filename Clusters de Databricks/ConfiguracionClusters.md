# Configuración de los clusters

## Single/Multi node

Dentro de databricks podemos configurar los clusters para que trabajen como un **multi node**, es decir, que habra un nodo controlador que es capaz de distribuir los trabajos entre nodos para distribuir la carga en paralelo. En este modo podemos escalar muy facilmente para trabajos que requieran mas poder computacional.

También tenemos el **single node**, solo tenemos un nodo que hace ambos roles de controlador y trabajador. No son escalables y por lo tanto no deberian ser utilizados para trabajos fuertes.

## Modo de acceso

- Single user: Solo un usuario puede acceder al cluster a traves de python, SQL, scala o R.

- Compartido: Permite que muchos usuarios puedan acceder. Este modo solo es utilizable por usuario premium. Es capaz de soportar Python o SQL.

- No insolation shared: Permite que muchos usuarios puedan utilizar el cluster, el problema es que no hay espacios ailsados, por lo que todos los usuarios podran ver todo el workspace sin restricciones. Soporta python, SQL, scala y R.

## Entorno de ejecución de databricks

Databricks proporciona 4 tipos de maneras de entorno de ejecución:

- Databricks runtime: Es una versión optimizada de apache spark library. Ofrece librerias java, scala, python y R. Librerias de GPY y librerias de Data Lake.

- Databricks runtime ML: Ofrece las librerias del runtime basico y otras de ML como Keras, XGBoost o TensorFlow.

- Photon runtime: Todo del runtime basico pero con el motor de photon.

- Runtime Light: Para tareas o trabajos que no necesitan mucho poder computacional.

## Terminación automatica

Se puede poner un tiempo temporizado para que los clusters se apaguen cuando no se utilicen despues de un tiempo.

## Escalamiento automatico

Se puede configurar el minimo y maximo de trabajadores. Databricks suele configurar por defecto un numero de trabajadores.



