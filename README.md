# 🚗 Motores con nueva vida · Arduino Week 2026

Proyecto educativo desarrollado en el **Circular FAB Jarandilla de la Vera** dentro de la **Red de Centros de Innovación Territorial (CIT) de la Diputación de Cáceres**.

Este repositorio reúne una colección de prácticas de electrónica, robótica y fabricación digital basadas en la **reutilización de componentes**, el aprendizaje por proyectos y la documentación abierta para que puedan ser replicadas en centros educativos, talleres maker y actividades formativas.

---

## 🌐 Web del proyecto

👉 Disponible en GitHub Pages:

```txt
https://circularfabjarandilladelavera.github.io/motores-nueva-vida/
```

Sustituye la URL anterior por la dirección real del repositorio cuando actives GitHub Pages.

---

## 🎯 Objetivo

El objetivo del itinerario es avanzar desde el control básico de cargas eléctricas hasta sistemas más completos con motores, sensores, automatización y control desde navegador.

A través de las prácticas se trabajan conceptos como:

- Control de potencia.
- Inversión de giro.
- Uso de relés, MOSFET y drivers de motor.
- Sensores ultrasónicos.
- Displays y contadores.
- Alimentación externa y GND común.
- Documentación técnica con GitHub Pages.
- Reutilización de componentes electrónicos.

---

## 🧩 Prácticas incluidas

### 🚦 1. Semáforo 12V con Arduino

Control de lámparas de 12V utilizando Arduino, transistores/MOSFET y una fuente ATX reciclada.

**Componentes principales:**

- Arduino.
- Lámparas 12V.
- Fuente ATX reciclada.
- Transistores 2N222 / MOSFET IRLZ44N.
- Resistencias.
- Cableado de potencia y señal.

---

### 🔁 2. Inversor de giro con 2 relés

Práctica para invertir el sentido de giro de un motor DC mediante dos relés, trabajando la lógica de conmutación y la seguridad eléctrica.

**Componentes principales:**

- Arduino.
- Módulo de 2 relés.
- Motor DC.
- Fuente externa para el motor.
- Botones de control.
- GND común.

**Idea clave:** nunca deben activarse los dos relés simultáneamente para evitar cortocircuitos.

---

### 🚗 3. Coche WiFi con ESP32

Vehículo controlado desde el móvil mediante una página web servida por el propio ESP32.

**Componentes principales:**

- ESP32.
- Driver L298N.
- 2 motores DC.
- Sensor ultrasónico HC-SR04.
- Servo para orientar el sensor.
- Fuente externa.
- Control desde navegador.

**Nota técnica:** el pin ECHO del HC-SR04 debe adaptarse a 3.3V si se conecta al ESP32.

---

### 🚧 4. Barrera automática con Arduino Mega

Sistema de control de acceso con barrera motorizada, sensores ultrasónicos y contador de vehículos.

**Componentes principales:**

- Arduino Mega 2560.
- Motor paso a paso 28BYJ-48.
- Driver ULN2003.
- Display TM1637.
- 2 sensores ultrasónicos HC-SR04.
- Botón de reset.
- Fuente estable de 5V.

**Funcionalidad:**

- Detecta entrada y salida de vehículos.
- Abre y cierra la barrera automáticamente.
- Actualiza un contador en el display.
- Permite reset manual.
- Incluye simulador visual en la web.

---

## 📁 Estructura recomendada

```txt
.
├── index.html
├── README.md
├── LICENSE
├── .gitignore
└── assets/
    ├── logo-cf.png
    ├── esquema-inversor-reles.png
    └── otros-recursos.png
```

---

## 🚀 Publicación en GitHub Pages

1. Subir al repositorio:
   - `index.html`
   - `assets/`
   - `README.md`
   - `LICENSE`
   - `.gitignore`

2. Ir a:

```txt
Settings → Pages
```

3. Seleccionar:

```txt
Deploy from branch
```

4. Elegir:

```txt
main / root
```

5. Guardar y esperar a que GitHub genere la web.

---

## ⚠️ Notas técnicas importantes

- Los motores no deben alimentarse directamente desde Arduino o ESP32.
- Usar siempre fuente externa adecuada para motores y cargas.
- Compartir GND entre la placa de control y la alimentación externa cuando sea necesario.
- Revisar polaridades antes de conectar.
- En ESP32, adaptar señales de 5V a 3.3V.
- En relés, evitar estados peligrosos donde se puedan activar dos canales incompatibles.
- En motores paso a paso, revisar el orden de bobinas si vibra pero no gira.

---

## 🏫 Contexto educativo

Proyecto desarrollado como recurso formativo para actividades de:

- Arduino Week 2026.
- Circular FAB Jarandilla de la Vera.
- Robótica educativa.
- Electrónica aplicada.
- Fabricación digital.
- Automatización básica.
- Reutilización tecnológica.

---

## 📜 Licencia

Este proyecto está publicado bajo licencia **MIT**.

Puedes usarlo, modificarlo, adaptarlo y compartirlo libremente, manteniendo la atribución correspondiente.

---

## 🤝 Créditos

Desarrollado como material educativo en el **Circular FAB Jarandilla de la Vera**, dentro de la red de innovación territorial impulsada por la **Diputación de Cáceres**.

---

💡 **Tecnología accesible + reutilización + aprendizaje práctico.**
