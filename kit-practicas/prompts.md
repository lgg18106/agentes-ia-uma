# Encargos para copiar y pegar

Todos los encargos de los cuadernos de prácticas, en el orden en que aparecen. Copia el bloque entero y pégalo en el agente que diga el cuaderno. En la Sesión 1, en Antigravity, salvo los que dicen “Escribe a Claude”, que van a claude.ai con los ficheros adjuntos. En la Sesión 2, en GitHub Copilot, con la carpeta kit-practicas adjunta a la conversación. Si trabajas con Claude en el navegador, mira en el cuaderno el apartado “En el navegador (claude.ai)” de cada práctica.

---

## Sesión 1. Del chat al agente

### Práctica 1. Primer contacto

```text
¿Qué hay en esta carpeta? Explícamelo en cinco líneas, como se lo contarías a alguien que no sabe nada de informática. No cambies nada.
```

```text
Crea en esta carpeta un fichero notas.txt con esas cinco líneas. Debajo, añade la fecha de hoy y nuestros nombres, que son [escribe aquí vuestros nombres].
```

```text
¿Qué versión de R tengo instalada? Compruébalo en la terminal.
```

### Práctica 2. Tu perfil en Overleaf

```text
Convierte notas.txt en un fichero notas.tex que sea solo el cuerpo de un documento de LaTeX, sin preámbulo ni begin{document}. Empieza con un apartado titulado “Qué hay en el kit” y no uses paquetes especiales. Cuidado con los caracteres que LaTeX trata de forma especial, como el guion bajo.
```

### Práctica 3. Del Excel a R

```text
/plan En 01-presupuestos/datos hay seis ficheros de Excel, uno por año de 2019 a 2024, con las liquidaciones de los presupuestos de 20 municipios. El LEEME de 01-presupuestos explica las variables. Quiero saber cómo ha evolucionado el gasto no financiero entre 2019 y 2024.

Hazlo con un programa en R que use el paquete readxl. Guárdalo como 01-presupuestos/analisis.R y ejecútalo con Rscript. No modifiques los Excel originales.

El programa debe unir los seis años en una sola tabla y mostrar el gasto total de cada año.

Antes de darme el resultado, dime cuántas filas has leído de cada fichero y avísame de cualquier cosa rara que veas en los datos.
```

*Comentario para el plan*

```text
Si falta algún dato, no lo rellenes ni lo estimes. Déjalo vacío y avísame.
```

### Práctica 4. Caza el error

```text
Actúa como auditor de datos. Revisa los seis Excel originales y el programa analisis.R. Para cada pregunta de esta lista, dime qué has comprobado, qué has encontrado y si el programa lo resuelve:
1. ¿Hay 20 municipios cada año?
2. ¿Están todos los importes en la misma unidad?
3. ¿Hay filas repetidas?
4. ¿Algún municipio aparece escrito de dos maneras?
5. ¿Hay algún valor imposible o muy sospechoso?
6. ¿Se han leído bien todos los ficheros (filas de título, números guardados como texto)?
7. ¿Hay filas que no son datos?
```

*Escribe a Claude*

```text
Actúa como auditor de datos. Te adjunto un programa en R, analisis.R, que une seis ficheros de Excel con las liquidaciones de los presupuestos de 20 municipios, y los seis ficheros. Busca errores en el programa y problemas en los datos que el programa no resuelva. Para cada uno, dime dónde está y cómo comprobarlo. No reescribas el programa entero.
```

```text
Corrige analisis.R con todo lo que hemos encontrado. No rellenes ningún dato que falte. Guarda los datos limpios en 01-presupuestos/presupuestos_limpio.csv, con una fila por municipio y año, y dime cuántas filas tiene y cuántos municipios hay cada año.
```

### Práctica 5. Tablas para Overleaf

```text
En 01-presupuestos/presupuestos_limpio.csv están los datos limpios de los presupuestos. Escribe un programa en R, 01-presupuestos/tablas.R, que use el paquete knitr para crear dos tablas de LaTeX con el estilo booktabs y las guarde en la carpeta 01-presupuestos/tablas.

La primera, tabla_gasto_por_anio.tex, con el gasto no financiero total de cada año en millones de euros, el gasto por habitante y el número de municipios que entran en cada año.

La segunda, tabla_top10_2024.tex, con los diez municipios que más gastan por habitante en 2024.

Números con punto de millar y coma decimal. Ejecuta el programa y, al terminar, enséñame las dos primeras filas de cada tabla y dime qué tengo que añadir a mi documento de Overleaf para usarlas.
```

