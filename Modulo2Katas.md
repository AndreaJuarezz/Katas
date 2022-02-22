# Ejercicio - Crear un paquete

En este ejercicio, aprenderás a utilizar entornos virtuales como una forma para no afectar a los paquetes instalados globalmente u otros programas que se ejecutan en tu máquina.

*Para este ejercicio es necesario que lo ejecutes desde la terminal, línea de comandos, cmd, consola, cli, etc. de tu computadora, sé que es desafíante, pero no te preocupes ¡¡Sé que puedes lograrlo!!*

## Crear un entorno virtual

Crea un entorno virtual mediante ``venv``

* Ejecutar en su terminal: ``python3 -m venv env`` o bien ``python -m venv env``

    ```
       python3 -m venv env 
    ```
    ``
    python -m venv env
    ``
    Ahora tienes un directorio (folder) ``env`` creado en tu terminal.
    
    ![image](https://user-images.githubusercontent.com/99098014/155043541-40f614bf-c0f3-4e1f-bcfa-d0c878286d78.png)

* Ejecuta el comando para activar el entorno virtual: ``source env/bin/activate``

    ```
    source env/bin/activate
    # Windows
    env\bin\activate
    
    o bien: 
    env\Scripts\activate

    # Linux, WSL or macOS
    source env/bin/activate
    ```

Ahora ves en tu terminal ``(env)``. Eso significa que has activado tu entorno virtual y se ha aislado del resto de tu máquina.

![image](https://user-images.githubusercontent.com/99098014/155043296-09062f9b-e01a-49ba-ae96-0e416c121a09.png)


## Instalar una biblioteca

Ahora que estás dentro de tu entorno virtual, puedes instalar una biblioteca y saber que la biblioteca solo existirá en el entorno virtual.

* Ejecuta el comando ``pip freeze`` para ver las bibliotecas instaladas en tu entorno:

    ```
    pip freeze
    ```

    No deberías obtener respuesta. A continuación, veamos cómo cambia la salida de ``pip freeze`` cuando se agrega una biblioteca (un paquete).
    
    ![image](https://user-images.githubusercontent.com/99098014/155043344-bb662a07-1b7f-4c5b-91ab-ea0e5d7caccb.png)


* Ejecuta el comando ``pip install`` para instalar una biblioteca:
   ```
   pip install python-dateutil
   ```
   ![image](https://user-images.githubusercontent.com/99098014/155043365-d0c70aba-53f5-4f24-a787-eb1b9db3ea58.png)

* Un gran mensaje de salida de texto dice que está instalando tu biblioteca, y debe terminar con la siguiente oración:

    ```
    Successfully installed python-dateutil-2.8.2 six-1.16.0
    ```
* Vuelve a ejecutar ```pip freeze``` para ver cómo ha cambiado tu lista de bibliotecas:
    ```
    pip freeze
    ```
    ![image](https://user-images.githubusercontent.com/99098014/155043439-9875a416-c05b-4caf-9184-ce13b9319c36.png)

* Ahora deberías ver la siguiente lista:
    ```
    python-dateutil==2.8.2
    six==1.16.0
    ```

### Desactivar un entorno virtual

Hasta ahora, has creado un entorno virtual y le has agregado un paquete. Sin embargo, es posible que estés trabajando en varios proyectos de Python y necesites cambiar entre ellos. Para hacer eso, debes salir (desactivar) tu entorno virtual.

Ejecuta el comando ``deactivate``:
```
deactivate
```
![image](https://user-images.githubusercontent.com/99098014/155043481-90136dac-2f77-4101-8108-a19fe85d94e0.png)

Observa cómo cambia el mensaje de tu terminal ``(env)`` a cómo se veía antes.

¡Felicidades! Has logrado crear y usar correctamente un entorno virtual.

![image](https://user-images.githubusercontent.com/99098014/155043506-62626fdd-e0a5-45cd-89a6-dac3a33f52ba.png)


Curso Propedútico de Python para Launch X - Innovacción Virtual.

Material desarrollado con base en los contenidos de MSLearn y la metáfora de LaunchX, traducción e implementación por: Fernanda Ochoa - Learning Producer de LaunchX.

Redes:
* GitHub: [FernandaOchoa](https://github.com/FernandaOchoa)
* Twitter: [@imonsh](https://twitter.com/imonsh)
* Instagram: [fherz8a](https://www.instagram.com/fherz8a/)
