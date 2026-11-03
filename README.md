# Qiskit 101: tu primer circuito cuántico

Material de la sesión *Qiskit 101* del **Qiskit Fall Fest 2026**: del bit al estado de Bell, ejecutado en un simulador y en un computador cuántico real de IBM.

[![Qiskit](https://img.shields.io/badge/Qiskit-2.6-6929C4?logo=qiskit&logoColor=white)](https://www.ibm.com/quantum/qiskit)
[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Idioma](https://img.shields.io/badge/idioma-espa%C3%B1ol-success)](#)
[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/practica_en_vivo.ipynb)

---

## Sobre la sesión

| | |
|---|---|
| **Evento** | [Qiskit Fall Fest 2026 · Kat Quantum](https://katquantum.com/fall-fest) |
| **Fecha** | Martes 3 de noviembre de 2026, 19:20 – 20:00 (hora de Colombia) |
| **Modalidad** | Virtual, en español |
| **Nivel** | Introductorio: no se necesita experiencia previa en computación cuántica |

**Ruta de la sesión:** bit → qubit → superposición y medición → esfera de Bloch → compuertas como giros → varios qubits y CNOT → estado de Bell → ejecución en un simulador y en hardware real.

## Autora

**Natalia Remolina**, estudiante de Ingeniería Física de la Universidad Nacional de Colombia, sede Medellín.

Hago parte del **Semillero QUANT Research Group** y del **Semillero de Modelos Generativos SIMG** de la Universidad Nacional de Colombia. Me entusiasma aprender tecnologías de impacto, y en especial estoy aprendiendo sobre divulgación científica; esta sesión es parte de ese camino.

[![GitHub](https://img.shields.io/badge/GitHub-NatoRemolina-181717?logo=github)](https://github.com/NatoRemolina)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Natalia%20Remolina-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/natalia-patricia-remolina-rodriguez-1327a8220/)

## Contenido

### Sesión en vivo

| Notebook | Qué hay | Cuándo usarlo | Colab |
|---|---|---|---|
| [`practica_en_vivo.ipynb`](notebooks/practica_en_vivo.ipynb) | El estado de Bell paso a paso: Composer, código, simulador, hardware real y un reto | **Durante la sesión** (19:43 – 19:56) | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/practica_en_vivo.ipynb) |
| [`hello-world_es.ipynb`](notebooks/hello-world_es.ipynb) | Bell con Sampler y Estimator, y un estado de 100 qubits | Después de la sesión | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/hello-world_es.ipynb) |
| [`get-started-with-qiskit_es.ipynb`](notebooks/get-started-with-qiskit_es.ipynb) | Los conceptos básicos de Qiskit desde cero | Después de la sesión | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/get-started-with-qiskit_es.ipynb) |
| [`your-first-quantum-experiment_es.ipynb`](notebooks/your-first-quantum-experiment_es.ipynb) | Un primer experimento: la energía de un sistema de dos espines | Después de la sesión | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/your-first-quantum-experiment_es.ipynb) |
| [`QGSS2026_Lab0_es.ipynb`](notebooks/QGSS2026_Lab0_es.ipynb) | Ejercicios de calentamiento de la Qiskit Global Summer School | Para practicar | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/notebooks/QGSS2026_Lab0_es.ipynb) |

### Material de estudio

| Notebook | Qué hay | Colab |
|---|---|---|
| [`compuertas_explicadas.ipynb`](estudio/compuertas_explicadas.ipynb) | Las compuertas X, Y, Z, H, S, T y CNOT paso a paso, con su matriz, la esfera de Bloch y experimentos para adivinar, hasta llegar al estado de Bell. Complementa la parte teórica de la presentación | [Abrir](https://colab.research.google.com/github/NatoRemolina/qiskit-101-fall-fest-2026/blob/main/estudio/compuertas_explicadas.ipynb) |

### Orden sugerido

1. `estudio/compuertas_explicadas.ipynb`: la base teórica.
2. `notebooks/practica_en_vivo.ipynb`: el primer circuito, de principio a fin.
3. `notebooks/hello-world_es.ipynb`: el mismo circuito con Estimator y a gran escala.
4. Los demás notebooks, según tu interés.

## Estructura del repositorio

```
qiskit-101-fall-fest-2026/
├── notebooks/          # Notebooks de la sesión
├── estudio/            # Material de estudio complementario
├── requirements.txt    # Dependencias de Python
└── README.md
```

## Cómo empezar

### Opción 1: en tu computador

Requisitos: Python 3.10 o más reciente y Git.

```bash
git clone https://github.com/NatoRemolina/qiskit-101-fall-fest-2026.git
cd qiskit-101-fall-fest-2026
python3 -m venv .venv
source .venv/bin/activate        # en Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

En JupyterLab, abre `notebooks/practica_en_vivo.ipynb` para seguir la sesión, o `estudio/compuertas_explicadas.ipynb` para repasar las compuertas.

### Opción 2: en Google Colab, sin instalar nada

Usa el enlace **Abrir** de las tablas. En la primera celda de código, quita el `#` de la línea `%pip install …` y ejecútala antes que las demás.

### Opción 3: en el navegador

El paso 0 de la práctica se hace en el [IBM Quantum Composer](https://quantum.cloud.ibm.com/composer), que funciona sin cuenta ni instalación.

### ¿Hace falta una cuenta de IBM Quantum?

No. El simulador corre en tu computador y, en lugar del hardware real, puedes usar las celdas marcadas **«Alternativa sin cuenta»**, que usan una copia local de un procesador de IBM (`FakeTorino` o `FakeBelemV2`) con su ruido.

Para ejecutar en hardware real, crea una cuenta gratuita en [IBM Quantum Platform](https://quantum.cloud.ibm.com/) (el plan Open da el equivalente a 10 minutos de QPU cada 28 días) y sigue la guía [Configurar IBM Cloud](https://quantum.cloud.ibm.com/docs/es/guides/cloud-setup).

> [!IMPORTANT]
> Guarda tu clave de API una sola vez con `QiskitRuntimeService.save_account(...)` y bórrala de la celda. No la subas a ningún repositorio ni la muestres en pantalla.

## Referencias y créditos

Los notebooks son traducciones y adaptaciones al español, con notas para principiantes, de material de IBM Quantum y de la comunidad de Qiskit:

| Notebook | Fuente original |
|---|---|
| `practica_en_vivo` | [Build and run your first quantum program](https://quantum.cloud.ibm.com/learning/en/courses/use-a-qc-today/build-and-run-your-first-quantum-program) y el video [De cero a lo cuántico, Ep. 1](https://www.youtube.com/watch?v=vSFv_i_FAXg), IBM Quantum |
| `hello-world_es` | [Hello world](https://quantum.cloud.ibm.com/docs/en/guides/hello-world), documentación de IBM Quantum |
| `get-started-with-qiskit_es` | [Get started with Qiskit in the classroom](https://quantum.cloud.ibm.com/learning/en/modules/quantum-mechanics/get-started-with-qiskit), IBM Quantum Learning |
| `your-first-quantum-experiment_es` | [Your first quantum experiment](https://quantum.cloud.ibm.com/learning/en/courses/use-a-qc-today/your-first-quantum-experiment), IBM Quantum Learning |
| `QGSS2026_Lab0_es` | [Lab 0, Qiskit Global Summer School 2026](https://github.com/qiskit-community/qgss-2026/blob/main/lab-0/QGSS2026_Lab0.ipynb), qiskit-community |
| `compuertas_explicadas` | Material propio, basado en la [documentación de Qiskit](https://quantum.cloud.ibm.com/docs/es) |

Material de apoyo de la presentación:

- IQM Quantum Computers, *Quantum Computing Cheat Sheet for circuit magicians* (CC BY-SA): fuente de las figuras de compuertas de las diapositivas.
- [Documentación de Qiskit](https://quantum.cloud.ibm.com/docs/es) e [IBM Quantum Learning](https://quantum.cloud.ibm.com/learning/es).

El contenido original pertenece a sus autores y conserva sus licencias; este repositorio solo lo traduce y lo adapta con fines educativos.

## Versiones probadas

Qiskit 2.6.1 · qiskit-ibm-runtime 0.51 · qiskit-aer 0.18.2 · Python 3.12 y 3.14
