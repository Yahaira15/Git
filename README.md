# GIT Y GITHUB
---

### ¿QUÉ ES GIT?
Git es un sistema de control de versiones que nos ayuda a llevar un registro sobre el historial de cambios que se le hacen a los proyectos ademas de que se permite a los desarrolladores colaborar en proyectos 

![git](/img/git.png)

### TERMINOLOGÍA
- **Repositorio:** Es todo proyecto que ya tiene un segumiento por git, es decir que ya tiene un historial en el que se estan registrando sus cambios 
- **Commit:** Un commit es cada uno de los cambios registrados en el historial de git, estos cambios se deben enviar y justificarse 
- **Ramas:** Son ramificaciones que toma el proyecto para hacer correciones o alguna caracteristica nueva, esta es una copia exacta del proyecto y se trabaja en un ambiente aislado para no causar daños al proyecto principal. Tenemos la rama principal que se le llama ***master***, donde se encuentra el proyecto 
- **Clon:** Es una copia exacta del repositorio, todos los miembros del equipo al iniciar clonan el repositorio en su equipo
- **Fork:** Es un proyecto completamente diferente que se crea a partir de otro, o sea se basó en lo que habia trabajado el otro proyecto   
    
### CARACTERISTICAS
1. Git es *distribuido*, esto significa que cada desarrollador tiene una copia identica dek repositorio, incluyendo todo el historial 
2. Como vimos anteriormente las *ramas* son nuevos caminos que toma el proyecto para no afectar a la rama principal, pero sus ramas deben *fusionarse*, o sea debe integrarse de nuevo con la rama principal 
3. Git maneja la *integridad de datos* con un checksum (una suma de comprobación a cada uno de los archivos y los commit de tal manera hay seguridad total)

> ### HISTORIA
> La historia de Git es un tanto curiosa, en el año 2005 el creador de Linux, 'Linus Torvalds', crea Git a partir de una necesidad.  
> Minetras se desarrollaba LInux, una comunidad bastante grande daba sus aportes para el desarrollo de Linux, 
> para manejar e integrar todos estos aportes se manejaba el sistema de control de versiones Bitkeeper, 
>sin embargo este mismo dejo de ser gratuito y LInus no quería pagar por la licencia porque linux es un proyecto open source, 
>así que decidio crear su propio sitema de control de versiones al que llamo Git, su segundo proyecto mas grande
>

#### Equipo: 
Cuando se trabaja en quipo tenemos dos ramas, una llamada *Master* (el proyecto principal) y *Dev*

---
### PRINCIPALES COMANDOS DE GIT 

- ***git init*** -> Se utiliza para crear un repositorio, se empieza desde cero
- ***git clone*** -> Se utiliza para clonar un repositorio ya existente, este crea una copia en el equipo
- ***git add*** -> Se utiliza para preparar los cambios en el directorio actual y sus subdirectorios
- ***git commit*** -> Se utiliza para confirmar los cambios preparados con un mensaje de confirmación
- ***git push*** -> Se utiliza para enviar los cambios locales a un repositorio remoto
- ***git pull*** -> Se utiliza para descargar los cambios de un repositorio temoto y los fusiona con el repositorio local
- ***git remote*** -> Agrega un repositorio remoto y permite ver y eliminar conexiones con otros repositorios 
- ***git branch*** -> Se utiliza para gestionar las ramas, permite crear, listar, renombrar y eliminar ramas 
- ***git fetch*** -> Recupera los datos mas recientes de un repositorio repositorio remoto, pero no integra ninguno de estos datos nuevos en los archivos de trabajo
- ***git checkout*** -> Se utiliza para ccambiar a la rama especificada 
- ***git merge*** -> Se utiliza para fusionar la rama especificada con la rama actual
- ***git status*** -> Se utiliza para mostrar el estado del repositorio, incluidos los cambios no confirmados
- ***git reset*** -> Se utiliza para restablecer la rama actual al *commit* epspecificado

---

### PASO A PASO PARA ENVIAR CAMBIOS 
1. Verifica el estado del repo
```
git status
```

2. Agregar los cambios

Agregar todos los cambios
```
git add .
```
O agregar un archivo específico
```
git add nombre_archivo
```

3. Confirmar los cambios (commit)
```
git commit -m "Descripción clara de los cambios"
```

5. Sube los cambios a GitHub (push)

Rama principal (master)
```
git push origin master
```
Rama principal (main)
```
git push origin main
```

# Pongamoslo en practica!!

Primero abriremos nuestra terminal con la carpeta que queremos subir (Hay que fijarse que este en GitBash)

![git](/img/Paso1.png)

Segundo, vamos a digitar el comienzo de nuestra iteracion

![git](/img/Paso2.png)

Ahora añadiremos los acrhivos que queremos subir, con el nombre del archivo o si queremos subir todo el contenido de nuestra carpeta. En nuestro caso vamos a subir el archivo de nuestra carpeta 

![git](/img/Paso3.png)

Siguiendo la ruta para poder subir nuestro repositorio, git nos pide hacer un commit siempre que hagamos algo nuevo en el repositorio 

![git](/img/Paso4.png)

Ya para hacer el cargue a nuestro repositorio en GitHub, solo tenemos que agregar un comando para que sepa dónde se debe subir 

![git](/img/Paso5.png)

Y por ultimo hacemos el push que por fin nos mostrara nuestro repositorio con todos los archivos de nuestro equipo local

![git](/img/Paso6.png)


``` 
Por ultimo, vamos a tener en cuenta una información muy importante que nos servirá en un futuro y es poder cambiar el nombre a la rama que estamos usando "git branch -M main"
```