git config --global user.email albertozb96@gmail.com
git config --global user.name "J. Alberto Zapata"

git init
git add *
git commit

git remote add origin https://github.com/albertozb96/BookStack-Notes.git
git push --set-upstream origin master (las siguientes veces basta con git push)

con git commit -m y git ammend salen los comentarios de un commit normal ???

------------editar remotos-----------------

git remote -h
git remote
git remote -v
git remote rename <old> <new>
git remote set-url <name> <newurl>

-----------nomenclatura-------------

-- opciones de entrada
<> para parametros
[] para opcional, [<>] parametros opcionales
