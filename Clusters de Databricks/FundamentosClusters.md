# Fundamentos de clusters

Un cluster es una colección de maquinas virtuales. Normalmente hay un nodo controlaador que orquesta las tareas realizadas por cada maquina virtual.

## Tipos de clusters

- Cluster de todo proposito

Se crea a traves de una interfaz grafica. Son persistentes pueden ser reiniciados en cualquier momento. Son adecuados para analisis interactivo.

- Clusters de trabajo

Se crean cuando se necesita que este se ocupe en de un trabajo. No tiene presistencia, por lo general se termina cuando se termina el trabajo. Son adecuados para cargas de trabajo automatizado.

- Clusters de pool

Es un grupo de maquinas virtuales listas para usar, que permiten reducir los tiempos de arranque de los clusters y escalamiento automatico.

Basicamente son instancias de maquinas virtuales que están ya arrancadas y listas para ser asignadas a un cluster.

No se recomienda paralas cuentas de estudiante ya que cuestan mucho y probablemente no te permitan crear un cluster de este tipo.


## Politicas de un cluster

Las politicas son un conjunto de reglas que nos permiten ocultar o eliminar opciones de configuración. Además, nos permite fijar valores de configuración y restringir acceso a los usuarios.

Las politicas generalmente son creadas por un usuario administrador y son asignadas a un conjunto de usuarios. Lo que a largo plazo nos permite controlar costos haciendo que los usuarios creen objetos con determinadas caracteristicas.





