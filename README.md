# Redis



## Definicion

Se podria definir redis como una gran tabla en memoria, donde se utiliza el metodo clave valor



## Intalacion

Para instalar redis en ubuntu se utiliza el siguiente comando

```bash
sudo apt install redis-server redis-tools
```

Esto instalara lo necesario para ejecutar el CLI.



## Acceder a Redis

Para Acceder a redis, se hara uso de la consola.

```bash
redis-cli
```

Acordarte de tener el servicio arriba de 'redis-server'



## Ping y Echo
Es para hacer pings, este solo respondera "PONG" si se ejecuta solo

```bash
ping
```

solo imprime en consola

```bash
echo 
```


## Guardando y leyendo

Con lo anterior guardamos la clave "hello" y el valos es "world"

```bash
set "hello" "world"
```


### Obtener un valor

150489```bash
get hello
```



### Guardando solo si la clave no existe

```bash
set clave valor NX
```

### Guardando solo si la clave existe

```bash
set clave valor XX
```

### Obtener todas las claves registradas

```bash
keys *
```

### Eliminar claves

```bash
del nombre_clave
```

### Borrar todos los datos

```bash
flushall
```



### Lanzar un comando varias veces

En el siguiente ejemplo imprimira 4 veces lo que tenga la clave "Hola" 

```bash
4 get hola
```


## Pedir ayuda de un comando 

La siguiente linea, dara ayuda del comando `set`

```bash
help set
```

## Escaneando claves

Es preferible usar `scan` que `keys`, sobre todo en produccion

```bash
scan 0 COUNT 3
```

## Bases de datos en Redis. Como crear diferentes namespaces?

Por defecto redis ofrece 16 base de datos, empieza en la 0. Para cambiar a otra base de datos se utiliza lo siguiente

```bash
select 1
```

# un Nuevo titulo
