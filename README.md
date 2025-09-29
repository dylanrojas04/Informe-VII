# Laboratorio: Codificación Hamming (7,4) con Raspberry Pi Pico 2W

Este proyecto implementa un sistema de **codificación Hamming (7,4)** sobre los datos obtenidos del acelerómetro **MPU6050**, utilizando la **Raspberry Pi Pico 2W**.  
Los datos codificados son transmitidos por el pin **Tx (UART)** y visualizados en un **osciloscopio digital**, además de mostrarse en una pantalla **OLED SSD1306**.

---

## 📌 Objetivos
- Leer los datos del acelerómetro MPU6050 mediante I2C.  
- Dividir la muestra de 16 bits en nibbles de 4 bits.  
- Codificar cada nibble con el esquema **Hamming (7,4)** con paridad par.  
- Transmitir la trama codificada de 28 bits por **UART (Tx)**.  
- Visualizar los resultados en el **osciloscopio** y en la pantalla OLED.  

---

## ⚙️ Requisitos de hardware
- Raspberry Pi Pico 2W  
- Acelerómetro MPU6050  
- Pantalla OLED SSD1306 (I2C)  
- Osciloscopio digital  
- Jumpers y protoboard  

---

## 📂 Conclusiones
1. La implementación de la codificación Hamming (7,4) en la Raspberry Pi Pico 2W demostró ser una técnica efectiva para garantizar la detección y corrección de errores de un bit en la transmisión de datos.  
2. El uso del acelerómetro MPU6050 permitió obtener lecturas reales que, al ser procesadas y codificadas, evidenciaron la aplicabilidad de los códigos de canal en sistemas embebidos de adquisición de datos.  
3. Los resultados observados en el osciloscopio digital confirmaron que las tramas transmitidas por el pin Tx coincidieron con los datos generados en el programa, validando la correcta implementación del algoritmo.  
4. La decodificación verificó la capacidad de recuperar información íntegra incluso en presencia de alteraciones, cumpliendo con los objetivos del laboratorio.  
