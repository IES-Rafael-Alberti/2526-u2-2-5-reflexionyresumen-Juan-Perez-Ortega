# RESPUESTAS — Reflexión y Resumen (Plantilla genérica)

> **Nombre y apellidos: Juan Pérez Ortega**  
> **Iniciales: JPO**  
> **Grupo:G4**  
> **Actividad / ID: 2.a..e**  
> **Unidad / Tema: Reflexión y Resumen sobre la Unidad**  
> **Fecha de entrega: 23/02/2026** 

---

## 1) Reflexión crítica (preguntas)

Responde con **lenguaje técnico** y **argumentos** (no solo opiniones). Si procede, usa ejemplos, riesgos y decisiones justificadas.

### 1.1) ¿Qué te han parecido los temas tratados en la unidad?

He visto que es una unidad fundamental ya que nos enseña que la ciberseguridad no es solo tener los programas instalados. La Taxonomía es lo que nos permite que cuando estamos recibiendo un ataque como por ejemplo el SOC se entienda a que nos enfrentamos y que prioridad tienen. Sin esta estructura, el triaje sería subjetivo y perderíamos un tiempo bastante crítico.

### 1.2) ¿Qué ha sido más útil para tu futuro puesto de trabajo? ¿Por qué?

Lo más útil ha sido poder llegar a entender el ecosistema del **SOC** y del **SIEM**. Un *SIEM* no solo sirve para poder guardar logs también sirve para poder detectar los ataques que pueden sufrirse en tiempo real. En el futuro saber como poder configurar estos casos de usos me permitira ser más eficiente a la hora de realizar el trabajo

### 1.3) ¿Qué partes ya conocías y cuáles han sido nuevas para ti?

Conocia algunos conceptos sobre tipos de virus o el firewall, pero con OSINT ha sido algo completamente neuvo, no sabía que se podía obtener tanta información técnica (como versiones de software o subdominios) de forma pasiva y legal, simplemente usando Google Dorking o Shodan. También me ha sorprendido la importancia de los IoC (Indicadores de Compromiso) para compartir inteligencia de amenazas con otros centros

### 1.4) ¿Qué concepto/idea te ha llamado más la atención y por qué?

Desde mi punto de vista es la diferencia entre Peligrosidad e Impacto. Podemos poner un ejemplo como hacer pruebas en un ejercito en donde vemos que usan armas reales donde la pelogrosidad es alta en si pero su impacto es nulo ya que se hace en un lugar controlado pero imaginemos que un empleado de la limpieza desenchufa un servidor por un descuido, la peligrosidad como podemos ver es baja pero el impacto es crítico, por lo que podemos ver como llevar a cabo la seguridad en una empresa es algo que debemos de tener en cuenta.

### 1.5) ¿Qué parte recortarías o simplificarías si hubiera menos tiempo? Justifica.

Simplificaría el apartado de herramientas específicas de análisis forense avanzado. Son vitales si pero para un analista de Nivel 1 del SOC lo prioritario es el monitoreo, triaje y contención inicial. 

### 1.6) ¿Qué tema has echado en falta o ampliarías? Justifica.

En falta no he visot nada en si pero si ampliaría la integración de Cloud SIEM y entornos multi-cloud. Dado que la superficie de ataque se ha expandido fuera del perímetro tradicional, profundizar en cómo recolectar y correlacionar logs de infraestructuras como Azure o AWS es crítico para no dejar puntos ciegos en la visibilidad del SOC moderno.

### 1.7) ¿Qué aplicarías “mañana” en un entorno real con recursos limitados?

Una cosa que aplicaria que ya que la siento en falta sería el uso de fuentes OSINT y reglas de IoC gratuitas. Por ejemplo, sin presupuesto para obtener herramientas caras pues puedes usar plataformas como MISP (Malware Information Sharing Platform), para hablar de manera breve y por que la introduciria es por el hecho de facilitar el intercambio de amenazas.

### 1.8) ¿Qué duda, riesgo o punto crítico te queda abierto tras la unidad?

Me preocupa el riesgo de los falsos positivos. Si configuramos un SOAR para que bloquee IPs automáticamente y la regla está mal hecha, podríamos causar una denegación de servicio a nuestros propios clientes legítimos. El equilibrio entre automatizar para ganar velocidad y mantener el criterio humano para no cometer errores es el punto más crítico que veo


## 2) Resumen esquematizado (obligatorio)

1. **Dimensiones de la seguridad:** Aqui podemos ver la clasificación de los sistemas según las dimensiones **C-I-T-A-D** (Confidencialidad, Integridad, Trazabilidad, Autenticidad y Disponibilidad). Tambien los niveles de impacto que los clasificamos en *Bajo, Medio y Alto*.

2. **Taxonomía:**  Lo que hace es acutar como un lenguaje común (ENISA/CCN-CERT) para clasificar las amenazas que hay y priorizar el triaje

3. **SOC y Equipos:** Esto realiza una supervisión contínua meidante diferentes niveles *L1* (Analistas de alertas) *L2* (Investigadores) y *L3* (Profesionales altamente calificados)

4. **SIEM:**  El SIEM (Security Information and Event Management) o sistema de gestión de eventos e información de seguridad. Estos dispositivos se encargan de reocger los eventos de los IDS e IPS, analizarlos y señalar alertas.

5. **SOAR:** El SOAR (Security Orchestration, Automation, and Response) lo que hace es orquestar y automatizar las respuestas mediante PlayBooks para ayudsar a los analistas a centrarse en los incidentes más complejos y dejar de lado las tareas más repetitivas.

6. **OSINT:** El OSINT (Open Source Intelligence) lo que hace es recopilar información de fuentes públicas para identificar amenazas potenciales y prevenir posibles ataques.

