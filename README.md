# Proyecto_parqueadero_Ean
En este repositorio realizamos un proyecto en el cual generamos un programa útil para lo que se comprende del funcionamiento de un parqueadero

![empleado](https://user-images.githubusercontent.com/88093015/134287788-000752fb-7bf4-41a0-b08c-9a92a36178dd.PNG)

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

![mismo_dia](https://user-images.githubusercontent.com/88093015/134277739-17628af3-e1dc-4df0-97bf-e1f8da28992e.PNG)

en está parte del código se usa una variable dias en el cual se calcula si el vehiculo ingresó y salió el mismo día, en caso de ser así se ejecuta este código y calculará
los minutos transcurridos.

![dia_siguiente](https://user-images.githubusercontent.com/88093015/134278345-b50255e0-0da9-4931-82fc-64c19b52749d.PNG)

si la estadía del vehículo es de un día para otro por ejemplo, si el vehículo entra a las 11 PM y sale a la 1 AM el código anterior al que está arriba dará error entonces
para eso se pide la fecha para calcular el día, al saber que salió un día despúes y se ejecute está parte del código donde se guarda el tiempo real de entrada y una hora relativa de salida donde fijamos las 12 AM en hora militar, como no se puede fijar las 24 horas se fijan 23:59:59 y luego se suma el segundo faltante paras las 24, luego restamos la hora de salida con la hora relativa 12 AM entonces de la 1 AM a las 12 AM hay una hora y sumamos la hora de entrada con la hora de salida lo que nos da el tiempo transcurrido de 2 horas equivalentes a 120 minutos.

![Ejemplo](https://user-images.githubusercontent.com/88093015/134280170-2eb11902-e8d7-4023-bb08-257c1815e4b8.PNG)

Este sería el ejemplo practico-visual anterior.

![más_dias](https://user-images.githubusercontent.com/88093015/134282339-baa1f9d8-be21-458b-8ab9-73f52947d8a7.PNG)

si por alguna razón el usuario lleva estacionado en el parqueadero más de 1 día se debe calcular de otra manera el tiempo transcurrido en él, para eso restamos 1 día que es
el equivalente a las horas de el vehículo el dia de retirar y el resto de tiempo seran las 24 horas por cada día transcurrido, por ultimo haríamos la conversión de horas a minutos para poder calcular el cobro de los usuarios por sus vehículos.

![total_cobrar](https://user-images.githubusercontent.com/88093015/134286320-3197c985-cb14-42eb-b413-55209fc2a54f.PNG)

y para terminar el algoritmo que necesita de la librería datatime en el cual definimos el cobro por minuto de todos los tipos de vehículos, preguntandole al usuario su numero de identificacion para saber si ha estado en el parqueadero más de 5 veces y obtener un descuento del 20 % en el saldo total a pagar y se calculan los precios a pagar por cada tipo de vehículo según el tiempo permanecido en el parqueadero por el cliente.

![cupos](https://user-images.githubusercontent.com/88093015/134286342-e6cf2e9e-1bd1-49eb-818b-6ca784640232.PNG)

en está parte del código irían los cupos del parqueaderos puestos de asignación y disponibilidad del mismo pero lamentablemente no logramos concretar este requerimento y no funciona esta parte del codigo por eso la dejamos comentada pero la idea en un principio era asignar una lista por cada piso pensamos que todo el piso uno fuera destinado a bicicletas y motos ya que es donde necesitamos pocos cupos y el piso dos y tres serían destinados para carros ya que nos piden más cupos usando matrices por ejemplo,
piso_uno=[[101,0],[102,1]] donde piso_uno[0] es [101,0] y piso_uno[0][0] es 101 que es la posicion del estacionamiento y por ultimo piso_uno[0][1] es 0 que es la disponibilidad
donde 0 es que está libre y 1 que está ocupado, pero como explique desde un principio se quedo como una idea porque no logramos concretarla. :'C

![agradecimiento](https://user-images.githubusercontent.com/88093015/134284431-d6a299c4-e870-4513-8beb-d901b094ec65.PNG)

por último en el programa damos las gracias al usuario por usar nuestro servicio, le pedimos que por favor realice el pago correspondiente en caja y le deseamos un feliz dia y además le decimos que vuelva pronto.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Funcionamiento del programa

![empleado_entrada](https://user-images.githubusercontent.com/88093015/134286890-a7264a59-1ed2-46b8-a208-3b1daeac6ebc.PNG)

Cuando el usuario es empleado o no es empleado y si la contraseña es correcta o incorrecta.

![sin_descuento](https://user-images.githubusercontent.com/88093015/134287569-13461e9e-32ca-43c0-8e2c-322a90aa9cb5.PNG)

cuando se registra un usuario sin descuento.

![descuento](https://user-images.githubusercontent.com/88093015/134287590-988d3ebc-cd43-45bf-a12f-c34f6487c680.PNG)

cuando se registra un usuario con descuento.

Muchas gracias por su atención

Fin del proyecto
