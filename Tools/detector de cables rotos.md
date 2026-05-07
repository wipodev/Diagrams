# **Rastreador de Cables por Inducción (Versión Probador de Corriente)**

Esta versión optimizada permite integrar el detector en un probador de corriente tipo punzón, utilizando la batería de 12V del vehículo para su alimentación.

## **Componentes Necesarios**

| Componente | Especificación | Función |
| :---- | :---- | :---- |
| Transistores (3) | NPN (2N3904 o BC547) | Amplificación Triple Darlington. |
| Resistencia | 1 kΩ (1000 ohmios) | Protege el LED del voltaje de 12V-14V. |
| LED | Cualquier color | Indicador visual de continuidad. |
| Carcasa | Probador de corriente tipo punzón | Estructura física y punta de prueba. |

## **Diagrama de Conexión Interna**

El montaje se basa en la configuración **Triple Darlington** para maximizar la sensibilidad:

1. **Configuración de Transistores:**  
   * Emisor del 1er transistor a la Base del 2do.  
   * Emisor del 2do transistor a la Base del 3er.  
   * El Emisor del 3er transistor se conecta al **Negativo (Masa)** del vehículo mediante el cable con caimán.  
2. **Entrada (Antena):**  
   * La Base del 1er transistor se suelda directamente a la **punta metálica (punzón)** del probador.  
3. **Salida (Indicador):**  
   * Unir los tres Colectores de los transistores y conectarlos al **Cátodo (pata corta)** del LED.  
   * Conectar el **Ánodo (pata larga)** del LED a un extremo de la resistencia de 1 kΩ.  
   * El otro extremo de la resistencia debe ir al **Positivo (+12V)** de la batería del vehículo.

## **Instrucciones de Uso en Vehículos**

Para localizar una rotura en el cableado sin pinchar el aislante, siga estos pasos:

* **Energizar el cable:** Asegúrese de que el cable sospechoso tenga voltaje (ej. encendiendo el interruptor correspondiente).  
* **Conexión de la herramienta:** Conecte el caimán a tierra (chasis) y el cable de alimentación al positivo de la batería.  
* **Rastreo:** Deslice la punta del punzón sobre el aislante del cable. El LED brillará mientras detecte el campo eléctrico.  
* **Localización:** En el punto exacto donde el LED se apague, se encuentra la rotura interna del cobre.

*Nota: El uso de la resistencia de 1kΩ es crítico para evitar daños al circuito debido a los picos de voltaje del sistema eléctrico del vehículo.*