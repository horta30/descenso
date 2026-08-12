# DESCENSO

Juego web de descenso en bicicleta para **Gravitas**. Dos etapas contrarreloj:

- **Alta Montaña** — bosque de cordillera, sendero de loam.
- **Cerro Abajo** — descenso urbano en Valparaíso.

## Cómo está hecho

Un solo archivo HTML, sin dependencias, sin imágenes y sin build.
Todo el arte se genera por código al arrancar. Pesa ~30 KB comprimido.

Motor pseudo-3D por segmentos: la pista es una lista de tramos con
altura y curvatura propias que se proyectan en perspectiva. De ahí
salen las bajadas, las lomas y las curvas peraltadas.

## Cómo incrustarlo

```html
<iframe src="https://horta30.github.io/descenso/"
        style="width:100%;aspect-ratio:16/9;border:0;border-radius:12px"
        allow="fullscreen; autoplay"
        title="Descenso"></iframe>
```

## Controles

| | |
|---|---|
| ← → | inclinar y esquivar |
| Espacio | saltar |
| ↑ (desde rampa) | 360 |
| ↓ (desde rampa) | backflip |
| ← → en el aire | whip |

En celular: toca los costados para inclinar, el centro para saltar,
la mitad superior para los trucos.
