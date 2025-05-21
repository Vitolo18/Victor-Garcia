**¿Qué es un branch?**
Una rama paralela del código principal para trabajar sin afectar la versión estable.
	
**¿Por qué pueden ser útiles los branches?**
Permiten desarrollar nuevas funciones, arreglos o pruebas sin romper el código principal.

**¿Cómo se crea una branch?**
git branch nombre_rama

**¿Cómo se cambia a una branch?**	
git checkout nombre_rama

**¿Cómo se elimina una branch?**
git branch -D nombre_rama

**¿Cómo se crea una branch y se cambia a ella en un solo paso?**
git checkout -b nombre_rama

**¿Qué es un merge?**
Unir los cambios de una rama con otra (ej. integrar una función nueva a main).

**¿Cómo se realiza un merge?**
git merge nombre_rama

**¿Que es un tag?**
Un marcador para señalar un punto importante (como una versión).

**¿Cómo se crea un tag?**
git tag v1.0



Practico:

6.
muestra el historial de commits en forma de gráfico visual.

10.
se observa una nueva rama anana que se separa desde el último commit de la rama base.
El commit con el cambio en pizza.txt aparece en esta rama.

13.
Al ejecutar git graph, se muestra un nuevo punto en el historial que indica el commit donde se agregó la cebolla.

15.
se observa que las dos ramas se han unido en un solo historial,
mostrando un commit de merge que integra los cambios de la branch anana dentro de master.

16.
esta mergeada checkout

18.
se observa que la rama experimento se integra a main mediante un commit de merge. 

19.
Git hizo el merge automáticamente porque no hubo conflictos entre las ramas.

20.
checkout

23.
checkout esta mergeada a main