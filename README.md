# Beca 18 RAG Chatbot

## Descripción
Pipeline RAG que responde preguntas sobre el reglamento oficial de Beca 18 
(Resolución Directoral Ejecutiva N.° 033-2026-MINEDU/VMGI-PRONABEC).

## Pipeline
PDF → extracción de texto → chunking → embeddings (Gemini) → ChromaDB → 
búsqueda semántica → generación fundamentada (Gemini) → interfaz de chat

## Instalación
pip install -r requirements.txt

## Configuración API Key
1. Copia .env.example a .env
2. Agrega tu GEMINI_API_KEY en el archivo .env
Obtén tu key gratis en: https://aistudio.google.com/app/apikey

## Cómo ejecutar
1. Configura el archivo .env con tu API key
2. Descarga beca18_reglamento.pdf en la carpeta data/
3. Abre notebooks/beca18_rag_chatbot.ipynb en Jupyter
4. Ejecuta todas las celdas en orden

## Uso del chatbot
- Escribe tu pregunta en el cuadro de texto
- Ajusta el slider para controlar cuántos fragmentos recuperar
- Haz clic en Consultar
- Expande las fuentes para ver los fragmentos utilizados
