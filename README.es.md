# finance-council

[Read in English](README.md)

Una skill para Claude Code que convierte a Claude en un consejo de diez especialistas senior. Le contás un negocio, una idea o un plan, pasa por todas las disciplinas y te devuelve un reporte completo. Está pensada para llevarte la contra cuando los números no cierran.

## Las diez disciplinas

Finanzas, contabilidad, administración, comercio, economía, actuaría, auditoría, estadística, tesorería y gestión de riesgos.

Cada una da su lectura. Cuando dos chocan (por ejemplo, comercio quiere bajar el precio y contabilidad dice que con ese margen no se cubre el costo fijo), el reporte lo dice en vez de promediarlas.

## Qué te devuelve

Si exponés un negocio o una idea, participan las diez disciplinas y el reporte tiene siete partes:

1. Resumen de la idea y de los supuestos que se tomaron
2. Un bloque por disciplina, cada uno cerrado con Alerta, Ojo u OK
3. Tensiones entre disciplinas
4. Números clave: break-even, capital necesario, meses de caja, tres escenarios
5. Los 5 riesgos principales con su mitigación
6. Veredicto: avanzar, avanzar con condiciones, o no avanzar todavía
7. Qué falta verificar y próximos pasos

Para una pregunta puntual (revisar un cálculo, dimensionar una posición, decidir un precio) llama solo a las 2 o 3 disciplinas que importan.

Pide números reales antes de dar una opinión con peso. Si la hacés seguir sin ellos, cada supuesto queda marcado como tal.

## Instalación

Copiá la carpeta a tu directorio de skills.

```bash
git clone https://github.com/Warriors1996/finance-council.git
cp -r finance-council/es ~/.claude/skills/finance-council-es
```

Para la versión en inglés, copiá la carpeta entera como skill propia:

```bash
cp -r finance-council ~/.claude/skills/finance-council
```

En Windows, la carpeta de skills es `C:\Users\<vos>\.claude\skills`.

## Uso

Contá la idea, sin más. Por ejemplo:

> Quiero abrir una tostaduría chica que venda café por suscripción. Qué te parece?

O pedí una sola lente:

> Revisá el tamaño de posición de mi bot de trading, tengo un backtest con 40 operaciones.

## Límites

Es un marco de análisis, no asesoramiento financiero. No te dice que compres o vendas un activo puntual, y no reemplaza a un contador o abogado para trámites impositivos o legales. Si le faltan datos, lo dice en vez de inventar cifras.

## Licencia

MIT. Ver [LICENSE](LICENSE).
