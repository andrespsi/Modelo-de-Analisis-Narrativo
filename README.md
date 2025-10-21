# Analizador de Narrativa Audiovisual v3 (Proyecto de Portafolio)

> **Nota Importante:** Este es un repositorio de portafolio y demostración. El código fuente (`.py`) que compone la lógica de este proyecto es privado, no es público y está protegido mediante `.gitignore`. 
>
> El propósito de este repositorio es mostrar la arquitectura del sistema, su modularidad y ejemplos de los informes y datos que genera.

## 1. Descripción General del Proyecto

Este proyecto es un sistema de software avanzado diseñado para el **análisis profundo de contenido audiovisual**.

La herramienta ingiere un archivo de video y audio y lo procesa a través de un *pipeline* de múltiples analizadores especializados. El objetivo es deconstruir el contenido en sus componentes fundamentales, incluyendo elementos perceptuales (cinematografía, audio), narrativos (estructura, storytelling) y de comportamiento (gestos, intención).

El sistema genera como salida un conjunto de datos estructurados (JSON) y un informe completo en lenguaje natural (DOCX) que detalla los hallazgos.

## 2. Arquitectura del Software (Componentes)

El proyecto está construido sobre una arquitectura modular en Python, permitiendo que cada analizador opere de forma independiente. Los componentes principales del sistema (cuyo código fuente es privado) incluyen:

* **Motor Central (`main.py`, `analizador_completo.py`):** Orquesta el flujo de trabajo completo, desde la ingesta del video hasta la generación del informe final.
* **Módulos de Pre-procesamiento (`imports.py`, `check_env.py`):** Gestionan las dependencias y la configuración del entorno.
* **Conectores Externos (`llm_connector.py`):** Administra las conexiones con modelos de lenguaje de IA para el análisis semántico y la redacción.

### Módulos de Análisis Especializados

El núcleo de la innovación reside en una suite de analizadores que diseccionan el contenido:

* **Análisis Perceptual:**
    * `analizador_audio_avanzado.py`: Procesa la prosodia, el tono, el ritmo y los silencios.
    * `analizador_de_cinematografia.py`: Analiza los tipos de plano, ángulos de cámara y movimiento.
    * `analizador_sensorial_Version2.py`: Mide la densidad y el impacto de los estímulos visuales y auditivos.

* **Análisis Narrativo y Contextual:**
    * `analizador_storytelling_Version2.py`: Identifica la estructura narrativa, arquetipos y progresión.
    * `analizador_contextual_Version2.py`: Evalúa el contexto y el subtexto de las escenas.
    * `analizador_de_microeventos.py`: Detecta eventos narrativos de corta duración.
    * `analizador_de_microestructuras.py`: Analiza patrones y repeticiones.

* **Análisis de Comportamiento y Semántica:**
    * `analizador_de_gestos.py`: Interpreta el lenguaje corporal.
    * `analizador_de_intencion.py`: Infiere la intención probable detrás del diálogo o acciones.
    * `analizador_de_lenguaje_Version2.py`: Procesa el diálogo.
    * `analizador_ocr_avanzado.py`: Extrae y analiza texto presente en pantalla.

* **Módulos de Síntesis y Evaluación:**
    * `analizador_de_potencial_Version2.py`: Evalúa el potencial de impacto del contenido.
    * `analizador_de_contrapuntos.py`: Busca congruencias o incongruencias entre los canales (ej. audio vs. video).
    * `analizador_de_cluster_Version2.py`: Agrupa escenas o eventos por temática o energía.
    * `analizador_neuro_Version2.py`: (Módulo avanzado para la interpretación de carga cognitiva).

* **Módulos de Generación de Salida:**
    * `redactor_de_guion.py`: Transcribe y formatea el guion.
    * `analizador_guion_tecnico_modificado.py`: Genera un guion técnico basado en el análisis.
    * `analizador_vision_maestra.py`: Produce la síntesis final del análisis.

## 3. Contenido del Repositorio (Archivos Públicos)

Este repositorio contiene **ejemplos de los resultados** generados por el sistema:

* `resultado_analisis_DATOS.json`: Un archivo JSON que muestra la salida de datos estructurados del análisis.
* `Download (55)_GUION.txt`: Un ejemplo de un guion técnico-narrativo generado por la herramienta.
* `Download (56)_ANALISIS_COMPLETO.docx`: Un informe final completo (formato Word) que presenta la síntesis del análisis en lenguaje natural.
* `Download (57)_ANALISIS_COMPLETO.docx`: Un segundo ejemplo de informe final.

## 4. Autor

**Andrés Eduardo Gonzales Palacios**

https://www.linkedin.com/in/andr%C3%A9s-gonzales-palacios-57344156/
https://osf.io/user/8yrm4