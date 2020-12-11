# Redis

## Definicion

Se podria definir redis como una gran tabla en memoria, donde se utiliza el metodo clave valor

## Intalacion

Para instalar redis en ubuntu se utiliza el siguiente comando

'''bash
sudo apt install redis-server redis-tools
'''

Esto instalara lo necesario para ejecutar el CLI.

## Acceder a Redis

Para Acceder a redis, se hara uso de la consola.

'''bash
redis-cli
'''

Acordarte de tener el servicio arriba de 'redis-server'

## Ping y Echo

'''bash
ping
'''

Es para hacer pings, este solo respondera "PONG" si se ejecuta solo

'''bash
echo 
'''

solo imprime en consola

## Guardando y leyendo

'''bash
set "hello" "world"
'''

Con lo anterior guardamos la clave "hello" y el valos es "world"

### Obtener un valor

'''bash
get hello
'''

### Guardando solo si la clave no existe

'''bash
set clave valor NX
'''

### Guardando solo si la clave existe

'''bash
set clave valor XX
'''

### Obtener todas las claves registradas

'''bash
keys *
'''

### Eliminar claves

'''bash
del nombre_clave
'''