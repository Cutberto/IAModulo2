# Proyecto de Segmentación de Imágenes con U-Net y MobileNet

Este proyecto utiliza la arquitectura U-Net combinada con la red neuronal pre-entrenada MobileNet para realizar la segmentación de imágenes. Utiliza el dataset oxford_iiit_pet para entrenar y evaluar el modelo de segmentación. El dataset se encuentra bajo la licencia Creative Commons 4.0
Este proyecto esta basado en el tutorial de tensorflow para segmetación de imágenes, el cual se encuentra bajo la licencia https://www.apache.org/licenses/LICENSE-2.0

## U-Net

El modelo U-Net es una arquitectura popular utilizada principalmente para tareas de segmentación de imágenes. Se llama U-Net debido a su forma característica similar a la letra "U".

1. La arquitectura U-Net consta de dos partes principales: el "encoder" y el "decoder".

2. El encoder se encarga de extraer características relevantes de la imagen de entrada. Se compone de una serie de capas de convolución y agrupación (pooling) que reducen la resolución espacial de la imagen pero aumentan el número de canales de características. Esto ayuda a capturar características de diferentes niveles de abstracción.

3. A medida que el encoder reduce la resolución espacial, guarda copias de las características en diferentes etapas en una estructura llamada "conexiones de salto" (skip connections). Estas conexiones de salto capturan detalles de la imagen original en diferentes escalas y se utilizarán más adelante en el decoder.

4. El decoder toma las características del encoder y las utiliza para generar una máscara de segmentación detallada. A medida que el decoder se expande, se aplican operaciones de convolución y desconvolución (o upsampling) para aumentar gradualmente la resolución espacial de las características.

5. En cada paso del decoder, se agregan las características de la etapa correspondiente del encoder mediante las conexiones de salto. Esto permite combinar características de diferentes escalas y preservar detalles finos mientras se reconstruye la imagen segmentada.

6. Finalmente, la salida del decoder es una máscara de segmentación que tiene la misma resolución espacial que la imagen de entrada original. Esta máscara se puede utilizar para identificar y clasificar diferentes regiones o elementos de interés en la imagen.

## Ejecución

Para ejecutar el proyecto recomiendo ampliamente utilizar Google Colab, debido a que su ambiente de python ya se encuentra preparado para poder ejecutar todo sin hacer configuraciones adicionales. Además, recomiendo usar un entorno de ejecución GPU para acelerar el proceso de entrenamiento =)
