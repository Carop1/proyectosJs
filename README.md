# Taller Alias 

## 1.

Está trabajando en un proyecto Git colaborativo con varias ramas y commits. Tu tarea es utilizar el comando git log con algunas opciones específicas para obtener un resumen gráfico de los últimos 5 commits en todas las ramas.

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