**�Qu� es un branch?**
Una rama paralela del c�digo principal para trabajar sin afectar la versi�n estable.
	
**�Por qu� pueden ser �tiles los branches?**
Permiten desarrollar nuevas funciones, arreglos o pruebas sin romper el c�digo principal.

**�C�mo se crea una branch?**
git branch nombre_rama

**�C�mo se cambia a una branch?**	
git checkout nombre_rama

**�C�mo se elimina una branch?**
git branch -D nombre_rama

**�C�mo se crea una branch y se cambia a ella en un solo paso?**
git checkout -b nombre_rama

**�Qu� es un merge?**
Unir los cambios de una rama con otra (ej. integrar una funci�n nueva a main).

**�C�mo se realiza un merge?**
git merge nombre_rama

**�Que es un tag?**
Un marcador para se�alar un punto importante (como una versi�n).

**�C�mo se crea un tag?**
git tag v1.0



Practico:

6.
muestra el historial de commits en forma de gr�fico visual.

10.
se observa una nueva rama anana que se separa desde el �ltimo commit de la rama base.
El commit con el cambio en pizza.txt aparece en esta rama.

13.
Al ejecutar git graph, se muestra un nuevo punto en el historial que indica el commit donde se agreg� la cebolla.

15.
se observa que las dos ramas se han unido en un solo historial,
mostrando un commit de merge que integra los cambios de la branch anana dentro de master.

16.
esta mergeada checkout

18.
se observa que la rama experimento se integra a main mediante un commit de merge. 

19.
Git hizo el merge autom�ticamente porque no hubo conflictos entre las ramas.

20.
checkout

23.
checkout esta mergeada a main