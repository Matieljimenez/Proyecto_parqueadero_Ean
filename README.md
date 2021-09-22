# Proyecto_parqueadero_Ean
En este repositorio realizamos un proyecto en el cual generamos un programa útil para lo que se comprende del funcionamiento de un parqueadero

![empleado](https://user-images.githubusercontent.com/88093015/134273025-a758eb4e-2ee5-4f6e-ab4b-76664bda915e.PNG)

En la primera parte del codigo lo que hicimos fue preguntar a la persona que ingrese si es empleado o usuario del parqueadero en caso de que sea empleado
se activara está parte del codigo que dará la bienvenida al usuario y en caso de ser empleado le pedirá que ingrese su usuario y contraseña hasta que sea
correcta registrando el ingreso del empleado en una lista.

![Usuario](https://user-images.githubusercontent.com/88093015/134273930-a1eb84fc-ef1a-4224-82d0-b890596f5640.PNG)

En caso de que el usuario dijite que no es empleado se desplagará la siguente parte del codigo que le preguntará los datos al usuario para ingresarlo al
sistema del parqueadero y poder hacer el ingreso al parqueadero y respectivamente cobrar la estadia en el mismo, le preguntará el nombre, número de identificación 
que estará en un try para que el usuario ingrese un numero positivo como lo son todas las identificaciónes, seguido de esto se pedirá que especifique el tipo de
vehiculo con el que se va a ingresar al parqueadero.

![placa_bici](https://user-images.githubusercontent.com/88093015/134275002-4f18d6ab-4d0f-47ba-9c6f-6cbf34b9db68.PNG)

y por ultimo en está parte se pedirá la placa en caso de ser un carro ó moto, en caso de ser bicicleta se
pedirá un numero de registro de la bicicleta para poder ingresarla que consta de un maximo de 8 digitos.

![datos_tiempo](https://user-images.githubusercontent.com/88093015/134275485-b59882b3-c51a-4ced-9eff-fb88554ad852.PNG)

Importamos la librería datatime de los recursos que nos proporciona python en el cúal pedimos la fecha para calcular los dias transcurridos cosa que nos ayuda mucho más
adelante, támbien pedimos la hora de entrada al parqueadero y la hora de salida para calcular los minutos de estancia en el parqueadero ya que de está manera es como se
le va a cobrar al usuario.

![Horas](https://user-images.githubusercontent.com/88093015/134277267-541b4d82-e1ee-4c4e-bd7e-46fa33257f06.PNG)

luego se registran en dos variables que despues las pasaremos con un formato especifico para poder hacer cualculos correspondientes con estos datos.

