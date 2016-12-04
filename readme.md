# Respuestas a la práctica de Git

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

```python
git reset --hard HEAD~1
```

Para volver al paso anterior moviendo tanto el **HEAD** como la rama y con **--hard**
para deshacer también nuestro **working copy**.


- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

```python
git reflog
git reset --hard bb52517
```

Se hizo un **reflog** para localizar el commit donde queremos regresar. Posteriormente, se ha usado el **reset --hard** para rehacer lo deshecho y obtener en nuestro **working copy** los datos que teníamos.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

```python
git merge master
```

No causó conflicto porque los nodos estaban en forma de lista por lo que se pudo hacer bien el merge y absorber los cambios de una rama a otra, cambiando así el puntero.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

```python
git checkout styled
git merge htmlify
```

Esta vez si que hay conflicto porque Git detecta que hay cambios en dos ramas diferentes para el mismo archivo y además no se encuentran en formato lista por lo que no puede hacer el merge. Hay que resolver el conflicto de manera manual y aplicar los cambios.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

```python
git checkout master  
git merge styled
```

En este caso no causó conficto porque ya indicamos a Git con que nos queríamos quedar por lo que se hizo un commit donde se indicó que era lo correcto por lo que ambas ramas están en el mismo punto con el conflicto resuelto. Master puede absorber los cambios de styled porque se encontraría en el caso lista.

- ¿Qué comando o comandos utilizaste en el paso 25?

```python
git log --graph --decorate --pretty=oneline
```

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

Si que se podría hacer fast-forward aunque se haya hecho de otro modo porque en este caso las ramas se encuentran en modo lista y podría absorber los cambios sin problema.


- ¿Qué comando o comandos utilizaste en el paso 27?

```python
git reset HEAD~1
```

- ¿Qué comando o comandos utilizaste en el paso 28?

```python
git checkout -- git-nuestro.md
```

- ¿Qué comando o comandos utilizaste en el paso 29?

```python
git branch -D title
```

- ¿Qué comando o comandos utilizaste en el paso 30?

```python
git reset --hard f7cd3dc
```

- ¿Qué comando o comandos usaste en el paso 32?

```python
git checkout 2369635
```

- ¿Qué comando o comandos usaste en el punto 33?

```python
git checkout bfff6c0
```
