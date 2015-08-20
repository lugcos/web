# Como agregar un post a la web del LugCOS

0) Activar nikola

```bash
cd nikola
source bin/activate
```

1) Asegurarse de tener la última versión de ambos repositorios

```bash
cd web
git pull
cd output
git pull
cd ..
```

2) Crear archivo para nuevo post

```bash
nikola new_post
```
(ingresar el título, primer letra en mayúscula, usar tildes)

Se crea el archivo `posts/titulo-del-post.rst`

3) Editar el archivo .rst con cualquier editor. Agregarle como segunda línea: 

```
.. author: Tu nombre o nick
```

(usar siempre el mismo nombre, mismas mayúsculas, mismos espacios)

3.1) Completar tags con etiquetas referentes a lo que se habla en el post. Ejemplo

```
.. tags: corriente, voltaje, resistencias
```

(separado por comas, dejando un espacio luego de los : y un espacio lueg de las comas)

3.2) Agregar el post a una categoría: puede ser Electrónica, Impresoras 3D, General, o alguna otra que inventemos. El nombre de la categoría siempre se debe escribir igual. Ejemplo:

```
.. category: Electrónica
```

3.3) Borrar `Write your post here.` y empezar a escribir ahí el post.

