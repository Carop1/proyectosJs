# Taller Alias 

## 1.

git log --graph --oneline --all

Este comando utiliza las siguientes opciones:

- `--graph`: Muestra el historial de commits en forma de gráfico ASCII.
- `--oneline`: Muestra cada commit en una sola línea para hacer el gráfico más compacto.
- `--all`: Muestra todos los commits de todas las ramas.

Resultado:

![image-20240206181931571](C:\Users\USUARIO\AppData\Roaming\Typora\typora-user-images\image-20240206181931571.png)

## 2.

git log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%ar)%Creset %C(bold blue)<%an>%Creset' --abbrev-commit --all

- `%Cred%h%Creset`: Muestra el hash corto del commit en color rojo.
- `-%C(yellow)%d%Creset`: Muestra las referencias (ramas o tags) en las que está involucrado el commit en color amarillo.
- `%s`: Muestra el mensaje del commit.
- `%Cgreen(%ar)%Creset`: Muestra la fecha relativa del commit en color verde.
- `%C(bold blue)<%an>%Creset`: Muestra el nombre del autor en negrita y azul.
- `--abbrev-commit`: Muestra el hash del commit como un identificador abreviado.

Resultado:

![image-20240206182638867](C:\Users\USUARIO\AppData\Roaming\Typora\typora-user-images\image-20240206182638867.png)

## 3. 

git config --global alias.last 'log -1 HEAD'

Este comando agrega un alias llamado "last" al archivo de configuración global de Git.

![image-20240206183918693](C:\Users\USUARIO\AppData\Roaming\Typora\typora-user-images\image-20240206183918693.png)

4.

git config --global alias.ec '!git config --global --edit'

Este comando agrega un alias llamado "ec" que ejecuta el comando `git config --global --edit`. El signo de exclamación (`!`) al principio del alias indica que se ejecutará un comando del sistema

![image-20240206184411231](C:\Users\USUARIO\AppData\Roaming\Typora\typora-user-images\image-20240206184411231.png)

## 5.

git log --graph --pretty=format:'%C(yellow)%h%Creset %C(red)%d%Creset \ %s \%C(bold blue)[%an]%Creset' --abbrev-commit --all

![image-20240206190737160](C:\Users\USUARIO\AppData\Roaming\Typora\typora-user-images\image-20240206190737160.png)