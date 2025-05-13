# cv_camera 

Este paquete está basado en este [repositorio](https://github.com/Kapernikov/cv_camera) del cual sólo se ha ajustado la declaración de algunas librerías para que no marque un error a la hora de compilar en ROS2 Jazzy Jalisco. 

Este paquete ocupa [camera_info_manager](http://wiki.ros.org/camera_info_manager), si no se establecen datos de calibración, tendrá valores ficticios excepto el ancho y la altura.

Para obtener los datos de calibración de alguna cámara se tiene que instalar el siguiente paquete (si es que no se ha instalado antes) y seguir los pasos de este [tutorial](https://github.com/ros-perception/image_pipeline/blob/rolling/camera_calibration/doc/tutorial_mono.rst):

```
sudo apt-get install ros-jazzy-image-pipeline
```
Al igual que asegurarse que se tengan instaladas las dependencias del paquete al ejecutar la siguientes líneas de código desde la raíz del workspace:

```
sudo apt update
rosdep install -i --from-path src --rosdistro jazzy -y
```