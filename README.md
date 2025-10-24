# Proyecto-Final-Sistemas-Operativos
**Simulador de Algoritmos de Planificación de Procesos**
Una aplicación gráfica en Java que simula algoritmos de planificación de procesos en tiempo real con una interfaz visual intuitiva.

**🚀 Características**
Simulación en Tiempo Real: Visualización dinámica de la ejecución de procesos

Múltiples Algoritmos:

FCFS (First-Come, First-Served)

SJF (Shortest Job First)

Round Robin con quantum configurable

Interfaz Gráfica Moderna: Diseño limpio y coloreado para mejor experiencia

Métricas de Rendimiento: Cálculo automático de tiempos de retorno, espera e índices de servicio

Visualización Avanzada: Tabla de simulación con coloreo dinámico de estados

**📋 Requisitos**
Java 8 o superior

Sistema operativo: Windows, Linux o macOS

**🛠️ Instalación y Ejecución**
Clonar el repositorio:

**bash**
cd simulador-planificacion
Compilar el proyecto

**bash**
javac SimuladorPlanificacion.java
Ejecutar la aplicación:

bash
java SimuladorPlanificacion
**📖 Cómo Usar**
**1. Configurar Procesos**
Ingresa el nombre del proceso

Especifica el instante de llegada (unidades de tiempo)

Define el tiempo de CPU requerido

Selecciona el algoritmo de planificación

**2. Algoritmos Disponibles**
🔹 FCFS (First-Come, First-Served)
Ejecuta procesos en orden de llegada

No requiere quantum

🔹 SJF (Shortest Job First)
Prioriza procesos con menor tiempo de CPU

Política no apropiativa

🔹 Round Robin
Usa quantum para tiempo compartido

Configurable por el usuario

Muestra cola de procesos en tiempo real

**3. Iniciar Simulación**
Haz clic en "▶ Iniciar Simulación"

Observa la ejecución en tiempo real

Los procesos se colorean dinámicamente:

**🟢 Verde: Proceso en ejecución**

**🟡 Amarillo: Instante de llegada**

**4. Analizar Resultados**
La aplicación calcula automáticamente:

Tiempo de finalización

Tiempo de retorno (T = tf - ti)

Tiempo de espera (Te = T - t)

Índice de servicio (I = t/T)

**🎯 Métricas Calculadas**
Métrica	Fórmula	Descripción
Tiempo de Retorno	T = tf - ti	Tiempo total en el sistema
Tiempo de Espera	Te = T - t	Tiempo esperando ejecución
Índice de Servicio	I = t/T	Eficiencia del proceso
📊 Ejemplo de Uso
Agregar procesos:

Proceso A: Llegada 0, CPU 5

Proceso B: Llegada 2, CPU 3

Proceso C: Llegada 4, CPU 2

Seleccionar algoritmo (ej: Round Robin, quantum=2)

Iniciar simulación y observar:

Secuencia de ejecución

Cola de procesos activos

Métricas finales de rendimiento

**🏗️ Estructura del Código**
Clases Principales
SimuladorPlanificacion: Clase principal con interfaz gráfica

Proceso: Representa un proceso con sus atributos

Simulador: Hilo que ejecuta la simulación en tiempo real

Componentes de la UI
Panel de configuración: Entrada de parámetros de procesos

Tabla de cola de procesos: Estado actual de procesos listos

Tabla de simulación: Visualización temporal de ejecución

Tabla de resultados: Métricas de eficiencia calculadas

Panel de estado: Información en tiempo real

**🔧 Personalización**
Ajustar Velocidad de Simulación
Modificar la constante TIEMPO_UNIDAD_MS:

java
private static final int TIEMPO_UNIDAD_MS = 3000; // 3 segundos por unidad
Modificar Colores
Los colores están definidos como constantes:

java
private static final Color COLOR_EJECUCION = new Color(46, 204, 113);
private static final Color COLOR_ESPERA = new Color(241, 196, 15);
📈 Salida Esperada
La aplicación genera:

Visualización gráfica de la línea de tiempo de ejecución

Tabla de resultados con métricas cuantitativas

Secuencia de ejecución de procesos

Promedio del índice de servicio del sistema
Asegúrate de tener Java instalado: java -version



**👨‍💻 Autor**
Desarrollado como herramienta educativa para el estudio de algoritmos de planificación de sistemas operativos.

Nota: Esta aplicación es ideal para:

Estudiantes de sistemas operativos

Profesores en clases de planificación

Entendimiento visual de algoritmos de scheduling

Análisis comparativo de políticas de planificación
