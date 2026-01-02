📘 Manual de Usuario: Monitor de Riesgo Hemodinámico Dataflow IA
¡Bienvenido al sistema de inteligencia de salud Dataflow IA! Este monitor es una herramienta interactiva diseñada para visualizar cómo los signos vitales de un paciente afectan su probabilidad de riesgo clínico mediante modelos de Regresión Logística.
•	1. Introducción al Sistema
El monitor utiliza un motor de inferencia avanzado para calcular la estabilidad de un paciente en tiempo real. A diferencia de las calculadoras tradicionales, este sistema muestra la dinámica del riesgo, permitiéndote ver no solo qué está pasando, sino por qué está pasando.
•	2. Guía de Controles (Panel Izquierdo)
En la sección "Parámetros Clínicos", encontrarás cuatro controles deslizantes (sliders). Al moverlos, verás que todo el panel de la derecha reacciona instantáneamente.
•	Frecuencia Cardíaca (BPM): Rango de 40 a 180. Simula estados desde bradicardia hasta taquicardia extrema.
•	Saturación (SpO2): Rango de 70% a 100%. Es uno de los predictores más potentes del modelo.
•	Presión Sistólica y Diastólica: Permiten calcular la PAM (Presión Arterial Media), fundamental para la perfusión de órganos.
•	Indicadores Rápidos:
•	Probabilidad de Evento: El número central grande. Indica la posibilidad (0% a 100%) de que el paciente sufra una descompensación crítica.
•	Nivel de Riesgo: Una etiqueta de color que clasifica el estado:
o	🟢 Compensado: Estado óptimo.
o	🟡 Pre-Shock: Alerta preventiva.
o	🔴 Shock Inminente: Requiere intervención inmediata.
•	3. Interpretación de Gráficos (Panel Derecho)
•	A. Dinámica de Probabilidad (Curva Sigmoide)
Este gráfico representa la función matemática del modelo.
•	La Curva Cyan: Es el "camino" del riesgo definido por el modelo de IA.
•	El Punto Rojo: Eres tú (el paciente actual).
o	Si el punto está en la parte baja (izquierda), el paciente está seguro.
o	Si el punto sube por la curva hacia la derecha, el riesgo está escalando exponencialmente.
•	B. Ponderación Variable ($\beta$)
Este es el corazón analítico del monitor. Responde a la pregunta: ¿Cuál de todos los síntomas es el más peligroso ahora?
•	Eje X (0-10): Indica la fuerza del impacto.
•	Barras Dinámicas: Si bajas la saturación a niveles críticos, verás que la barra de SpO2 se estira. Esto indica que la hipoxia es la causa principal del riesgo total.
•	C. Confianza del Diagnóstico
Indica qué tan fiable es la predicción actual.
•	Certidumbre Clínica: Alta cuando los datos son coherentes.
•	Inconsistencia: Sube cuando introduces valores extremadamente contradictorios, avisándote que el modelo está operando en sus límites.
•	4. Protocolos Médicos y Correlación Clínica
El monitor integra criterios de protocolos internacionales para fundamentar su predicción de riesgo:
•	A. Índice de Choque (Shock Index)
El sistema calcula automáticamente el cociente $FC / PAS$.
•	Normal: 0.5 - 0.7.
•	Alerta: $> 0.9$. Un índice elevado predice la necesidad de transfusión masiva o soporte vasopresor incluso antes de que la presión arterial caiga (choque oculto).
•	B. Criterios qSOFA (quick SOFA)
El modelo otorga una ponderación crítica a:
1.	Alteración de la Presión: PAS $\leq 100$ mmHg.
2.	Taquicardia Compensatoria: Como signo temprano de sepsis o hipovolemia. Si detectas que la barra de PAM y FC crecen simultáneamente en el gráfico de ponderación, el paciente cumple criterios de sospecha de mal pronóstico.
•	C. Metas de Perfusión (PAM)
El monitor destaca la Presión Arterial Media (PAM). El protocolo estándar sugiere mantener una PAM $> 65$ mmHg para asegurar la perfusión renal y cerebral. Verás que cuando la PAM cae por debajo de este umbral, la probabilidad de riesgo en el monitor aumenta drásticamente.
•	5. Consejos para la Simulación
1.	El Corredor: Sube la FC a 120 pero mantén la SpO2 en 98% y la Presión en 120/80. El riesgo es bajo por la coherencia de los datos.
2.	El Choque Silencioso: Baja la PAS a 80 y sube la FC a 130. Observa cómo el Índice de Shock y la Ponderación ($\beta$) se disparan.
•	6. Soporte y Validación
Este monitor es una herramienta de soporte a la decisión y fines educativos. Todos los cálculos están basados en coeficientes de regresión logística estándar para hemodinámica crítica.
Dataflow IA Salud Inteligente, Decisiones Precisas. www.dataflowia.com
 





Rodrigo Cárcamo Hurtado
CEO DataflowIA
