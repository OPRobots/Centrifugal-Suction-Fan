# Centrifugal-Suction-Fan
Sistema de succión empleado en #DragonBot y #FujitoraBot
![alt_tag](https://github.com/OPRobots/Centrifugal-Suction-Fan/blob/master/Images/2019-08-20%20(6).jpg)

Para la construcción del sistema de succión centrifugo hay dos partes principales, El ventilador, y la falda. Ambos elementos son cruciales para un funcionamiento eficiente.

#VENTILADOR:
A la hora de diseñar el ventilador hay muchos factores a tener en cuenta cuyos parámetros fueron obtenidos en base a prueba y error, sacando algunas conclusiones personales de los resultados, pero sin estar cotejados con ningún software de dinámica de fluidos o alguna fórmula física. Solo daré mi opinión que puede estar acertada o no. Por favor tengan esto en cuenta. 

El objetivo de realizar un ventilador centrifugo es lograr crear una zona de baja presión debajo del robot para que aparezca una fuerza de atracción al suelo debido a la diferencia de presión encima y debajo del robot. Para lograr la mayor efectividad existe una fórmula que dice lo siguiente:

	Qmax = (φ * (R ^ 2) * H * ω) / 2

**φ:** coeficiente de flujo 

**R:** diámetro exterior del ventilador

**H:** altura de las palas del ventilador

**ω:** Ventilador de velocidad angular de rotación

En definitiva, podemos llegar a la conclusión de que lo que más afecta es que cuanto mayor sea el diámetro exterior del ventilador mayor será el "vacío" que generemos debajo del robot. También podemos decrementar la presión haciendo el ventilador más alto o aumentando su velocidad. Pero es menos significativo que aumentar el radio exterior.
En cuanto al resto de parámetros los hemos realizado en función de la experiencia:

- Nº de palas: El número de palas suele estar comprendido entre 6 y 8 en función del tamaño del ventilador, la velocidad de giro y la curvatura de las palas.

- Velocidad de giro: Nosotros usamos un motor Brushless 1404 de 3500-4500kvs esto son entre 28krpms y 36krpms a 2s es común encontrar centrifugas que usan motores coreless que suelen ir a 52krpms a mayor velocidad creemos que es mejor reducir e inclinar las palas para que no ofrezca tanta resistencia

- Angulo de las palas: las palas están giradas respecto al radio de la circunferencia uns 45º con una ligera curvatura en lugar de ser rectas. Esto es porque en el centro del ventilador el motor proporciona más par y puede soportar mayor carga y a medida que se acerca al borde del ventilador el par proporcionado disminuye, por tanto, una curvatura en la pala aumenta la eficiencia. Cuanto mayo par desarrolle tu robot más pronunciada puede ser esta curvatura. Pero también tendrá más carga y afectará en el consumo. Con un par alto también se podría bajar un poco el ángulo de la pala para expulsar más aire. Pero también afectará al consumo. Hay que buscar una relación de compromiso

- Agujero en el robot: El agujero en el chasis del robot no debe abarcar el 100% del diámetro del ventilador, más bien sobre el 60-70% En nuestros robots tenemos un diámetro externo de ventilador de unos 38mm y un agujero de unos 28mm

- Posición del ventilador: El ventilador cebe ir lo más pegado al chasis cuanto sea posible sin que roce contra él. Para minimizar la entrada de aire por el propio agujero. Y para que las palas tengan menos aire que desplazar. Además, la colocación el sistema centrifugo es recomendable que esté centrado en el robot, pero el centro de la presión de "vacío" no estará determinada por la posición del ventilador, sino por el centro del área de la falda. La cual explicamos ahora.

#FALDA:
La falda es sin duda un elemento CLAVE! a la hora de lograr que este sistema sea eficiente, y de lograr gran fuerza de succión. Se encarga de contener la diferencia de presión y evitar que entre aire para que el ventilador trabaje casi sin carga y así reducir significativamente el consumo. La falda es sin lugar a dudas un 80% de la eficiencia del sistema, como mínimo. Para elaborar una buena falda solo hay que tener en cuenta que hay que crear un área lo más estanca posible. Donde entre la menor cantidad de aire, siendo lo ideal que no entre nada de aire, y que el material empleado sea lo suficientemente deslizante para no frenar al robot al rozar contra el suelo mientras corre, y duradero para que no se desgaste por el camino. Os explicamos como la hacemos nosotros:

![alt_tag](https://github.com/OPRobots/Centrifugal-Suction-Fan/blob/master/Images/2019-08-20%20(4).jpg)
Para crear el área de la falda usamos Scotch magic tape. Es muy deslizante duradero, pega muy bien, y no deja residuos en el robot cuando quitas la falda para poner una nueva.

![alt_tag](https://github.com/OPRobots/Centrifugal-Suction-Fan/blob/master/Images/2019-08-20%20(3).jpg)
Cortamos una tira de celo de la longitud deseada, y la apoyamos en una mesa con el adhesivo hacia arriba.

![alt_tag](https://github.com/OPRobots/Centrifugal-Suction-Fan/blob/master/Images/2019-08-20%20(2).jpg)
Doblamos el celo sobre sí mismo a lo largo, dejando 4-5mm de adhesivo para poder pegarlo más tarde al robot.

![alt_tag](https://github.com/OPRobots/Centrifugal-Suction-Fan/blob/master/Images/2019-08-20%20(1).jpg)
Este sería el resultado final de una de las tiras.

![alt_tag](https://github.com/OPRobots/Centrifugal-Suction-Fan/blob/master/Images/2019-08-20.jpg)
Y así sería como quedaría pegado.

De esta forma creamos unas 5 tiras y las pegamos debajo del robot haciendo un área cerrada, con un pico en la punta para que no se enganche en posibles desniveles que pueda tener la pista, y listo.

![alt_tag](https://github.com/OPRobots/Centrifugal-Suction-Fan/blob/master/Images/Falda.jpg)
Este sería el resultado final. También hemos tapado con celo todos los agujeros y posibles huecos por conde podría entrar aire por el propio chasis para evitar romper la estanqueidad. 

