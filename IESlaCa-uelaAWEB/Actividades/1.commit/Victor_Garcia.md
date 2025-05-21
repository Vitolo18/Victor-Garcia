 **¿Cómo se inicializa un repositorio local? (que comando se debe ejecutar?)**
Inicia un repositorio Git en un directorio, permitiendo el control de versiones.

**¿Cómo hago para que un directorio deje de ser controlado por git? (que comando se debe ejecutar?)**
Elimina la carpeta oculta .git, quitando el control de versiones del directorio.

**Si agrego un archivo a un directorio que ya está siendo controlado por git, ¿está siendo controlado por git?**
No. Debes usar git add para que Git empiece a rastrearlo.

**¿Qué comando se utiliza para agregar un archivo al repositorio local?**
Agrega el archivo al área de preparación (staging), listo para ser confirmado (commit)

**¿Cómo determino que archivos fueron modificados? (que comando se debe ejecutar?)**
Muestra los archivos modificados, nuevos o eliminados que aún no han sido confirmados.

**¿Qué comando se utiliza para hacer un commit?**
Guarda los cambios preparados (staged) en el historial del repositorio con un mensaje.

**En sus propias palabras, ¿qué es un commit?**
Es un punto de guardado que registra los cambios hechos en los archivos hasta ese momento.




Practico:

3. que enseña git status: 
Rama actual.
Archivos nuevos no rastreados.
Archivos modificados sin agregar.
Archivos listos para commit.
Si no hay cambios, indica que todo está limpio.

5.
git add sandwich.txt → prepara el archivo para guardar.
git commit -m "mensaje" → guarda el cambio en el repositorio.
Sin el commit, los cambios solo están preparados pero no guardados.

7.
Después de ejecutar git commit -m "Agrego mi sandwich.txt",
la salida de git status cambia a que ya no muestra archivos listos para commit ni modificaciones pendientes.
Indica que el directorio está limpio porque los cambios fueron guardados en el repositorio.

9.
Lista todos los commits hechos en el repositorio.
Cada commit aparece con:
Su identificador único (hash).
El autor.
La fecha.
El mensaje del commit.
Aparecen del más reciente al más antiguo (orden cronológico inverso).

10.
10.1. git log --oneline
Muestra el historial de commits en una línea por cada commit.
Cada línea incluye un hash corto y el mensaje del commit.
Es una forma rápida y resumida de ver el historial.
10.2. git log --stat
Muestra cada commit con detalles de los archivos modificados.
Indica cuántas líneas fueron añadidas o eliminadas en cada archivo.
Da una idea clara de qué cambios específicos se hicieron en cada commit.

11
11. git diff
Muestra las diferencias entre archivos que han cambiado y la última versión confirmada (commit).
Indica qué líneas fueron añadidas, modificadas o eliminadas.
Es útil para ver exactamente qué cambiaste antes de hacer un commit.
11.1. git difftool --tool=meld <hash> (Windows)
Abre una herramienta visual llamada Meld para comparar los cambios.
Permite ver las diferencias de forma gráfica y más fácil de entender.
<hash> es el identificador de un commit específico con el que quieres comparar.
11.2. git difftool --tool=opendiff <hash> (Linux)
Similar a Meld, pero usa la herramienta gráfica OpenDiff.
Muestra las diferencias entre commits o archivos de forma visual.
También requiere el <hash> para saber con qué commit comparar.

14.
Cambios en git status después del commit:
Ya no aparecerán archivos modificados o renombrados porque el cambio está guardado.
El directorio enseña "working tree clean", indicando que todo está confirmado.

Cambios en git log --oneline después del commit:
Aparecerá un nuevo commit con un mensaje que describe el renombrado (si lo pusiste al hacer commit).
El commit más reciente será el que contiene el cambio de nombre del archivo.

15.
Cambios en git status después del commit:
No habrá archivos pendientes; el directorio estará limpio (working tree clean).
No mostrará el archivo eliminado porque el cambio ya fue guardado.

Cambios en git log --oneline después del commit:
Aparecerá un nuevo commit con el mensaje que describa la eliminación del archivo.
Ese commit será el más reciente en el historial.

16.
Git muestra qué archivos se modificaron.
También muestra cuántas líneas se agregaron o borraron.
Es útil para ver el impacto de cada commit en los archivos del proyecto.











