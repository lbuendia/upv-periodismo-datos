# Editores texto
- EMACS
- Notepad ++
- Sublime (Mac)

# Consolas
- Cygwin (Windows)
- Terminal (Mac) 

# Navegadores y buscadores seguros
- TOR: navegador 
- Startpage: buscador 
- Duckduckgo: buscador 

# Tener en cuenta
- Codificación de caracteres de cada programa. (UTF-8)
- Datos buleanos (si/no)
- XML: uno de los formatos de datos más usado. (KML: tipo de XML para geolocalizar datos)
- CSV: coma separated values. (también TSV, *SV cualquier cosa separada por valores). 
- JSON: para páginas web (javascript Object notation)
- School of data: recursos para formación <https://schoolofdata.org/> 
- Tres acentos al revés al inicio y al final para meter un bloque de texto.Por ejemplo: 

```
# /etc/nsswitch.conf
#
#    This file is read once by the first process in a Cygwin process tree.
#    To pick up changes, restart all Cygwin processes.  For a description
#    see https://cygwin.com/cygwin-ug-net/ntsec.html#ntsec-mapping-nsswitch
#
# Defaults:
# passwd:   files db
# group:    files db
# db_enum:  cache builtin
# db_home:  /home/%U
# db_shell: /bin/bash
# db_gecos: <empty>
db_home:  /%H
```

# Cambiar la ruta home de Cygwin para que corresponda con la del usuario de Windows
- buscar archivo nsswitch.con
- Cambiar # db_home:  /home/%U  Añadir al final:  db_home:  /%H

# COMANDOS CONSOLA

- **pwd** print working directory "Dime dónde estoy"
- **cd** change directory (si no pones el espacio te va directamente a la home)
- **ls** listar
- **ls -a** listar todo
- **ls -l** listar ordenadamente (te da info de los permisos de cada archivo read, write, execute)
- **git init**  inicializar para Git
- **cd ../** para subir a un directorio superior (mantener espacio)
- **clear** borrar la pantalla de la consola
- **mv** mover para cambiar nombre de archivo mv carpetaorigen/ capertadestino (todo lo que pongas delante serça origen y solo el último será destino)
- **mkdir** make directory
- **touch** crear archivo touch carpeta/nuevo.md
- **Q** quitar, salir
- **rm** borrar
- **rm -rf** forzar borrado 
Control A: ir al inicio de la línea
- **git status** para saber en qué punto te encuentras y qué has hecho
- **git add .** para añadir a la rama master todos los archivos
- **git clone url** clonar desde el repositorio. Para clonar todo desde Git en local. 
- **git pull** para descargarse desde GitHub en local
- **git push** para subir desde local al GitHub

**PARA CLONAR DESDE GITHUB A LOCAL** 
**git clone**

**PARA COPIAR LOS ARCHIVOS EN LOCAL EN GIT EN UN DIRECTORIO VACÍO DE GITHUB**
```
git init
git add README.md
git commit -m "primer commit"
git remote add origin https://github.com/tu_usuarix/nombre_proyecto.git
git push -u origin master
```

**PARA NAVEGAR EN ARCHIVOS CSV**
- **cat nombrearchivo.csv | wc -l**
- **cat** muéstramelo todo en bruto. 
- **wc-l** para saber el número de líneas de un archivo. (añadirlo al final del nombre del archivo)
- **head** muestra las 10 primeras líneas
- **tail** muestra las últimas 10 líneas 
- **tail -3** muestra las 3 últimas 
- **grep -rn** búsqueda de término en el archivo y por número de línea
- **> nombre.csv** para añadir todos esos resultados en un archivo nuevo con ese nombre y formato. 
- **>>* para sumar datos a un archivo. *grep -r Oriola archivo.csv >> elx.csv**
