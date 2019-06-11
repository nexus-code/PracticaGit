- �Qu� comando utilizaste en el paso 11? �Por qu�?

	Utilizo git reset --hard HEAD~1 El comando --hard sobreescribe el contenido del working copy actual con el contenido del repositorio,
					provocando la perdida de los cambios realizados en el mismo (por el punto 9). 
					El comando HEAD~1 indica que el comit a recuperar es el anterior al �ltimo.



- �Qu� comando o comandos utilizaste en el paso 12? �Por qu�?
	
	git reflog			Para visualizar el log de commits y obtener sus identificadores hash (9c9dd30).
	git reset --hard 9c9dd30	Para ejecutar las instrucciones del punto 12 llamando al comit indicado.
	


- El merge del paso 13, �Caus� alg�n conflicto? �Por qu�?

	No ha habido conflicto, se han adaptado los cambios entre "versiones".


- El merge del paso 19, �Caus� alg�n conflicto? �Por qu�?

	Ha habido conflicto entre los ficheros de ambas ramas porque son "versiones" distintas y tienen modificaciones en las mismas l�neas.


- El merge del paso 21, �Caus� alg�n conflicto? �Por qu�?

	No ha habido conflicto, o m�s bien ha sido resuelto autom�ticamente, porque el fichero de styled es evoluci�n directa del que se encuentra en master.


- �Qu� comando o comandos utilizaste en el paso 25?

	git log --graph --decorate


- El merge del paso 26, �Podr�a ser fast forward? �Por qu�?

	Si, porque los cambios realizados sobre el fichero en title no crean conflico con el contenido del mismo en master: Se han a�adido nuevas filas.


- �Qu� comando o comandos utilizaste en el paso 27?

	git reset HEAD~1


- �Qu� comando o comandos utilizaste en el paso 28?
	
	git checkout -- git-nuestro.txt


- �Qu� comando o comandos utilizaste en el paso 29?

	git branch -D title


- �Qu� comando o comandos utilizaste en el paso 30?

	git reflog 				Para encontrar el nodo donde se hizo el merge
	git reset a dicho nodo
	git checkout -- git-nuestro.txt		Para descartar los cambios realizados y volver el fichero al estado del commit anterior.

	
- �Qu� comando o comandos usaste en el paso 32?

	git reflog 				Para encontrar el hash de dicho commit
	git reset --hard a dicho commit
	
- �Qu� comando o comandos usaste en el punto 33?
	
	git reflog 				Para encontrar el hash de dicho commit
	git reset --hard a dicho commit