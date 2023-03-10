#### Ver la dirección en la que estamos trabajando actualmente
```
pwd 
```

#### Te sirve para movernos de carpeta en carpeta en nuestro sistema operativo
```
cd
```

#### Nos sirve para devolvernos al directorio padre
```
cd ..
```

#### Abrir archivos de windows (desde wsl)
```
cd mnt
```

#### Nos sirve para ver los archivos, enlaces o directorios, que se encuentran dentro del directorio
```
ls
```

#### Lista para ver los archivos, enlaces o directorios en formato largo
```
ls -l
```

#### Nos sirve para ver los archivos, Nos muestra todo, incluso los ocultos.
```
ls -la
```

#### Los ordena por tamaño
```
ls -lS
```

#### Los ordena por tamaño y nos dice cuanto pesan en kb , mb, gb
```
ls -lSh
```

#### Los muestra en reversa.
```
ls -lr
```

#### Permisos de administrador
```
sudo
```

#### Crear una nueva carpeta, separa con espacion para crear mas de 1
```
mkdir
```

#### Crear archivos, separa con espacios para crear mas de 1
```
touch
```

#### Para copiar archivos 

```
  cp
```

#### Mover archivos/carpetas
```
mv
```

#### Abrir un archivo en VSCode
```
code . 
```

#### Nos permite borrar un archivo (por ejemplo, rm archivo.txt). Mucho cuidado con este comando, puedes borrar todo tu disco duro.

```
rm
```

#### Nos permite borrar una carpeta con el contenido. -i indica un mensaje de confirmación en consola para tener mas control sobre la elección de que archivos queremos eliminar.

```
rm -i nombredelacarpeta
```



#### Nos permite borrar una carpeta con el contenido.
```
rm -r nombredelacarpeta
```

#### Comando que borra una carpeta vacía.
```
rm -d nombredelacarpetavacia
```

#### Comando que borra un directorio con un contenido adentro de manera forzada (f).
```
rm -rf nombrededirectorio
```


#### Ver el contenido de un archivo (por ejemplo, cat nombre-archivo.txt).
```
cat
```

#### Este comando muestra un manual de uso de lo que se ponga consiguinete a él.
 ```
man cat
```

#### ir al inicio de ubuntu 
```
 cd ~
```

#### Comando para preguntarle al repositorio de dependencias si hay actualizaciones.
```
 sudo apt-get updade
```

#### Con este se aplican las actualizaciones. Se recomienda hacerlo habitualmente.
```
 sudo apt-get upgrade
```

#### Para ver tree, el contenido en modo arbol 
```
 tree
```

#### Para calcular los niveles que se mostraran con tree, el contenido en modo arbol 
```
 tree -L (cantidad de niveles)
```

#### Para instalar tree y ver el contenido en modo arbol 
```
  sudo apt-get install tree
```

#### Para ver versión de tree instalado 
```
  tree --version 
```

# Explorando el contenido de nuestros archivos

#### Nos muestra las primeras 10 líneas de un archivo de texto.

```
  head <documento de texto> 
```


#### Nos muestra las primeras líneas de un archivo de texto que le indiquemos.

```
  head -n <numero de lineas> <documento de texto> 
```


#### Nos muestra las ultimas 10 líneas de un archivo de texto.

```
  tail <documento>
```


#### Nos muestra las ultimas líneas de un archivo de texto que le indiquemos.

```
  tail <documento de texto> -n <numero de lineas> 
```


#### Observar todo el contenido usando el comando Less

```
 less [nombreDelArchivoParaAbrir]
```

<p>
Ahora tendrás una especie de interfaz gráfica donde podrás inspeccionar el documento. Puedes usar las flechas y el scroll para moverte arriba y abajo.

Además, puedes buscar palabras dentro del documento. Si presionas la tecla slash “/”, en la parte de abajo se habilitará un cuadro donde podrás buscar palabras, solo escribe y presiona enter.
</p>

<p>
  Para salir de la interfaz presiona “q”.
 </p>


#### Para abrir un archivo desde la terminal. Usa las aplicaciones predeterminadas.

```
  xdg-open <archivo>
```

#### Para abrir un archivo desde la terminal. Usa las aplicaciones predeterminadas.
```
  xdg-open <archivo>
```

#### Para abrir un archivo desde la terminal en visual studio code (hacerlo estando en el directorio que deseamos abrir)
```
  code .
```

#### Para abrir alguna carpeta de archivos (hacerlo estando en la carpeta que deseamos abrir)
```
  nautilus
```

# Comandos


#### Nos permite conocer que tipo de comando es 🤔.
```
  type <comando>
```

#### Nos permite crear comandos. Son temporales, se borran al cerrar la terminal 👶🏼.
```
  alias l="<secuencia de comandos>"
```

#### Nos permite consultar un poco de documentación de un comando 📄.
```
  help <comando>
```

####  De manual, nos permite conocer mucha mas información de un comando.
```
  man <comando>
```


####  Similar al anterior, pero un poco resumido y con otro formato.
```
  info <comando>
```

####  Describe un comando en una sola línea ☺️. No funciona con todos.
```
  whatis <comando>
```

# Wildcards

<p>
El asterisco * significa cualquier STRING o cadena de texto, entonces si ponemos ls *.txt cualquier archivo .txt se listará.
</p>

#### Listar todos los archivos que tengan extensión .txt, independientemente del nombre que tengan.
```
  ls *.txt
```


#### Listar todos los archivos que inicien con la palabra “datos”, independientemente de cómo siga el nombre o la extensión que tenga.
```
  ls datos*
```

#### Listar todos los archivos que inicien con la palabra “datos” y solamente tengan un caracter más luego de esa palabra.
```
  ls datos?
```

#### Listar todos los archivos que inicien con la palabra “datos” y solamente tengan tres caracteres más luego de esa palabra.
```
  ls datos???
```


#### Listar todos los archivos que inicien con una mayúscula, independientemente de cómo siga el nombre o la extensión que tenga.
```
  ls [[:upper:]]*
```


#### Listar todos los DIRECTORIOS que inicien con una mayúscula, independientemente de cómo siga el nombre que tenga.
```
  ls -d [[:upper:]]*
```


#### Listar todos los DIRECTORIOS que inicien con una minúscula, independientemente de cómo siga el nombre o la extensión que tenga.
```
  ls [[:lower:]]*
```

####  Listar todos los archivos que inicien con la letra “a” o con la letra “d”, independientemente de cómo siga el nombre o la extensión que tenga.
```
  ls [ad]*
```






