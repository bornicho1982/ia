# AsistenteIA-Codigo

¡Bienvenido al proyecto AsistenteIA-Codigo!

Este es un asistente de codificación inteligente con interfaz gráfica (GUI) diseñado para ayudarte a gestionar, analizar, generar y corregir código utilizando el poder de la Inteligencia Artificial. Podrás interactuar con modelos de lenguaje grandes (LLMs) directamente desde tu aplicación, trabajando con proyectos tanto de tu máquina local como de repositorios de GitHub.

---

## Características Principales

* **Carga Flexible de Proyectos:**
    * Carga y visualiza archivos o carpetas completas desde tu sistema de archivos local.
    * Clona y explora repositorios de GitHub (públicos y privados) directamente desde la aplicación.
* **Asistencia Inteligente de IA:**
    * Envía prompts personalizados a la IA para generar nuevas funciones, corregir errores, refactorizar código o recibir explicaciones detalladas.
    * Integración con **Google Gemini API** (y potencialmente otras APIs de LLMs con nivel gratuito).
* **Procesamiento Asincrónico:**
    * Las operaciones pesadas (clonación de GitHub, llamadas a la IA) se ejecutan en segundo plano, manteniendo la interfaz de usuario fluida y responsiva.
* **Interfaz Gráfica Intuitiva:**
    * Desarrollado con `CustomTkinter` para una experiencia de usuario moderna y fácil de usar.

---

## Requisitos Previos

Antes de empezar, asegúrate de tener instalado lo siguiente:

* **Python:** Versión 3.9 o superior. Puedes descargarlo desde [python.org](https://www.python.org/).
* **Git:** Necesario para clonar repositorios de GitHub. Puedes descargarlo desde [git-scm.com](https://git-scm.com/downloads).

---

## Configuración y Ejecución

Sigue estos pasos para poner en marcha el AsistenteIA-Codigo:

1.  **Clonar el Repositorio:**
    ```bash
    git clone [https://github.com/tu-usuario/AsistenteIA-Codigo.git](https://github.com/tu-usuario/AsistenteIA-Codigo.git)
    cd AsistenteIA-Codigo
    ```
    *(Reemplaza `tu-usuario` con tu nombre de usuario de GitHub).*

2.  **Crear un Entorno Virtual (Recomendado):**
    ```bash
    python -m venv venv
    # En Windows:
    .\venv\Scripts\activate
    # En macOS/Linux:
    source venv/bin/activate
    ```

3.  **Instalar Dependencias:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Crearemos el archivo `requirements.txt` en el siguiente paso).*

4.  **Configurar las Claves de API:**
    * Obtén tu **Google Gemini API Key** desde [Google AI Studio](https://aistudio.google.com/app/apikey).
    * Crea un archivo llamado `.env` en la raíz de este proyecto (la misma carpeta donde está `main.py`) y añade tu clave:
        ```
        GOOGLE_API_KEY="TU_CLAVE_API_DE_GEMINI_AQUI"
        ```
    * **Opcional - Token de Acceso Personal (PAT) de GitHub:** Si planeas acceder a repositorios privados, genera un PAT en la configuración de GitHub y añádelo también a tu archivo `.env` (por ejemplo):
        ```
        GITHUB_PAT="TU_PAT_DE_GITHUB_AQUI"
        ```
        *¡Recuerda NUNCA subir tu archivo `.env` a GitHub! El archivo `.gitignore` ya está configurado para esto.*

5.  **Ejecutar la Aplicación:**
    ```bash
    python main.py
    ```

---

## Uso

(Esta sección se completará a medida que desarrollemos la interfaz y las funcionalidades. Aquí se explicará cómo usar la GUI, seleccionar archivos, introducir prompts, etc.)

---

## Contribución

¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar este asistente, no dudes en abrir un "issue" o enviar un "pull request".

---

## Licencia

Este proyecto está bajo la licencia [MIT License](https://opensource.org/licenses/MIT). (O la licencia que decidas usar).

---
