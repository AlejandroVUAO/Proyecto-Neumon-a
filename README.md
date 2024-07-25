# Proyecto-Neumonia
El objetivo de este proyecto es ayudar a los estudiantes a desarrollar las habilidades técnicas para el desarrollo de software. En este proyecto deberán usar GIT, Docker, pruebas unitarias y conceptos de diseño de software.


Aplicación de una técnica de explicación llamada Grad-CAM para resaltar con un mapa de calor las regiones relevantes de la imagen de entrada.

# Uso de la herramienta:

Instale Anaconda para Windows siguiendo las siguientes instrucciones: https://docs.anaconda.com/anaconda/install/windows/

Abra Anaconda Prompt y ejecute las siguientes instrucciones:

conda create -n tf tensorflow

conda activate tf

cd UAO-Neumonia

pip install -r requirements.txt

python detector_neumonia.py

#Uso de la Interfaz Gráfica:

Ingrese la cédula del paciente en la caja de texto
Presione el botón 'Cargar Imagen', seleccione la imagen del explorador de archivos del computador (Imagenes de prueba en https://drive.google.com/drive/folders/1WOuL0wdVC6aojy8IfssHcqZ4Up14dy0g?usp=drive_link)
Presione el botón 'Predecir' y espere unos segundos hasta que observe los resultados
Presione el botón 'Guardar' para almacenar la información del paciente en un archivo excel con extensión .csv
Presione el botón 'PDF' para descargar un archivo PDF con la información desplegada en la interfaz
Presión el botón 'Borrar' si desea cargar una nueva imagen

![image](https://github.com/user-attachments/assets/abfcf76e-24fe-407e-b1fc-d11170d12a18)

Despues de probar localmente vamos a crear la imagen en docker adjuntando el codigo fraccionado:

![image](https://github.com/user-attachments/assets/d950a688-1874-4e85-9f4f-b3097c3ccf6d)

verificamos desde consola el login y las imagenes con "docker Login" y "Docker images":

![image](https://github.com/user-attachments/assets/5882ee39-3056-41bb-8342-0c766759ecda)

Instalamos xming y Finalmente con el comando docker "run -it  -e DISPLAY=host.docker.internal:0.0 proyectoneumoniaav:project2 python3 main.py" podemos ejecutar el programa: 

![image](https://github.com/user-attachments/assets/f72fc293-7d80-4631-8bf0-81c9803633be)



