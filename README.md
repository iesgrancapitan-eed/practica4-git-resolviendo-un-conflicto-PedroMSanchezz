# Practica 3 Resolviendo conflictos
1.Asegúrate de que tienes configurado el editor Visual Studio Code como tu editor de Git. (git config --global core.editor "code --wait")


2.Crea un repositorio local y avanza en la rama "master" añadiendo un fichero "index.html" con la estructura básica html. El body estará vacío

    - Se hace un touch index.html y se modifica el html para que no tenga nada en el cuerpo del body

3.Crea y salta a "rama-1". Avanza en un commit con tu nombre de pila en un párrafo dentro del body

    - Git checkout -b rama-1 (se modifica el index.html) git add . | git commit -m " " | git push origin rama-1

4.Vuelve a la rama master

    - Git switch main

5.Crea y salta a "rama-2". Avanza en un commit con tu apellido en un párrafo dentro del body

    - Git checkout -b rama-2 (se modifica el index.html) git add. | git commit -m " " | git push origin rama-2

6.Muestra el estado del repositorio de forma gráfica y resumida

    - Git log --graph

7.Haz un merge a rama-1. Intentas fusionar ambas ramas. Aparecerá un conflicto porque ambos commits trabajan en la misma porción <body></body> de un mismo archivo index.html. Git no será capaz de fusionarlas directamente. 


8.El editor VS Code reconoce los conflictos de fusión. Las diferencias se resaltan y hay acciones en línea para aceptar los cambios. Deja un único párrafo con tu nombre de pila y apellido.


9.Una vez que se resuelto el conflicto confirma el archivo en conflicto para que pueda realizar esos cambios


10.Muestra de nuevo el estado del repositorio de forma gráfica y resumida


11.Vuelve a la rama master y realiza otro merge. Es una fusión fast-forward. Los dos commits a fusionar tienen relación de ancestro. Entonces el merge no produce un commit nuevo, sencillamente avanza la rama, "avance rápido"


12.Visualiza las ramas que han sido fusionadas con la rama master


13.Elimina las ramas correctamente fusionadas (sin asterisco) para quedarte SOLO con la rama master. 


14.Realiza una copia a este repositorio remoto


15.Recuerda añadir estas instrucciones con los pantallazos en el fichero README.md


16.En GitHub entra en Insights/network y visualiza el gráfico del repositorio con los merge y cinco commits  
