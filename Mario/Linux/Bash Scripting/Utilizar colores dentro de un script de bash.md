Así guardamos los colores en variables y luego los podemos utilizar:
```bash
#!/bin/bash

# Definimos los colores como variables
rojo='\033[0;31m'
verde='\033[0;32m'
amarillo='\033[0;33m'
azul='\033[0;34m'
magenta='\033[0;35m'
cyan='\033[0;36m'
negro='\033[0;30m'
gris_claro='\033[0;37m'
blanco='\033[1;37m'
sin_color='\033[0m'

# Imprimimos una frase con cada uno de los colores
echo -e "${rojo}El sol es de color rojo."
echo -e "${verde}El mar es de color verde."
echo -e "${amarillo}La arena es de color amarillo."
echo -e "${azul}El cielo es de color azul."
echo -e "${magenta}Las flores son de color magenta."
echo -e "${cyan}El agua es de color cyan."
echo -e "${negro}La noche es de color negro."
echo -e "${gris_claro}La nieve es de color gris claro."
echo -e "${blanco}Las nubes son de color blanco."
```
Y el resultado:
![[Pasted image 20230211002019.png]]
También podemos guardar en variables colores más alegres como estos:
```bash
#!/bin/bash

# Definimos los colores más luminosos como variables
rojo_luminoso='\033[1;31m'
verde_luminoso='\033[1;32m'
amarillo_luminoso='\033[1;33m'
azul_luminoso='\033[1;34m'
magenta_luminoso='\033[1;35m'
cyan_luminoso='\033[1;36m'
blanco_luminoso='\033[1;37m'
sin_color='\033[0m'

# Imprimimos una frase con cada uno de los colores más luminosos
echo -e "${rojo_luminoso}El sol es de color rojo luminoso."
echo -e "${verde_luminoso}El mar es de color verde luminoso."
echo -e "${amarillo_luminoso}La arena es de color amarillo luminoso."
echo -e "${azul_luminoso}El cielo es de color azul luminoso."
echo -e "${magenta_luminoso}Las flores son de color magenta luminoso."
echo -e "${cyan_luminoso}El agua es de color cyan luminoso."
echo -e "${blanco_luminoso}Las nubes son de color blanco luminoso."
```
Y este es el resultado, con unos colores más luminosos y alegres:
![[Pasted image 20230211002232.png]]
Por último, si queremos volver al color por defecto, debemos utilizar el color reset:
```bash
# Resetear el color por defecto
sin_color='\033[0m'

# Imprimimos una frase en el color por defecto
echo -e "${sin_color}Esta frase está en el color por defecto."
```
Si ejecutamos este color, volvemos al color por defecto en bash:
![[Pasted image 20230211002413.png]]
