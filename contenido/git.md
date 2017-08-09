![Git acaba con versiones finales](../assets/git/git.png)

Git es un **sistema de control de versiones** distribuido, gratuito y de c�digo abierto. Es decir, es un tipo de software pensando para hacer un seguimiento claro y ordenado de todos los cambios que vas haciendo en los archivos de un proyecto. Mejor todav�a, te permite hacerlo en equipo, de forma colaborativa.

Gracias al software de control de versiones, pod�s mantener tus archivos **organizados, coordinados y protegidos**, tanto de posibles eventos catastr�ficos como de los inevitables errores cometidos por tus compa�eros de equipo (y bueno, tambi�n de los tuyos); si eso sucede es f�cil solucionar el problema rescatando lo que haga falta de una versi�n anterior.

Git naci� en **2005**, despu�s de que se venga abajo la relaci�n entre la comunidad que desarrollaba el n�cleo de Linux y la compa��a responsable de BitKeeper, el sistema de control de versiones que ven�an usando hasta entonces. A estos muchachos (y en particular a Linus Torvalds, el creador de Linux) se les ocurri� que la mejor forma de reemplazarla era desarrollando una herramienta propia. Desde entonces Git ha logrado evolucionar manteniendo su **dise�o sencillo** y su tremenda **eficiencia**, incluso para manejar proyectos muy grandes.

### Lista comandos Git:

	git init
Indicamos que el directorio donde nos encontramos comenzar� a ser versionado bajo Git.

	git status
Vemos el estado actual de nuestra carpeta versionada as� como archivos que no est�n versionados, archivos modificados, archivos eliminados, etc. Los mensajes que podremos ver con este comando pueden ser los siguientes: 
Untracked files: nos mostrar� todos los archivos que no han sido agregados al "Stage"
Changes to be committed: nos indica qu� archivos ser�n agregados a nuestro commit.

	git add
Agrega los archivos que no est�n bajo versionamiento (los Untracked files que vimos anteriormente).

	git commit -m "mensaje"
Confirma los cambios hechos con "git add" en una nueva versi�n del proyecto; con el par�metro -m le indicamos un mensaje para describir la raz�n del commit.

	git remote add origin url_del_repositorio
Hasta ahora todos los comandos visto han sido puro trabajo local, con el comando git remote add agregamos nuestro repositorio a un servidor remoto; para hacerlo debemos tener ya creado nuestro repositorio en un servidor y este nos brindar� la url.

	git push -u origin master 
Empujamos todo lo que tengamos en nuestros commits al repositorio remoto.

	git pull
Trae los cambios que haya trabajado otra persona en el mismo repositorio, es recomendable siempre que trabajemos un repositorio que no hayamos iniciado nosotros hacer siempre un git pull primero antes de comenzar a trabajar en los archivos.

	git remote -v
Nos muestra la url remota del repositorio en el que nos encontremos.

	git clone url_del_repositorio nombre_local
Realiza una copia en nuestro directorio local de un repositorio existente.

	git branch -all
En Git se trabaja con branches (ramas en espa�ol), originalmente se crea la master por defecto, a ra�z de esto nosotros podemos crear nuestras propias ramas, siendo claro una copia de la master en primera instancia. Con este comando podemos ver todas las ramas que tenga el proyecto.

### Extras:

Presentaci�n hecha en Google -> [Git-Cheat Sheet](../assets/git/ppt/git-cheatSheet.pdf)

### Referencias:

La biblia -> [Progit](https://git-scm.com/book/es/v1)    
Link para favoritos-1 -> [Git - la gu�a sencilla](http://rogerdudler.github.io/git-guide/index.es.html)  
Link para favoritos-2 -> [Introducci�n a Github](http://www.cristalab.com/tutoriales/introduccion-a-github-en-linux-ubuntu-c106086l/)   