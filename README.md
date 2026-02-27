# FacePhi-Challenge-2026-Bi-metrics
Por Andrea Fuentes Pérez y Víctor Sánchez Auñón
## Requerimientos (instalar con "py -3.11 -m pip install -r requirements.txt"):
- Python 3.11.9
- doctr 1.9.0 --> Imagen a texto
- pillow 11.1.0 --> uso de PIL para añadir contraste, rotación y recorte de las imágenes
- os (de la instalación de Python) --> Guardado de imágenes temporales y borrado de estas
- date --> formateo de fechas
- mediapipe 0.10.21 --> Visión por computador
- opencv-python 4.11.0.86 -->  Uso de webcam
- deepface 0.0.98 --> Comparación facial
- re --> Comprobaciones con expresiones regulares
- copy --> Manejo de diccionarios para evitar errores
- json --> Export a JSON
- matplotlib --> para show_ocr_result()
- mplcursors --> para show_ocr_result()
- Dependencias:
    - tensorflow 2.12.0 --> Deep Learning de los modelos de deepface
    - numpy 1.23.5 --> arrays y matemáticas
 
## Funcionalidades Principales
Extracción de Datos (OCR): Lectura automática de campos del DNI y validación de Checksums (MRZ) entre otros.

Prueba de Vida (Liveness): Validación mediante MediaPipe que requiere parpadeo y un número aleatorio de gestos manuales para evitar fraudes.

Matching Biométrico: Comparación facial entre la foto del DNI y la captura de la webcam usando DeepFace (modelo VGG-Face).

Exportación de Resultados: Generación de un informe final en formato JSON con veredicto de aptitud.

