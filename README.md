# 🧠 Detector de Frases Tóxicas

Este proyecto es una aplicación web simple que permite al usuario ingresar una frase para verificar si contiene contenido tóxico, utilizando el modelo preentrenado de TensorFlow.js.

## 🚀 Características

- Interfaz web sencilla y clara.
- Detecta insultos y toxicidad en comentarios en **inglés**.
- Utiliza el modelo preentrenado [`@tensorflow-models/toxicity`](https://github.com/tensorflow/tfjs-models/tree/master/toxicity).
- Análisis instantáneo desde el navegador sin necesidad de backend.

## 📦 Tecnologías utilizadas

- HTML5 + CSS3
- JavaScript
- [TensorFlow.js](https://www.tensorflow.org/js)
- [Modelo de Toxicidad de TensorFlow](https://github.com/tensorflow/tfjs-models/tree/master/toxicity)

## 📸 Captura

![Demo de la app](demo.gif)

## ⚠️ Limitaciones

Actualmente, el modelo **solo detecta toxicidad en inglés**, ya que fue entrenado con un dataset de comentarios en inglés.

Ejemplos detectados correctamente:

- `You're a piece of trash!`
- `I hate you so much.`
- `Go kill yourself.`

Ejemplos **no detectados** porque están en español:

- `Eres un idiota.`
- `Callate, imbécil.`
- `Vete a la mierda.`

## ✅ Posibles mejoras

- 🌐 Traducir automáticamente el texto del usuario (de español a inglés) antes de analizarlo.
- 🧠 Integrar un modelo de detección de toxicidad entrenado en español como [`pysentimiento/toxic-comments-es`](https://huggingface.co/pysentimiento/toxic-comments-es).
- 🔁 Permitir detección de múltiples frases a la vez.
- 🎨 Mejorar la UI/UX.

## 🧪 Cómo usar

1. Abre el archivo `index.html` en tu navegador.
2. Escribe una frase en el cuadro de texto.
3. Haz clic en **"Analizar"**.
4. El resultado mostrará si el mensaje contiene toxicidad y su tipo (insulto, amenaza, lenguaje obsceno, etc.).

## 📄 Licencia

MIT

---

Hecho con ❤️ usando TensorFlow.js.
