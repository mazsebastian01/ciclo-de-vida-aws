# Preguntas de reflexión

### 1. ¿Qué podía hacer el usuario justo después de crearlo, antes de adjuntarle una política? ¿Por qué?

No podía hacer casi nada dentro de AWS, porque todavía no tenía permisos asignados. Para poder realizar acciones necesitaba que se le dieran permisos.

### 2. En el error del paso 13, ¿qué tres datos te dice el mensaje?

El mensaje indica qué usuario intentó hacer la acción, qué acción quiso realizar y por qué AWS no le permitió hacerla.

### 3. ¿Por qué cambió el ARN al renombrar el usuario?

Porque el ARN incluye el nombre del usuario. Al cambiarle el nombre, también cambia su ARN para que coincida con el nuevo nombre.

### 4. ¿Por qué AWS obliga a borrar las llaves antes de borrar el usuario?

Porque las llaves de acceso están relacionadas con ese usuario. Primero hay que eliminarlas para evitar que queden credenciales asociadas a una cuenta que ya no existe.

### 5. ¿Qué pasaría si le hubieras dado AdministratorAccess en vez de solo lectura? ¿En qué caso real estaría justificado?

El usuario tendría permisos para administrar prácticamente todos los servicios de AWS, no solamente consultar información. Esto sería útil para un administrador que necesite controlar toda la cuenta, pero no para alguien que solo necesita consultar datos.