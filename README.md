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
````

# Cambiar la ruta home de Cygwin para que corresponda con la del usuario de Windows
buscar archivo nsswitch.con
Cambiar # db_home:  /home/%U  Añadir al final:  db_home:  /%H
