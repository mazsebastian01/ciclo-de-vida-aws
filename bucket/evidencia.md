# Preguntas y respuestas

**1. ¿Por qué el nombre de tu bucket tuvo que ser distinto al de tus compañeros si cada uno tiene su propia cuenta?**

Porque los nombres de los buckets en AWS son únicos a nivel mundial. Eso significa que no se pueden repetir, aunque sean de cuentas diferentes.

**2. El usuario del paso 21 pudo leer un archivo, pero en el paso 22 no pudo ver la lista. ¿Qué acción le faltaba en la política?**

Le faltaba el permiso `s3:ListBucket`, que es el que permite ver la lista de archivos que hay dentro del bucket.

**3. En la política, ¿qué significa el `/*` al final del `Resource`? ¿Qué pasaría si se quitara?**

El `/*` indica que el permiso aplica a todos los archivos que están dentro del bucket. Si se quita, el recurso sería el bucket como tal y no los archivos que contiene.

**4. ¿En qué se diferencia compartir un archivo con un enlace temporal de hacer público el bucket?**

El enlace temporal permite acceder a un archivo específico durante un tiempo limitado. En cambio, hacer público el bucket puede permitir que otras personas accedan a los archivos sin esa limitación de tiempo, dependiendo de los permisos configurados.

**5. Según el modelo de responsabilidad compartida, si alguien deja un bucket público con datos de clientes, ¿de quién es la responsabilidad?**

La responsabilidad es del usuario o de la empresa que administra el bucket, porque debe configurar correctamente los permisos y proteger la información de sus clientes. AWS se encarga de la seguridad de su infraestructura.