7. **Ciclo del Incidente:** Nos referimos como ciclo de Incidentes a cualquier evento que no es planificado o que no sea deseado que pueda comprometer la seguridad de la información en donde sigue las diferentes fases: (Preparación, Identificación, Contención, Erradicación, Recuperación y Lecciones aprendidas).

8. **Vectores de Ataque:** Identificamos los vectores en donde pueden ser por un canal de entrada como por correo, RODP, USB frente a la a otras como Phishing, Brute Force.

9. **Documentación:** Tenemos que hacer una documentacion básica del incidente en donde escrbimos el asunto la identificación de la persona afectada la fecha y hora tanto del incidente como de la detección, una descripción detalada del incidente el origen en donde sila página ha sido comprometida si hay credenciales comprometida

### 2.1) Mapa/índice de la unidad (visión global)
- 

### 2.2) Conceptos clave (lista breve)

• C-I-T-A-D: Dimensiones de seguridad: Confidencialidad, Integridad, Trazabilidad, Autenticidad y Disponibilidad.
• Peligrosidad vs. Impacto: La peligrosidad reside en la naturaleza de la amenaza; el impacto, en las consecuencias reales para el negocio.
• IoC (Indicador de Compromiso): Evidencia técnica (hash, IP, dominio) que confirma una intrusión.
• Triaje: Proceso de validación y priorización de alertas para descartar falsos positivos.
• Vector de ataque: El canal o medio por el que el atacante contacta con el sistema

### 2.3) Procesos / procedimientos (pasos o checklist)

Los procedimientos que podemos llevar a cabo son los siguientes

**El ciclo de vida de un incidente:**

1. **Preparación:** Establecer políticas, procedimientos, herramientas y entrenar al equipo antes de que ocurra un incidente.

2. **Identificación:** Detectar y confirmar que realmente está ocurriendo un incidente de seguridad

3. **Contención:** Aislar el problema para evitar que se propague y cause más daños

4. **Erradicación:** Eliminar la causa raíz del incidente (malware, vulnerabilidad explotada, cuenta comprometida, etc.)

5. **Recuperación:** Restaurar los sistemas y servicios a su estado operativo normal

6. **Lecciones aprendidas:** Analizar qué ocurrió, cómo se gestionó y qué podemos mejorar para el futuro

También podemos ver el proceso de **OSINT:**

El proceso de OSINT tiene estas fases:

1. **Planificación y dirección:** definir objetivos y alcance.

2. **Identificación de fuentes:** elegir fuentes fiables y relevantes.

3. **Adquisición:** recopilar datos sin exceder lo necesario.

4. **Procesamiento:** limpiar, ordenar y priorizar.

5. **Análisis:** convertir datos en conclusiones.

6. **Difusión:** presentar resultados de forma clara y útil.

## 2.4) Herramientas / técnicas (si aplica)

| Categoría | Herramientas / Técnicas | Función Principal |
| :--- | :--- | :--- |
| **Monitorización** | **SIEM** (Splunk, Sentinel, QRadar) | Recolección, correlación de logs y alertas. |
| **Respuesta** | **SOAR** (Cortex XSOAR, Phantom) | Orquestación y automatización mediante *playbooks*. |
| **Protección Red** | **IDS/IPS** (Snort, Suricata) | Detección y prevención de intrusiones. |
| **Endpoint** | **EDR** (CrowdStrike, SentinelOne) | Detección y respuesta en dispositivos finales. |
| **OSINT** | **Shodan, Maltego, FOCA** | Búsqueda de dispositivos, relaciones y metadatos. |
| **Investigación** | **Google Dorking** | Búsqueda avanzada mediante operadores (`site:`, `filetype:`). |

### 2.5) Buenas prácticas y errores típicos

Buenas prácticas:

• Triaje basado en peligrosidad e impacto: Debemos de diferenciar entre peligrosidad e impacto para priorizarlos de manera eficiente.

• Documentar en tiempo real: Es importante empezar a registrar las evidencias y las acciones desde el momento en el que el incidente sucede.

• Verificación Post-Incidente: Hay que mantener una monitorizacion intensiva que debe de durar de 3 a 2 semanas para evitar que el incidente se repita.

Errores típicos:

• Confundir entre hechos e hipótesis: En los informes por ejemplo no podemos dar por sentado las suposiciones que se hagan o cualquier hecho que no esté contrastado. Cualquier hallazgo que se saque debe de estar verificado en los logs por ejemplo.

• Falta de gestión de falsos positivos: Un SIEM que está mal configurado puede generar falsos positivos esto puede provocar que incidentes reales no sean "visibles"  

• Improvisación: No hay que seguir los playbooks o runbooks establecidos durante una crisis.

### 2.6) Glosario mínimo (términos y definiciones cortas)

• **SIEM**: Gestión de eventos e información de seguridad.

• **SOAR**: Orquestación, automatización y respuesta de seguridad.

• **IoC** (Indicador de Compromiso): Evidencia técnica (IP, hash) de un ataque.

• **Falso Positivo**: Alerta errónea causada por una actividad legítima.

• **Triaje**: Proceso de validar y priorizar alertas según peligrosidad e impacto.

• **Playbook**: Conjunto de pasos predefinidos para responder a un incidente.


## 3) (Opcional) Evidencias y recursos usados


## 4) Conclusión (cierre)

La conclusión a la que uno puede llegar que la defensa, el éxito de esta depende de la capacidad de las personas para hacer una buena documentación de todo lo sucedido, o aplicar un trabajo excelente en **OSINT** y también se debe de aprender de cada ataque para cerrar cualquier brecha de seguridad y poder prevenir en un futuro porisbles ataques, debemos de entender que esto es lo mas importante y  no depender solo de las herramientas como puede ser el **SIEM** o el **SOAR**.
