# 💰 Calculadora Salario España 2026

- [💰 Calculadora Salario España 2026](#-calculadora-salario-españa-2026)
  - [⚠️ Descargo de responsabilidad](#️-descargo-de-responsabilidad)
  - [🚀 Uso](#-uso)
  - [🧮 Características](#-características)
  - [⚙️ Modelo de cálculo](#️-modelo-de-cálculo)
  - [🤝 Cómo contribuir](#-cómo-contribuir)
  - [📄 Licencia](#-licencia)

Calculadora web para estimar el salario bruto y neto anual y por paga en España, con modo individual o comparativo entre varios escenarios.

La aplicación **funciona completamente offline y es 100% privada**: todos los cálculos se realizan en el lado del cliente, es decir, en tu navegador, sin enviar ni recibir datos de servidores externos.

## ⚠️ Descargo de responsabilidad

Los resultados proporcionados por la herramienta son **meramente orientativos** y **no constituyen asesoramiento fiscal**. Esta herramienta no sustituye a un gestor o asesor fiscal profesional. Las normativas pueden cambiar y cada caso personal (ingresos del cónyuge, discapacidad, deducciones autonómicas específicas, etc.) puede alterar significativamente el resultado real.

**Consulta siempre con un profesional antes de tomar decisiones económicas.**

## 🚀 Uso

1. Descarga el archivo [calculadora_salario.html](calculadora_salario.html) y ábrelo en tu navegador, o visita la versión alojada en mi servidor:

   [https://sh.juanje.net/salario](https://sh.juanje.net/salario)

2. Elige el modo de entrada con el selector superior: `bruto anual` o `neto por paga`.
3. Ajusta el salario bruto anual o el neto objetivo por paga.
4. Selecciona el territorio, el tipo de contrato, el grupo de cotización, el número de hijos, si aplica familia numerosa, la edad y la situación de discapacidad.
5. Si seleccionas `5 o más hijos`, introduce además el número exacto para no perder el mínimo por descendientes adicional.
6. Elige el número de pagas al año.

En 12 pagas, el modo inverso interpreta la entrada como **neto mensual**. Si eliges 13, 14, 15 o 16 pagas, la entrada se interpreta como **neto por paga** para mantener la coherencia del cálculo anual.

Si lo deseas, puedes activar el modo **Comparar salarios** para ver entre 2 y 10 situaciones diferentes lado a lado y ajustar el número de escenarios con los botones `+` y `−`.

[![Vista previa de la calculadora](img/screenshot.png)](img/screenshot-fullpage.png)

## 🧮 Características

- Salario bruto anual ajustable entre 0 € y 300.000 €.
- Cálculo inverso del bruto anual a partir del neto mensual o del neto por paga.
- Cálculo en 12, 13, 14, 15 o 16 pagas.
- Escala diferenciada según territorio, incluyendo territorios forales y la deducción específica de Ceuta y Melilla.
- Cotización del trabajador desglosada en contingencias comunes, desempleo, formación profesional, MEI y cuota de solidaridad, con tope máximo y base mínima por grupo de cotización.
- Mínimos por descendientes con soporte para `5 o más hijos` indicando el número exacto.
- Deducción explícita por familia numerosa general o especial, con incremento por hijos adicionales sobre el mínimo estándar de la categoría.
- Ajuste del mínimo personal por edad del contribuyente.
- Tratamiento de discapacidad del contribuyente con tramos `33% al 64%`, `33% al 64% con movilidad reducida o asistencia` y `65% o más`.
- Reducción por obtención de rendimientos del trabajo y gasto deducible adicional para trabajador activo con discapacidad.
- Deducción adicional en cuota para rentas bajas vinculada al SMI 2026.
- Modo comparación para evaluar entre 2 y 10 escenarios simultáneos.
- Tema oscuro y claro y detección automática del modo preferido en la primera visita.
- Funcionamiento completamente offline, sin necesidad de conexión a Internet.

## ⚙️ Modelo de cálculo

La calculadora aplica un modelo aproximado:

- Seguridad Social del trabajador según el Régimen General 2026: 4,70% por contingencias comunes, desempleo del 1,55% o 1,60% según el contrato, 0,10% por formación profesional, 0,15% por MEI y cuota de solidaridad cuando el salario supera la base máxima anual.
- Base de cotización calculada con base máxima mensual de 5.101,20 € y base mínima mensual dependiente del grupo de cotización seleccionado.
- Rendimiento neto del trabajo: bruto anual menos Seguridad Social y 2.000 € de gastos deducibles generales, más el gasto adicional por trabajador activo con discapacidad cuando procede.
- Reducción por obtención de rendimientos del trabajo según el artículo 20 de la LIRPF para salarios bajos.
- El mínimo personal y familiar no se resta de la base sin más: se calcula la cuota completa y se descuenta el efecto del mínimo en cuota, como hace la LIRPF.
- Cuota IRPF calculada como suma de la escala estatal y la escala autonómica o foral seleccionada, incluyendo el tratamiento específico de Ceuta y Melilla.
- Deducción adicional en cuota para rentas bajas en 2026: 590,89 € hasta 17.094 € y reducción lineal hasta 20.048,45 €.
- Deducción por familia numerosa general o especial con 600 € extra por cada hijo que exceda el umbral estándar de la categoría; el límite por cotizaciones se aproxima con la cuota obrera calculada y no se modelan abono anticipado, cesiones ni devoluciones por encima de cuota.
- Cuando partes de un neto por paga, el bruto anual se estima con una búsqueda binaria sobre la misma función `IRPF + Seguridad Social` que usa el cálculo directo, evitando desajustes entre ambos modos.

El resultado mostrado es una estimación orientativa del neto anual, del neto por paga y de los porcentajes efectivos de cotización e IRPF.

## 🤝 Cómo contribuir

Originalmente hice esta herramienta para uso privado pero creo que puede ser de utilidad a otros, por eso decidí publicarla.

Si detectas un problema o quieres proponer una mejora, te animo a abrir una [pull request](https://github.com/JuanJesusAlejoSillero/calculadora-salario/pulls) con los cambios que harías o una [issue](https://github.com/JuanJesusAlejoSillero/calculadora-salario/issues) con el problema encontrado.

**¡Muchas gracias!**

## 📄 Licencia

Este proyecto se distribuye bajo la licencia **GNU Affero General Public License v3.0 (AGPL-3.0)**. Consulta el archivo [LICENSE](LICENSE) para el texto completo.
