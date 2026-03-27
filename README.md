# Animación 2D Tradicional: Ciclo de Caminata con Grease Pencil

Este repositorio documenta el desarrollo de una animación 2D realizada en **Blender**, utilizando la herramienta **Grease Pencil**. El proyecto recrea un ciclo de caminata (*walk cycle*) basado en el personaje de Luffy, aplicando técnicas de animación tradicional cuadro a cuadro.

---

## Configuración del Proyecto en Blender

Para replicar esta animación, se configuró el entorno de trabajo siguiendo estos pasos técnicos:

### 1. Preparación del Entorno 2D
* **Modo de Trabajo**: Se utilizó el entorno "2D Animation" de Blender para acceder a las herramientas de dibujo nativas.
* **Objeto Grease Pencil**: Se creó un objeto tipo "Blank" para iniciar desde cero sin trazos predeterminados.
* **Estructura de Capas**:
    * **Trazo (Lines)**: Capa superior para definir el contorno del personaje.
    * **Relleno (Fills)**: Capa inferior para aplicar los colores base sin obstruir las líneas.

### 2. Paleta de Materiales 
Se definieron materiales específicos basados en el modelo **RGB** para cuantificar el espectro lumínico del personaje:
* **01 Trazo**: Color sólido oscuro para la definición de silueta.
* **01 - 09 Rellenos**: Materiales tipo *Fill* para la piel, chaleco, pantalón y sombrero.

---

## Metodología de Animación

La animación se basa en una secuencia lineal de **7 poses clave progresivas** para lograr fluidez.

### 1. Referencia y Rasterización
* **Papel Cebolla (Onion Skin)**: Se importó una hoja de referencia con opacidad al 0.5 para servir de guía visual durante el trazado.
* **Timing**: La animación se configuró a **24 FPS**. Los dibujos se realizaron cada **3 fotogramas** para cubrir el ciclo completo en 1 segundo ($3 \times 8 = 24$).

### 2. Proceso de Dibujo
* **Herramientas de Curva**: Se utilizaron pinceles de arco y poligonales para mantener la limpieza en las extremidades.
* **Interpolación Manual**: Cada cuadro fue redibujado siguiendo la posición del anterior para asegurar la continuidad del movimiento.

<img width="1250" height="750" alt="Captura de pantalla 2026-03-26 205525" src="https://github.com/user-attachments/assets/f0755847-0a49-437f-a944-3624fca7235a" />

---

## Efectos y Post-Procesamiento

Para mejorar el acabado visual de la animación, se aplicaron los siguientes efectos en el panel de **Properties**:

* **Efecto Ribete (Rim)**: Añade una iluminación en los bordes para resaltar la silueta del personaje.
* **Sombra Proyectada (Shadow)**: Se configuró una sombra en los ejes X y Y para dar sensación de profundidad y contacto con el suelo.
* **Se hizo uso del siguiente material para lograr con exito esta práctica:**
  [Blender 2D | Animación con Grease Pencil](https://youtu.be/0myBDB1vuq0?si=uDzSnSswq3CJ-IIM)
