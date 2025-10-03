
 🏭  ## PREDICCIÓN DE FALLAS EN HERRAMIENTAS ROTATIVAS INDUSTRIALES  🔩


## 📝 DESCRIPCIÓN DEL PROYECTO
Este análisis se enfoca en anticipar fallas en herramientas rotativas mediante la clasificación técnica del desgaste. Se definió un umbral crítico en `tool_wear_level` (≥ 80.06) que permite identificar registros con alto riesgo de falla. El objetivo es optimizar el mantenimiento predictivo, priorizar revisiones y reducir paros no planeados.

## 🛠️ TECNOLOGÍAS UTILIZADAS
- **Python**: Análisis y modelado  
- **Pandas**: Limpieza, filtrado y clasificación por umbral  
- **Scikit-learn**: Entrenamiento de modelo de clasificación (árbol de decisión)  
- **Matplotlib**: Visualización funcional del árbol

## 🎯 RESULTADOS CLAVE
- Se clasificaron 685 registros como críticos por desgaste  
- El modelo de árbol de decisión predice `failure_flag` con **100% de precisión**  
- El umbral ≥ 80.06 separa perfectamente los casos de falla  
- El árbol es explicable, directo y útil para mantenimiento

## 🌳 VISUALIZACIÓN DEL MODELO
El árbol de decisión entrenado muestra que `tool_wear_level` es suficiente para anticipar falla:

- Nodo raíz: `tool_wear_level <= 80.011`  
- Rama izquierda: 2213 registros sin falla  
- Rama derecha: 556 registros con falla  
- Gini = 0.0 en ambas ramas → separación perfecta

## 📈 CONCLUSIÓN OPERATIVA
El análisis confirma que el desgaste crítico en herramientas rotativas puede anticipar falla con precisión total. El criterio técnico es claro, el resultado es confiable, y la aplicación en planta es inmediata: prioriza revisiones, reduce paros y respalda decisiones de mantenimiento sin rodeos.