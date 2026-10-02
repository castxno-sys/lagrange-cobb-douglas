# Lagrange · Cobb-Douglas

Material interactivo para la exposición del Tema 3 de Cálculo Vectorial: **multiplicadores de Lagrange** aplicados al modelo de producción de Cobb-Douglas (Stewart, sección 14.8, ejercicio 27).

El problema: maximizar `P(L, K) = b · L^α · K^(1−α)` sujeto a `mL + nK = p`, y demostrar que el máximo ocurre en

```
L* = α·p / m        K* = (1 − α)·p / n        λ = P* / p
```

## Contenido

| Archivo | Qué es |
|---|---|
| [`simulacion.html`](simulacion.html) | Gráfica 3D interactiva: superficie P(L,K), recta de restricción y punto óptimo. Los deslizadores de `b`, `α`, `m`, `n` y `p` recalculan el óptimo. Arranca con el ejemplo de la presentación: b=1, α=0.5, m=20, n=30, p=600 → (L\*, K\*) = (15, 10), P\* ≈ 12.247. |
| [`banco/index.html`](banco/index.html) | 40 preguntas con respuesta, en tarjetas, para ensayar por turnos (modo pareja, filtros por tema, repaso de las falladas). |
| [`index.html`](index.html) | Página de inicio que enlaza las dos. |

## Cómo verlo

**En línea (GitHub Pages):** https://castxno-sys.github.io/lagrange-cobb-douglas/

**En local:** son archivos HTML sin paso de compilación. Basta abrir `index.html` en el navegador, o servir la carpeta:

```bash
python3 -m http.server 8000
# luego abrir http://localhost:8000
```

La simulación carga [Plotly](https://plotly.com/javascript/) desde cdnjs y el banco carga tipografías de Google Fonts, así que necesitan conexión a internet la primera vez. Si las tipografías no cargan, el banco usa las del sistema.

## Atajos del banco de preguntas

`espacio` voltear la tarjeta · `1` la sabía · `2` hay que repasarla · `←` `→` navegar.