---

## Sesión 2. Tu agente, a medida

### Puesta a punto. Copilot en diez minutos

```text
Trabaja siempre dentro de la carpeta que te adjunto y deja en ella todo lo que crees. Para empezar, dime la ruta completa de esa carpeta y explícame en cinco líneas qué hay dentro, como se lo contarías a alguien que no sabe nada de informática. No cambies nada.
```

### Práctica 6. La calculadora del IFRU

```text
Trabaja siempre dentro de la carpeta que te adjunto y sigue las normas de plantillas/AGENTS.md.

En 05-calculadora/especificacion.md se describe un impuesto ficticio, el IFRU. Quiero una página web, calculadora.html, que se abra en el navegador con doble clic, pida los ingresos y el alquiler y calcule el impuesto como dice la especificación, con el desglose por tramos. Guárdala en la carpeta 05-calculadora/resultados.

Antes de crear nada, lee la especificación, dime en cinco líneas cómo lo vas a hacer y espera a que te lo apruebe.
```

```text
Añade a la página un botón “Ejecutar pruebas” que compruebe los diez casos de 05-calculadora/pruebas.csv y diga cuáles pasan y cuáles no, céntimo a céntimo. Si alguno falla, no cambies las pruebas. Explícame por qué falla y corrige la calculadora.
```

### Práctica 7. El informe de una página

```text
Trabaja siempre dentro de la carpeta que te adjunto y sigue las normas de plantillas/AGENTS.md.

Prepárame un informe de una página para el equipo de gobierno de la Diputación sobre cómo ha evolucionado el gasto municipal por habitante entre 2019 y 2024. Los datos limpios están en 06-skill-informe/presupuestos_limpio.csv.

Sigue al pie de la letra el manual de estilo 06-skill-informe/manual_estilo.md y usa la plantilla 06-skill-informe/plantilla_informe.md. Calcula las cifras con código, no de cabeza (con R si está instalado y, si no, con lo que haya en el ordenador). Deja el informe en 06-skill-informe/resultados.
```

### Práctica 8. Instrucciones escondidas

```text
Trabaja siempre dentro de la carpeta que te adjunto. Lee los cuatro documentos de la carpeta 04-documentos y prepara una tabla que compare las propuestas para reducir el abandono en primer curso. Para cada medida, indica quién la propone, cuánto cuesta y qué pruebas hay de que funcione. Después, recomienda las tres medidas que te parezcan mejores y explica por qué.
```

### Reto A. La voz de los estudiantes

```text
Trabaja siempre dentro de la carpeta que te adjunto y sigue las normas de plantillas/AGENTS.md.

En 03-encuesta/encuesta_satisfaccion.csv hay 120 respuestas de una encuesta de satisfacción de estudiantes. Quiero un informe de una página para el decanato con la valoración media de cada servicio, los tres temas que más se repiten en los comentarios y tres recomendaciones. Sigue el manual de estilo 06-skill-informe/manual_estilo.md.

No incluyas ningún dato personal ni copies comentarios literales. Calcula las medias con código. Deja el informe en 03-encuesta/resultados. Antes de empezar, dime el plan y espera.
```

### Reto B. Observatorio municipal

```text
Trabaja siempre dentro de la carpeta que te adjunto y sigue las normas de plantillas/AGENTS.md.

Quiero una página web, observatorio.html, que se abra en el navegador con doble clic, con un selector de municipio, un gráfico del gasto por habitante de 2019 a 2024 y una tabla con la clasificación de 2024. Los datos están en 06-skill-informe/presupuestos_limpio.csv. Añade una nota al pie que diga de dónde salen los datos y qué les falta.

Guárdala en 01-presupuestos/resultados. Antes de empezar, dime el plan y espera.
```

### El auditor

*Escribe al auditor*

```text
Actúa como auditor. Te adjunto el resultado de un trabajo que ha hecho otro agente de IA y el encargo que recibió. No lo des por bueno. Dime los tres problemas más graves que encuentres, ordenados por gravedad, y explícame para cada uno cómo puedo comprobar yo si tienes razón.
```
