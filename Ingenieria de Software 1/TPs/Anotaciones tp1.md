## Anotaciones TP1

### Yacimiento
- Se divide en parcelas de 1 hectárea.

### Recervorio
Tiene un valor de producto en m3:
- % agua
- % gas
- % petroleo

### Parcela
- Cada una tiene un **único reservorio**. Este se encuentra a una profundidad (en metros).
- Puede a lo sumo excavarse un único pozo.
- Para cada día se decide si se extrae producto o no (no puede abrirse el día que se construyó).
- Cantidad *potencial* de producto (en m3) está dado por la fórmula *1* (pág 1).


### RIGS
- Tiene un poder de excavasión: metros/día.
- Tiene un costo diario de alquiler (que varía). Y un mínimo de días de alquiler.
- En un día puede ser usado en un único pozo.
- Consumo de combustible: litros/día.
- Su rendimiento cambia según el terreno:
  - Rocoso: 60%
  - Arenoso: 110%

### Plantas Separadoras
- Todos los pozos deben estar conectados a al menos una de estas plantas.
- Separan los componentes del producto.
- Su construcción lleva días o meses, tiene un costo.
- Procesan cierta cantidad de m3 de producto por día.
- Una vez que se separa el petroleo se vende (automáticamente).

### Tanques de almacenamiento
- Almacenan agua y gas.
- Su construcción tiene un costo y tiempo.
- Tienen una capacidad máxima.
- El gas almacenado puede venderse.

### Reinyección
- Puede inyectarse agua comprada (precio por m3).
- Puede inyectarse gas y agua de un tanque de almacenamiento.
- Valor de la presión luego de reinyectar: fórmula 3, pág 3.
- Cuando se reinyecta, no se puede extraer nada de ningún pozo ese mismo día.
- Nueva composición del producto (luego de reinyectar): fórmulas 4, pág 4.



El producto sale con una fuerza determinada del pozo que depende de la parcela (presión inicial de boca de poco P_{bc t_{0}})

### Parámetros
- Cantidad máxima de RIGS a utilizarse simultáneamente.
- Alpha1 y Alpha2 de la fórmula de *cantidad potencial de producto extraído* (fórmula 1, pág 1).
- Plantas separadoras y en qué momento se construye cada una.
- Tanques de almacenamiento, capacidad y en qué momento se construye cada uno.
- Valor del gas almacenado en tanques (precio por m3).
- Valor de presión crítica: indica cuándo es conveniente reinyectar.
- Valor de dilusión crítico: es un porcentaje de petroleo. Si un pozo baja este porcentaje, llega a su fin operativo.
- Parcelas que se quiere excavar y a qué plantas van conectadas.
- En qué momento se excavan los pozos.
- Cuántos pozos disponibles se usan para extraer día a día. Por ejemplo, todos; n que tengan mayor presión; aleatorio.
- Condiciones de fin.



## Preguntas
- ¿Un tanque sirve para almacenar solo un componente? En caso negativo, ¿la capacidad máxima de los tanques de almacenamiento es m3 de agua y gas (juntos)?
- ¿Puede no haber un tanque de almacenamiento?
- ¿El agua de los tanques de almacenamiento se puede tirar?
- ¿La venta de gas en tanques de almacenamiento hace que quede sólo agua?
- Dice que se puede reinyectar agua y gas almacenados en los tanques, ¿cómo puede darse esto? Por ejemplo, reinyectar todo lo que hay en un tanque, solo una parte, varios tanques, etc.
- ¿Las parcelas elegidas para perforar son pasadas por parámetro o se pasa todo el yacimiento y se pasa una forma de elección? Por ejemplo, las 4 parcelas con reservorio mas cercano y con terreno mas accesible.
- ¿Conviene pensar en parámetros por día o en formas de decisión? Por ejemplo, *en qué pozos se extrae por día* o *con qué criterio seleccionarlos*. (entre unos ciertos criterios dados).
- Idem reinyección.
- Idem condiciones de fin.
