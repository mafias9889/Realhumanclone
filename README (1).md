# 🧬 RealHumanClone
**By @mafias9889**

Sistema completo de simulación facial hiperrealista + bypass de detección biométrica (Face ID, liveness e IA defensiva). Diseñado para correr localmente desde tu PC con GPU.

---

## 🎯 Objetivo

Construir una identidad digital que se comporte como un humano real, a nivel visual, biológico y conductual. El sistema simula:

- Reconstrucción 3D de rostro
- Parpadeos naturales, microexpresiones
- Flujo sanguíneo sintético (fake PPG)
- Reacción a estímulos
- Ataques adversariales contra IA de detección

---

## 🛠 Requisitos

- Python 3.10+
- GPU AMD (o CPU si no usas ROCm)
- Windows/Linux
- Dependencias:

```bash
pip install -r requirements.txt
```

---

## 📂 Estructura del Proyecto

RealHumanClone/
├─ data_faces/                ← Fotos reales base
├─ models/                    ← Modelos GAN / adversariales
├─ 3d_face/
│   └─ generate_3d_face.py    ← Malla 3D del rostro
├─ liveness_sim/
│   ├─ simulate_ppg.py        ← Pulso sintético
│   ├─ blink_engine.py        ← Microparpadeos
│   └─ head_movement.py       ← Inclinación de cabeza
├─ adversarial_ai/
│   ├─ attack_liveness.py     ← Patch adversarial
│   └─ analyze_target.py      ← Visualiza IA defensiva
├─ deploy/
│   ├─ deploy_local.py        ← Ejecuta todo localmente
│   └─ test_interface.py      ← Interfaz de prueba
├─ requirements.txt
└─ README.md

---

## 🚀 Cómo usar

1. Clona el proyecto:

```bash
git clone https://github.com/mafias9889/RealHumanClone.git
cd RealHumanClone
pip install -r requirements.txt
```

2. Coloca tus imágenes base en `data_faces/`

3. Genera rostro 3D:

```bash
python 3d_face/generate_3d_face.py
```

4. Simula biología facial:

```bash
python liveness_sim/simulate_ppg.py
```

5. Ejecuta ataque adversarial:

```bash
python adversarial_ai/attack_liveness.py
```

6. Lanza el sistema completo localmente:

```bash
python deploy/deploy_local.py
```

---

## 🧠 Créditos y herramientas clave

- DeepFaceLab  
- PIFuHD  
- OpenCV  
- Foolbox  
- YOLOv8  
- Python / Torch

---

## 🔒 Disclaimer

Este proyecto es con fines educativos y de investigación avanzada en IA facial y biometría. No debe usarse para fines maliciosos ni ilegales. Tú eres responsable del uso que le des.

---

## 🤖 By @mafias9889 — stay real, stay invisible.
