
# RAG Exercise with Cohere
Este proyecto implementa un sistema RAG (Retrieval-Augmented Generation) básico usando la API de Cohere.

## Arquitectura RAG Implementada

1. **Vectorización**: Conversión de documentos y queries a embeddings usando `embed-english-v3.0`
2. **Almacenamiento**: Embeddings guardados en formato JSON para reutilización
3. **Recuperación**: Búsqueda semántica por similitud coseno
4. **Generación**: Respuestas contextualizadas usando `command-r-plus`

## Estructura del Proyecto
rag-exercise-cohere/
├── notebooks/
│   └── rag_exercise.ipynb    # Notebook principal
├── data/
│   └── embeddings.json       # Embeddings precalculados
├── src/                      # Código reutilizable (futuro)
├── .env                      # API keys (no incluido en Git)
├── requirements.txt          # Dependencias Python
└── README.md                # Esta documentación

## Tecnologías Usadas

- **Cohere API**: Embeddings y generación de texto
- **NumPy**: Cálculos vectoriales y similitud coseno
- **Pandas**: Manipulación de datos
- **Python-dotenv**: Gestión segura de API keys

## Resultados

- ✅ Sistema RAG funcional con 8 documentos de ejemplo
- ✅ Búsqueda semántica con embeddings de 1024 dimensiones
- ✅ Generación de respuestas contextualizadas
- ✅ Persistencia de embeddings para optimización

## Próximos Pasos

- [ ] Ampliar dataset con más documentos
- [ ] Implementar chunking para documentos largos
- [ ] Agregar métricas de evaluación (BLEU, ROUGE)
- [ ] Integrar con vector database (FAISS, ChromaDB)
