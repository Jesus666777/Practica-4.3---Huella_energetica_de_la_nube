# Resultado: lo que entendí en la práctica

## Idea principal

Usar internet parece gratis, pero cada video, foto guardada o pregunta a una IA se procesa en centros de datos que gastan electricidad y agua. Ese costo no está en lo que pago, así que es una **externalidad**: lo paga la sociedad y el ambiente, no quien lo usa ni la empresa que da el servicio.

## Lo que hice

1. Investigué qué es una externalidad y cómo se internaliza un costo (por ejemplo, con un impuesto al carbono).
2. Busqué cuánta energía gasta una hora de streaming en 2 fuentes: IEA (≈0.08 kWh) y Shift Project corregido (≈0.78 kWh). Difieren porque suponen dispositivos, redes y calidad de video distintos.
3. Busqué el factor de emisión de México: 0.444 kg CO₂e por kWh (SEMARNAT, 2024).
4. Revisé mi tiempo de pantalla y saqué mi promedio diario por tipo de uso.
5. Armé el flujo en Make: página web → webhook → Make AI Agent → webhook response → página.
6. Probé la página con mis datos.

## Mi resultado

Mi uso digital genera cerca de **358 kWh al año** y **159 kg de CO₂e**. La actividad que más pesa es el **video**, sobre todo por las horas de TikTok y YouTube.

## Qué tan confiable es

Es una estimación, no un dato exacto. La IA usa valores promedio que cambian mucho según la fuente (hasta casi 10 veces en el video). Además mezcló unidades: usó kWh por hora en varias actividades, pero en la nube usó kWh por GB al mes. Por eso sirve para ver el orden de magnitud, pero hay que verificar las suposiciones.

## Cómo se podría internalizar este costo

- Impuestos a la energía o a las emisiones de los centros de datos.
- Obligar el uso de energía renovable y reportar el consumo de energía y agua.
- Precios o planes que muestren el costo de lo que se consume.

## Lo que puedo hacer yo

Bajar la calidad del video cuando no se necesita, escuchar música como audio, borrar archivos que ya no uso y usar la IA solo cuando aporta algo.
