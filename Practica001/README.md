# Guía de Instalación y Ejecución

Este proyecto contiene un modelo de riesgo crediticio implementado en un Jupyter Notebook (`Modelo1.ipynb`).

## Requisitos Previos

Asegúrate de tener instalado Python (versión 3.8 o superior).

## Instalación

1.  **Clonar o descargar el proyecto** en tu máquina local.

2.  **Crear un entorno virtual** (opcional pero recomendado):
    ```bash
    python -m venv venv
    ```

3.  **Activar el entorno virtual**:
    *   En Windows:
        ```bash
        .\venv\Scripts\activate
        ```
        > **Nota:** Si recibes un error de "ejecución de scripts deshabilitada", ejecuta este comando en PowerShell antes de activar el entorno:
        > ```powershell
        > Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
        > ```
    *   En macOS/Linux:
        ```bash
        source venv/bin/activate
        ```

4.  **Instalar las dependencias**:
    Ejecuta el siguiente comando para instalar todas las librerías necesarias:
    ```bash
    pip install -r requirements.txt
    ```
    
    *Nota: Si no usas el archivo `requirements.txt`, puedes instalar las librerías manualmente:*
    ```bash
    pip install pandas numpy matplotlib scikit-learn scipy notebook
    ```

## Ejecución

Para ejecutar el notebook:

1.  Asegúrate de que el entorno virtual esté activado (si creaste uno).
2.  Inicia Jupyter Notebook:
    ```bash
    jupyter notebook
    ```
3.  Se abrirá una pestaña en tu navegador. Haz clic en `Modelo1.ipynb` para abrirlo.
4.  Ejecuta las celdas secuencialmente (Shift + Enter) o ve al menú `Cell` > `Run All`.

## Descripción del Modelo

El notebook realiza los siguientes pasos:
1.  **Simulación de Datos**: Genera datos sintéticos de 1,000 solicitantes.
2.  **Preprocesamiento**: Limpia y escala los datos.
3.  **Entrenamiento**: Entrena un modelo de Regresión Logística.
4.  **Evaluación**: Muestra métricas como la matriz de confusión y la curva ROC.
5.  **Predicción**: Simula decisiones de crédito para nuevos clientes.
