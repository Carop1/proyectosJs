# Taller Alias 

## 1.



- `--graph`: Muestra una representación gráfica del historial de commits.
- `--pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%ar)%Creset by %an'`: Define un formato personalizado para la salida.
- `%Cred`: Establece el color rojo para el hash corto del commit.
- `%h`: Muestra el hash corto del commit.
- `%Creset`: Restablece el color al predeterminado.
- `-%C(yellow)%d%Creset`: Muestra las referencias (ramas o tags) en las que está involucrado el commit en color amarillo.
- `%s`: Muestra el mensaje del commit.
- `%Cgreen`: Establece el color verde para la fecha relativa del commit.
- `(%ar)`: Muestra la fecha relativa del commit.
- `by %an`: Muestra el autor del commit.
- `--abbrev-commit`: Muestra el hash del commit como un identificador abreviado.
- `-n 5`: Limita la salida a los últimos 5 commits.
- `--all`: Incluye todas las ramas en la búsqueda