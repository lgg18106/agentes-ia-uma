# Especificación · Calculadora del IFRU

El **Impuesto Ficticio sobre la Renta Universitaria (IFRU)** es un impuesto
inventado para esta práctica. Se parece a un impuesto real sobre la renta, pero
es mucho más sencillo.

## Cómo se calcula

1. **Base liquidable** = ingresos anuales − mínimo personal de 5.000 €.
   Si sale negativa, es 0.
2. **Cuota íntegra**: se aplica a la base liquidable esta escala por tramos.

   | Base desde | Base hasta | Tipo marginal |
   |---:|---:|---:|
   | 0 € | 10.000 € | 10 % |
   | 10.000 € | 25.000 € | 20 % |
   | 25.000 € | 50.000 € | 30 % |
   | 50.000 € | en adelante | 40 % |

   Cada tipo se aplica **solo a la parte de la base que cae dentro de su tramo**.
3. **Deducción por alquiler** de la vivienda habitual: 10 % del alquiler anual
   pagado, con un **máximo de 600 €**. La deducción nunca puede dejar la cuota
   en negativo.
4. **Cuota líquida** = cuota íntegra − deducción.
5. **Tipo medio** = cuota líquida ÷ ingresos × 100 (0 si no hay ingresos).
6. **Tipo marginal**: el tipo del tramo en el que cae el último euro de la base
   (0 si la base es 0).

## Lo que debe hacer la calculadora

- Una sola página web, `calculadora.html`, que funcione **abriéndola en el
  navegador**, sin instalar nada y sin conexión a internet.
- Dos campos: ingresos anuales y alquiler anual pagado.
- Resultados: base liquidable, cuota íntegra, deducción, cuota líquida, tipo
  medio y tipo marginal, con formato español (1.234,56 €).
- Un desglose por tramos que explique de dónde sale la cuota.

## Cómo sabremos que está bien

`pruebas.csv` contiene diez casos con su resultado correcto. La calculadora debe
reproducirlos **todos, céntimo a céntimo**.
