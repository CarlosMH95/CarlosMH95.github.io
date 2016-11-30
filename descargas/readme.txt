El dataset presentado cuenta con un total de 155,530 imagenes.
Estas imagenes fueron obtenidas por medio de la grabacion de miembros del CIDIS, en 4 sesiones. En total se obtuvieron 10 videos con una duracion de 4 minutos cada uno.
Se pedia a los participantes que traigan ropa distinta, para asi poder dar variedad a las imagenes.
Luego de esto, se separaron los frames de los videos a una tasa de 5 frames por segundo.Todas estas imagenes fueron capturadas desde una perspectiva de top view.
Las imagenes originales tienen una resolucion de 1280x720 pixeles.
Posteriormente, se realizo una clasificacion para decidir cuales imagenes podrian ser usadas para el entrenamiento.
Todas estas imagenes fueron capturadas desde una perspectiva de top view.
Las imagenes originales tienen una resolucion de 1280x720 pixeles.
 
Se han dividido estas imagenes en dos carpetas: Originales y Entrenamiento.
En la carpeta Originales, se encuentran todas las imagenes que fueron adquiridas, sin ningun tipo de transformacion o procesamiento.
EN carpeta entrenamiento se encuentran imagenes que han sido procesadas mediante una transformacion utilizando algoritmos en MatLab.
 A estas imagenes se les aplico una reduccion del tamano del 50%, dejandolas con una resolucion espacial de 640x360 pixeles para que asi el entrenamiento de las redes neuronales fuera mas rapido.
 
 Las transformaciones fueron:
 
 FLIPH: 
	Se le aplica un flip Horizontal a la imagen
	
 FLIPV:
	Se le aplica un Flip Vertical a la Imagen.
	
 GAUSSIAN1:
	Se introduce ruido Gaussiano a la imagen, con intensidad 0.5.
	
 GAUSSIAN2:
	Se introduce ruido Gaussiano a la imagen, con intensidad 0.2.
	
 SP1:
	Se introduce ruido Sal y Pimienta a la imagen, con intensidad 0.5.
	
 SP2:
	Se introduce ruido Sal y Pimienta a la imagen, con intensidad 0.2.
	
 ROT45:
	Se rota la imagen 45 grados en sentido horario.
	
 ROT90:
	Se rota la imagen 90 grados en sentido horario.
	
 ROT135:
	Se rota la imagen 135 grados en sentido horario.
	
 ROT180:
	Se rota la imagen 180 grados en sentido horario.
	
 RESIZE:
	Se modifica el tamano de la imagen , reduciendola en un 50%
	Cada transformacion aplicada creaba una nueva imagen.
	
	
La carpeta Originales se divide en:
-Clase Cabezas
      -Head: Esta carpeta almacena todas las imagenes en las que se reconocen las cabezas de los participantes. Total: 3662 imag
      -No Head: Esta carpeta almacena todas las imagenes en las que no se reconocen las cabezas de los participantes. Total: 4352 imag
  
-Clase Caídas:

   -Pose 1: Esta carpeta almacena todas las imagenes en las que los participantes estan en posicion Boca arriba. Total: 1114 imagenes              
   -Pose 2: Esta carpeta almacena todas las imagenes en las que los participantes estan en posicion Boca abajo.Total: 800 imagenes
   -Pose 3: Esta carpeta almacena todas las imagenes en las que los participantes estan en posicion de lado, posición fetal. Total: 1072 imagenes
   -Pose 4: Esta carpeta almacena todas las imagenes en las que los participantes estan en posicion de resbalón semisentado, o arrodillado. Total: 1135 imagenes


  
 -Clase Floor:Esta carpeta contiene todas las imagenes en las que se diferencia el espacio de trabajo vacio. Total: 455 imagenes
  
 -Clase Obstacle: Esta carpeta contiene todas las imagenes en las que se diferencia el espacio de trabajo mas un obstaculo. Total: 2019 imagenes
 

 Cada transformacion aplicada creaba una nueva imagen.
 A continuacion se detalla el total de imagenes en cada carpeta, asi como las transformaciones que se les aplico a cada una de las imagenes.
-Clase Cabezas
    -Head: 37983 imagenes
		Transformaciones: (3453 X 11)
			-FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE

    -No Head: 46750 imagenes
        Transformaciones: (4250 X11)
			-FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE

 -Clase Caidas
    
	-Pose 1: 11517 imagenes
		Transformaciones: (1047 X 11)
                   -FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE
    
	-Pose 2: 8690 imagenes
		Transformaciones:(790 X11)
                   -FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE
    
	-Pose 3: 11847 imagenes
		Transformaciones:(1077 X 11)
                   -FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE
    
	-Pose 4:  3377 imagenes
		Transformaciones:(307X11)
                   -FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE

-Clase Floor: 5005 imagenes

	Transformaciones:(455 X11)
                   -FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE
	
-Clase Obstacle: 4675 imagenes
	Transformaciones:425X 11)
                   -FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE

-Clase Walk: 11077 imagenes
     Transformaciones:(1007X11)
                   -FLIPH, FLIPV, GAUSSIAN1,GAUSSIAN2, SP1,SP2 ROT45, ROT90, ROT135, ROT180,RESIZE