# 💰 Calculadora Salario Neto España 2026

- [💰 Calculadora Salario Neto España 2026](#-calculadora-salario-neto-españa-2026)
  - [⚠️ Descargo de responsabilidad](#️-descargo-de-responsabilidad)
  - [🚀 Uso](#-uso)
  - [🧮 Características](#-características)
  - [⚙️ Modelo de cálculo](#️-modelo-de-cálculo)
  - [🤝 Cómo contribuir](#-cómo-contribuir)
  - [📄 Licencia](#-licencia)

Calculadora web para estimar el salario neto anual y por paga en España.

La aplicación **funciona completamente offline y es 100% privada**: todos los cálculos se realizan en el lado del cliente, es decir, en tu navegador, sin enviar ni recibir datos de servidores externos.

## ⚠️ Descargo de responsabilidad

Los resultados proporcionados por la herramienta son **meramente orientativos** y **no constituyen asesoramiento fiscal**. Esta herramienta no sustituye a un gestor o asesor fiscal profesional. Las normativas pueden cambiar y cada caso personal (ingresos del cónyuge, discapacidad, deducciones autonómicas específicas, etc.) puede alterar significativamente el resultado real.

**Consulta siempre con un profesional antes de tomar decisiones económicas.**

## 🚀 Uso

1. Descarga el archivo [calculadora_neto.html](calculadora_neto.html) y ábrelo en tu navegador, o visita la versión alojada en mi servidor:

   [https://sh.juanje.net/neto](https://sh.juanje.net/neto)

2. Ajusta el salario bruto anual.
3. Selecciona el territorio, número de hijos y rango de edad.
4. Elige el número de pagas al año.

Si lo deseas, puedes activar el modo **Comparar salarios** para ver dos situaciones diferentes lado a lado.

[![Vista previa de la calculadora](img/screenshot.png)](img/screenshot-fullpage.png)

## 🧮 Características

- Salario bruto anual ajustable entre 0 € y 300.000 €.
- Cálculo en 12, 13, 14, 15 o 16 pagas.
- Escala diferenciada según territorio.
- Mínimos por descendientes para 0 a 5 hijos.
- Ajuste del mínimo personal por edad del contribuyente.
- Deducción por obtención de rendimientos del trabajo.
- Deducción adicional para rentas bajas vinculada al SMI 2026.
- Modo comparación para evaluar dos escenarios simultáneos.
- Tema oscuro y claro y detección automática del modo preferido en la primera visita.
- Funcionamiento completamente offline, sin necesidad de conexión a Internet.

## ⚙️ Modelo de cálculo

La calculadora aplica un modelo simplificado:

- Seguridad Social del trabajador: 6,5% sobre la base anual, con tope en 58.914 €.
- Rendimiento neto del trabajo: bruto anual menos Seguridad Social y 2.000 € de gastos deducibles generales.
- Reducción por obtención de rendimientos del trabajo según el artículo 20 de la LIRPF para salarios bajos.
- El mínimo personal y familiar no se resta de la base sin más: se calcula la cuota completa y se descuenta el efecto del mínimo en cuota, como hace la LIRPF.
- Cuota IRPF calculada como suma de la escala estatal y la escala autonómica o foral seleccionada.
- Deducción adicional en cuota para rentas bajas en 2026: 590,89 € hasta 17.094 € y reducción lineal hasta 20.048,45 €.

El resultado mostrado es una estimación orientativa del neto anual, del neto por paga y de los porcentajes efectivos de cotización e IRPF.

## 🤝 Cómo contribuir

Originalmente hice esta herramienta para uso privado pero creo que puede ser de utilidad a otros, por eso decidí publicarla.

Si detectas un problema o quieres proponer una mejora, te animo a abrir una [pull request](https://github.com/JuanJesusAlejoSillero/calculadora-neto/pulls) con los cambios que harías o una [issue](https://github.com/JuanJesusAlejoSillero/calculadora-neto/issues) con el problema encontrado.

**¡Muchas gracias!**

## 📄 Licencia

Este proyecto se distribuye bajo la licencia **GNU Affero General Public License v3.0 (AGPL-3.0)**. Consulta el archivo [LICENSE](LICENSE) para el texto completo.
