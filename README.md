
 # 🏭 PREDICCIÓN DE FALLAS EN HERRAMIENTAS ROTATIVAS INDUSTRIALES 🔩

## 📝 DESCRIPCIÓN DEL PROYECTO
Este análisis se enfoca en establecer una **regla simple y confiable** para anticipar fallas en herramientas rotativas. Utilizando el nivel de desgaste (`tool_wear_level`), se desarrolló un modelo de Machine Learning que provee **certeza total** en la predicción. El objetivo es optimizar drásticamente el mantenimiento predictivo, priorizar revisiones y **eliminar los paros no planeados** causados por el desgaste del herramental.

---

## 🛠️ TECNOLOGÍAS UTILIZADAS
- **Python**: Análisis y modelado
- **Pandas**: Limpieza, filtrado y preparación de datos
- **Scikit-learn**: Implementación y entrenamiento del **Modelo de Árbol de Decisión**
- **Matplotlib**: Visualización funcional del Árbol de Decisión

---

## 🎯 RESULTADOS CLAVE
- **Análisis de Riesgo:** Se clasificaron **685** herramientas en la zona crítica (alto riesgo de falla).
- **Precisión del Modelo:** El Árbol de Decisión predice la bandera de falla (`failure_flag`) con un rendimiento del **100% de precisión** en los datos de prueba.
- **Regla de Oro:** El **desgaste ($\text{tool\_wear\_level}$)** es la única variable necesaria para la predicción, con un punto de corte definitivo.

---

## 🌳 REGLA DE ORO: ÁRBOL DE DECISIÓN
El modelo establece una única y sencilla regla para la toma de decisiones:

- **Nodo Raíz:** Si $\text{tool\_wear\_level} \le \mathbf{80.011}$, la clase predicha es **No Falla**.
- **Nodo de Falla:** Si $\text{tool\_wear\_level} > \mathbf{80.011}$, la clase predicha es **Falla**.
- *Soporte:* Esta regla separa perfectamente los $\mathbf{2,213}$ casos sin falla de los $\mathbf{556}$ casos de falla (Gini = 0.0).

---

## 📈 CONCLUSIÓN OPERATIVA
Este proyecto transforma la estrategia de mantenimiento de reactiva a proactiva y garantizada.

1.  **Enfoque Único:** Se demostró que el monitoreo puede simplificarse concentrándose exclusivamente en la métrica de **desgaste**. Las variables de vibración, carga y acústica no añaden valor predictivo.
2.  **Acción Inmediata:** El criterio de **$\text{tool\_wear\_level} > \mathbf{80.011}$** debe implementarse como el **protocolo de retiro obligatorio** de la herramienta, eliminando el riesgo operativo y asegurando la continuidad de la producción.