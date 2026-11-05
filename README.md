# Modelos dinámicos interactivos

Dos herramientas para visualizar modelos dinámicos de economía, hechas en un solo archivo HTML cada una. No necesitan instalar nada ni conexión a internet: se abren con doble clic en cualquier navegador.

## Contenido

| Archivo | Qué es |
|---|---|
| [`telarana.html`](telarana.html) | Modelo de la telaraña: oferta rezagada, con equilibrio convergente o divergente oscilante |
| [`diagrama-fases.html`](diagrama-fases.html) | Diagrama de fases de un sistema de dos ecuaciones diferenciales, al estilo de los libros de texto |
| [`index.html`](index.html) | Página de inicio con enlaces a las dos |

## Modelo de la telaraña (`telarana.html`)

Modelo con demanda `Qᵈₜ = α − β pₜ` y oferta `Qˢₜ = −γ + δ pₜ₋₁`.

- Tres vistas: telaraña, diagrama de fases (`pₜ` contra `pₜ₊₁`) y trayectoria temporal.
- Sliders para α, β, γ, δ, p₀ y la cantidad de períodos (hasta 30).
- El título cambia solo: convergente oscilante si δ < β, divergente oscilante si δ > β.
- Casilla para que p₀ se calcule automáticamente: lejos del equilibrio si converge, cerca si diverge.
- Casilla para permitir o no precios negativos.
- Zoom con la rueda, arrastrar para mover y doble clic para restablecer.

## Diagrama de fases (`diagrama-fases.html`)

Sistema `x′ = u(x, y)`, `y′ = v(x, y)`.

- Seis casillas de tipo de equilibrio (nodo estable e inestable, foco estable e inestable, punto silla y vórtice) que asignan automáticamente los parámetros a, b, c y d.
- Los sistemas por defecto son lineales: `x′ = a(x−4) + b(y−3)`, `y′ = c(x−4) + d(y−3)`, con el equilibrio E en (4, 3).
- Se puede escribir un sistema propio, incluso no lineal, y la herramienta busca los equilibrios y los clasifica.
- Muestra la traza, el determinante y las raíces de cada equilibrio.
- Nulclinas (`x′ = 0` e `y′ = 0`), signos, flechas de dirección por región y tangentes punteadas, cada uno con su casilla.
- Trayectorias automáticas, una por cada comportamiento distinto, y trayectorias desde los puntos A, B y C, que se arrastran con el mouse.
- Zoom con la rueda, arrastrar el fondo para mover y doble clic para restablecer.

En las fórmulas se usa `*` para multiplicar y `^` para potencias. Funciones disponibles: `sin`, `cos`, `tan`, `exp`, `ln`, `sqrt`, `abs`, `pi`.

## Cómo usarlo

**En local:** descargá el repositorio y abrí `index.html` (o cualquiera de los dos archivos) en el navegador.

**En línea con GitHub Pages:** https://tomashannon.github.io/Modelos-economia/
