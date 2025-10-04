<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/18569986-3e5e-4149-b68a-458f25ad1a20" />


# 🧠 Cybersecurity Alert Classifier

**AI-powered cybersecurity alert classifier built with Orange to detect and reduce false positives.**

---

## 📘 Descripción

Este proyecto utiliza **machine learning** con la herramienta **Orange Data Mining** para clasificar alertas de ciberseguridad en tres categorías:

- 🟢 **Positivo:** Ataque o evento real detectado.  
- 🟡 **Falso Positivo:** Alerta generada incorrectamente (no representa una amenaza real).  
- ⚪ **No Positivo:** Tráfico o evento normal sin relación con un ataque.  

El objetivo principal es **mejorar la precisión de los sistemas de detección de intrusiones (IDS/IPS)** y **reducir el tiempo invertido en revisar falsos positivos**, optimizando la respuesta ante incidentes de seguridad.

---

## 🎯 Objetivo

Entrenar y evaluar un modelo de IA que aprenda a **distinguir entre eventos reales y falsos positivos** en registros de seguridad, utilizando un enfoque visual y supervisado en Orange.

---

## 🧩 Dataset

El dataset utilizado fue creado manualmente para simular distintos tipos de tráfico y alertas de ciberseguridad.  
Contiene las siguientes columnas:

| Columna | Descripción |
|----------|--------------|
| `src_ip` | Dirección IP de origen |
| `dst_ip` | Dirección IP de destino |
| `protocol` | Protocolo de red utilizado |
| `port` | Puerto de comunicación |
| `packet_size` | Tamaño del paquete en bytes |
| `alert_type` | Tipo de alerta generada |
| `label` | Clase objetivo (Positivo, Falso Positivo, No Positivo) |

📂 Archivo del dataset: `dataset_ciberseguridad.xlsx`

---

## ⚙️ Flujo de trabajo en Orange

1. **Carga del dataset** → Widget *File*  
2. **Preprocesamiento** → *Select Columns*, *Continuize*, *Normalize*  
3. **Entrenamiento del modelo** → *Random Forest*, *Logistic Regression*  
4. **Evaluación** → *Test & Score*, *Confusion Matrix*, *ROC Analysis*  
5. **Visualización de resultados** → comparación de modelos y detección de falsos positivos  

📸 *Ejemplo del flujo de trabajo en Orange.*
<img width="1743" height="1028" alt="Captura de pantalla 2025-09-29 201215" src="https://github.com/user-attachments/assets/ef372012-67a1-4ec4-8ed2-dcfb649e0881" />


---

## 🧠 Tecnologías utilizadas

- 🧩 **Orange Data Mining** (visual ML)
- 🐍 **Python** (backend de Orange)
- 📊 **Pandas / Excel** para manipulación de datos
- 💻 **Machine Learning Supervisado** (Clasificación)

---

## 📊 Resultados esperados

- Precisión promedio: **85–90%**  
- Reducción de falsos positivos en el dataset de prueba.  
- Matriz de confusión y curva ROC que reflejan la capacidad del modelo para distinguir correctamente las clases.

*(Los resultados pueden variar según los parámetros de entrenamiento y balanceo de datos.)*

<img width="962" height="1012" alt="Captura de pantalla 2025-09-29 204006" src="https://github.com/user-attachments/assets/6909d404-1874-4b94-808f-37485af6b7a4" />
<img width="1128" height="725" alt="Captura de pantalla 2025-09-29 204016" src="https://github.com/user-attachments/assets/7fbf7e3b-3e59-4689-a00c-441abd851bf4" />



---

## 🚀 Cómo ejecutar el proyecto

1. Abrí **Orange Data Mining**.  
2. Cargá el archivo `dataset_ciberseguridad.xlsx` desde el widget **File**.  
3. Reproducí el flujo mostrado en este repositorio o abrí el archivo `.ows` incluido.  
4. Ejecutá los clasificadores y analizá las métricas en **Test & Score**.  

---

## 🧑‍💻 Autor

Proyecto creado por **Ivan Rodriguez**  
📧 Contacto: ivan.rodriguez.cv@gmail.com  
🔗 LinkedIn: https://www.linkedin.com/in/ivan-francisco-rodriguez/
📁 Repositorio: https://github.com/ivanfr12/cybersecurity-alert-classifier

---

## 🛡️ Licencia

Este proyecto se distribuye bajo la licencia **MIT**, lo que permite su libre uso, modificación y distribución con fines educativos o de investigación.

---

> 💬 *"Reducing false positives means more time responding to real threats — not noise."*
