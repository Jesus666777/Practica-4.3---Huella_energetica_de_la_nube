# Práctica 4.3. Huella energética de la nube

**Materia:** Desarrollo Sustentable (ACD-0908) · Instituto Tecnológico de Mazatlán
**Carrera:** Ingeniería en Sistemas Computacionales
**Unidad 4:** Escenario económico · Tema 4.3 Externalización e internalización de costos
**Alumno:** Sanchez Gamboa Jesus

## ¿De qué trata?

Una página web donde cada persona captura su uso digital (video, música, redes, videollamadas, juegos, nube, IA y correos). Una inteligencia artificial estima la energía y las emisiones que genera, explica quién paga ese costo (una externalidad) y propone 3 acciones para reducirlo.

## Cómo funciona

```
Página web (index.html) → Webhook de Make → Make AI Agent → Webhook Response → Página web
```

1. La página envía los 8 campos con `fetch` (POST) y `URLSearchParams`.
2. Make recibe los datos en un Custom webhook.
3. El Make AI Agent calcula la estimación con el factor de emisión de México (0.444 kg CO₂e por kWh, SEMARNAT 2024).
4. El Webhook Response devuelve el resultado como texto plano y la página lo muestra.

## Video

https://youtu.be/N8Nvw1KJdgU?si=qBiuvRE2WhLlqiBg

## Resultado de la prueba

| Dato | Valor |
|---|---|
| Energía por año | 358 kWh |
| Emisiones por año | 159 kg CO₂e |
| Actividad que más consume | Video |

## Contenido del repositorio

| Archivo o carpeta | Qué contiene |
|---|---|
| `index.html` | Página web con el webhook de Make |
| `codigo/` | Instrucciones y configuración del Make AI Agent y del Webhook Response |
| `documentos/` | Instrucciones originales de la práctica y el reporte en Word |
| `imagenes/` | Capturas del proceso en Make y de la página funcionando |
| `resultado.md` | Resumen de lo que aprendí en la práctica |

## Página publicada

Enlace de GitHub Pages: _pendiente de agregar_

## Herramientas

IA generativa, Make (Webhooks, Make AI Agent, Webhook Response) y GitHub Pages.
