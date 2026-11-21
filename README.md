# Apuntes de clase

Es una aplicación web que transcribe una clase en directo usando solo el micrófono, sin grabar la pantalla. Cuando quieras, convierte la transcripción en apuntes estructurados con Claude. Funciona en el navegador y no hay que instalar nada.

## Funcionalidades

- **Transcripción en directo** en español con el reconocimiento de voz de Chrome o Edge. El texto aparece con marcas de tiempo y la sesión se guarda sola cada pocos segundos.
- **Frases clave (★)**: puedes marcar la última frase como importante y los apuntes le darán prioridad.
- **Generación de apuntes** al final o a mitad de clase, ordenados en resumen, ideas clave, conceptos, frameworks, ejemplos, citas y datos, preguntas de repaso y tareas o entregas.
- **Corrección automática**: al generar los apuntes se corrigen los errores evidentes del reconocimiento de voz, y lo dudoso queda marcado con (¿?).
- **Edición y pegado**: puedes corregir la transcripción a mano o pegar una de Teams o Zoom.
- **Historial privado** por sesión y asignatura, con un selector para pasar de una clase a otra.
- **Grabadora con mejor captación**: puedes elegir el micrófono, probarlo antes de clase con un medidor de nivel y activar «Profesor lejos» para reforzar la voz. La página avisa si el sonido llega débil o satura.
- **Whisper más preciso**: hay una opción de precisión «Máxima» (large-v3-turbo, con tarjeta gráfica). Antes de transcribir se quitan los silencios largos y se filtran las frases inventadas y repetidas.
- **Exportación** a Markdown, con la transcripción incluida, o a Word. Los apuntes también se pueden copiar directamente.

## Uso

1. Antes de la clase, rellena asignatura, tema, profesor y fecha.
2. Pulsa el micrófono rojo para empezar o pausar.
3. Marca con ★ las frases importantes.
4. Pulsa «Generar apuntes» cuando quieras.
5. Revisa los apuntes, edítalos y expórtalos.

## Requisitos

- Chrome, Edge o la app de escritorio de Claude, con conexión a internet.
- La primera vez pide permiso para usar el micrófono y para generar los apuntes con Claude.

## Limitaciones

- La pestaña tiene que estar visible. Si cambias de pestaña, la transcripción se pausa y aparece el botón «Reanudar».
- El audio pasa por los servidores de Google para transcribirse. No se guarda: solo se conserva el texto.
- Si hay varias voces o ruido en el aula, la calidad es media. Baja bastante si el portátil está lejos del profesor.

## Estado y próximos pasos

Es un prototipo y todavía no se ha probado en un aula real. Antes de usarlo en clase, haz una prueba corta para comprobar que el micrófono funciona en la página publicada. Si la calidad no es suficiente, el siguiente paso previsto es un script local con Whisper.
