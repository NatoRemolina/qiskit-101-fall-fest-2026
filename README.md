# Qiskit 101: tu primer circuito cuántico

**Qiskit Fall Fest 2026** · martes 3 de noviembre de 2026, 19:20 – 20:00 (hora de Colombia) · sesión virtual en español

Hola, soy **Natalia Remolina**, de la Universidad Nacional de Colombia y de [Kat Quantum](https://katquantum.com/fall-fest). Este repositorio tiene los notebooks de mi sesión *Qiskit 101*, para que puedas seguir la presentación en tu computador mientras la ves en vivo, o repetirla después con calma.

En la sesión vamos del bit al circuito: qubits, superposición, medición, la esfera de Bloch, las compuertas como giros, la CNOT y, al final, el estado de Bell, que construimos y ejecutamos primero en un simulador y después en un computador cuántico real de IBM.

## Los notebooks

| Notebook | Qué hay | Cuándo usarlo | Colab |
|---|---|---|---|
| [`practica_en_vivo.ipynb`](notebooks/practica_en_vivo.ipynb) | El estado de Bell paso a paso: Composer, código, simulador, hardware real y un reto | **Durante la sesión** (19:43 – 19:56) | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/practica_en_vivo.ipynb) |
| [`hello-world_es.ipynb`](notebooks/hello-world_es.ipynb) | Bell con Sampler y Estimator, y un estado de 100 qubits | Para casa | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/hello-world_es.ipynb) |
| [`get-started-with-qiskit_es.ipynb`](notebooks/get-started-with-qiskit_es.ipynb) | Los conceptos básicos de Qiskit desde cero | Para casa | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/get-started-with-qiskit_es.ipynb) |
| [`your-first-quantum-experiment_es.ipynb`](notebooks/your-first-quantum-experiment_es.ipynb) | Un primer experimento: la energía de un sistema de dos espines | Para casa | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/your-first-quantum-experiment_es.ipynb) |
| [`QGSS2026_Lab0_es.ipynb`](notebooks/QGSS2026_Lab0_es.ipynb) | Ejercicios de calentamiento de la escuela de verano de Qiskit | Para practicar | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/QGSS2026_Lab0_es.ipynb) |

### Material de estudio

| Notebook | Qué hay | Colab |
|---|---|---|
| [`compuertas_explicadas.ipynb`](estudio/compuertas_explicadas.ipynb) | Las compuertas X, Y, Z, H, S, T y CNOT paso a paso, con su matriz, la esfera de Bloch y experimentos para adivinar, hasta llegar al estado de Bell. Es el complemento de la parte teórica de la presentación | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/estudio/compuertas_explicadas.ipynb) |

Si es tu primera vez, te recomiendo este orden: `compuertas_explicadas` → `practica_en_vivo` → `hello-world_es`.

## Cómo seguir la sesión

### Opción 1: en tu computador

Necesitas Python 3.10 o más reciente y Git.

```bash
git clone https://github.com/NatoRemolina/qiskit-101-fall-fest-2026.git
cd qiskit-101-fall-fest-2026
python3 -m venv .venv
source .venv/bin/activate        # en Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

En JupyterLab abre `notebooks/practica_en_vivo.ipynb` para la sesión, o `estudio/compuertas_explicadas.ipynb` para repasar las compuertas.

### Opción 2: sin instalar nada

Usa el enlace **Abrir** de la tabla para abrir el notebook en Google Colab. En la primera celda de código quita el `#` de la línea `%pip install …` y ejecútala antes que las demás.

### Opción 3: solo mirar

El paso 0 de la práctica se hace en el [IBM Quantum Composer](https://quantum.cloud.ibm.com/composer), que funciona en el navegador sin cuenta ni instalación.

## ¿Necesito una cuenta de IBM Quantum?

No. Todo funciona sin cuenta: el simulador corre en tu computador y, en lugar del computador cuántico real, puedes usar las celdas marcadas **«Alternativa sin cuenta»**, que usan una copia local de un procesador de IBM (`FakeTorino` o `FakeBelemV2`) con su ruido.

Si quieres ejecutar en hardware real, crea una cuenta gratuita en [IBM Quantum Platform](https://quantum.cloud.ibm.com/) (el plan Open da el equivalente a 10 minutos de QPU cada 28 días) y sigue la guía [Configurar IBM Cloud](https://quantum.cloud.ibm.com/docs/es/guides/cloud-setup).

> **Cuida tu clave de API.** Guárdala una sola vez con `QiskitRuntimeService.save_account(...)` y después bórrala de la celda. Nunca la subas a un repositorio ni la compartas en pantalla.

## Referencias

Los notebooks son traducciones al español, con notas para principiantes, de material de IBM Quantum y de la comunidad de Qiskit:

- **Práctica en vivo**: basada en la lección [Build and run your first quantum program](https://quantum.cloud.ibm.com/learning/en/courses/use-a-qc-today/build-and-run-your-first-quantum-program) y el video [De cero a lo cuántico | Ep. 1](https://www.youtube.com/watch?v=vSFv_i_FAXg), de IBM Quantum.
- **hello-world_es**: [Hello world](https://quantum.cloud.ibm.com/docs/en/guides/hello-world), documentación de IBM Quantum.
- **get-started-with-qiskit_es**: [Get started with Qiskit in the classroom](https://quantum.cloud.ibm.com/learning/en/modules/quantum-mechanics/get-started-with-qiskit), IBM Quantum Learning.
- **your-first-quantum-experiment_es**: [Your first quantum experiment](https://quantum.cloud.ibm.com/learning/en/courses/use-a-qc-today/your-first-quantum-experiment), IBM Quantum Learning.
- **QGSS2026_Lab0_es**: [Lab 0 de la Qiskit Global Summer School 2026](https://github.com/qiskit-community/qgss-2026/blob/main/lab-0/QGSS2026_Lab0.ipynb), qiskit-community.

Material de apoyo de la presentación:

- IQM Quantum Computers, *Quantum Computing Cheat Sheet for circuit magicians* (CC BY-SA): de ahí vienen las figuras de las compuertas de las diapositivas.
- [Documentación de Qiskit](https://quantum.cloud.ibm.com/docs/es) e [IBM Quantum Learning](https://quantum.cloud.ibm.com/learning/es).
- [Qiskit Fall Fest 2026 en Kat Quantum](https://katquantum.com/fall-fest).

El contenido original pertenece a sus autores y conserva sus licencias; aquí solo se traduce y se adapta para la sesión.

## Versiones probadas

Qiskit 2.6.1 · qiskit-ibm-runtime 0.51 · qiskit-aer 0.18.2 · Python 3.12
