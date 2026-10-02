# Problem Brief

## Decisión del problema

### Problema elegido

Quien recibe dinero digital en México y necesita efectivo en mano no tiene una forma cercana, barata y segura de convertirlo, sobre todo si no tiene cuenta bancaria. Lo propusieron Raúl Vallejo y Anna Medina.

### Por qué elegimos este

- **Es un problema grande y frecuente:** México recibió US$61,791 millones en remesas en 2025 y casi la mitad de las electrónicas se cobró en efectivo. Ocurre cada vez que llega un pago.
- **Tiene un usuario concreto que hoy paga de más:** pierde entre 4 y 6% del monto, o se arriesga a un fraude en el cambio informal.
- **Cumple los criterios de la Sesión 1:** hay partes que no confían entre sí (usuario y comerciante), un intermediario que concentra la confianza (la remesadora) y valor en un historial que no se pueda alterar (la reputación del comercio).
- **Dos integrantes llegaron por separado al mismo problema**, con la misma evidencia y la misma hipótesis.

### Propuestas descartadas

| Propuesta | Propuesta por | Motivo del descarte |
| --- | --- | --- |
| *[Pendiente: propuestas del resto del equipo]* | | |

### Cómo tomamos la decisión

*[Pendiente: describir cómo llegó el equipo al acuerdo (votación, consenso tras debate u otro).]*

---

## Problem Brief

### Encabezado

**MicoPay** — cambiar dólares digitales por pesos en efectivo con alguien de tu colonia, sin que nadie tenga que confiar primero.

### Equipo y roles

| Integrante | Usuario de GitHub | Rol |
| --- | --- | --- |
| Raúl Vallejo | [vallejoraul08-debug](https://github.com/vallejoraul08-debug) | *[Pendiente]* |
| Anna Medina | [annapats](https://github.com/annapats) | *[Pendiente]* |
| *[Pendiente: resto del equipo]* | | |

**Responsable de las entregas:** *[Pendiente]*
**Canal de coordinación interna:** *[Pendiente]*

### Problema y evidencia

**Enunciado:** quien recibe dinero digital en México y necesita efectivo no tiene una forma cercana, barata y segura de convertirlo, sobre todo si no tiene cuenta bancaria.

**Contexto y alcance:** en 2025 México recibió US$61,791 millones en remesas y, de las enviadas por medios electrónicos, el 49.6% se cobró en efectivo ([Banxico](https://www.banxico.org.mx/publicaciones-y-prensa/remesas/%7BED06F2CB-06BA-2EC6-D145-73FF4579BADA%7D.pdf)). El 37% de los adultos de 18 a 70 años no tiene una cuenta de ahorro formal ([ENIF 2024](https://www.inegi.org.mx/contenidos/saladeprensa/boletines/2025/enif/ENIF2024_CP.pdf)), así que para muchos el efectivo no es una preferencia, es la única opción. A esto se suman los trabajadores independientes que cobran en dólares digitales y necesitan pesos para gastos del día.

**Frecuencia:** cada vez que llega un pago, que en remesas suele ser quincenal o mensual.

**Evidencia de costo:** el retiro en OXXO cuesta $17 MXN, tiene un tope de $3,000 MXN por referencia y la referencia vence a las 48 horas. En nuestras cuentas, una remesa de US$390 cobrada así pierde cerca de 5.5% entre tipo de cambio y comisiones. La alternativa barata, el cambio entre personas en redes o grupos de mensajería, obliga a una de las partes a mandar primero, sin a quién reclamar si la otra no cumple.

### Usuario y actores

**Usuario principal:** receptor de remesas o persona sin cuenta bancaria que recibe dólares digitales y necesita pesos en efectivo para renta, mandado o transporte. Necesita convertir su dinero cerca, rápido y sin perder una parte importante en el camino.

**Cómo lo resuelve hoy y qué le cuesta:**
1. **Ventanilla de remesas o tienda de conveniencia** (Elektra, Western Union, retiro en OXXO): traslado, fila, topes y vencimientos, y entre 4 y 6% del monto en comisiones y tipo de cambio.
2. **Cuenta bancaria y cajero:** exige la cuenta que justo le falta, y cobra comisión de cajero.
3. **Cambio informal entre personas:** más barato, pero con riesgo de perder el dinero si la otra parte no cumple.

**Otros actores:**
- **Remitente** (familiar en el extranjero o cliente): envía el dinero y absorbe la comisión de envío.
- **Remesadora o empresa de envío:** mueve el dinero, fija el tipo de cambio y concentra la confianza de ambas partes.
- **Punto de pago** (tienda de conveniencia, sucursal): entrega el efectivo, cobra su propia comisión e impone topes.
- **Comerciante de barrio** (tiendita, farmacia, café): hoy no participa, pero tiene efectivo parado en caja que podría convertir en ingreso por comisión.

### Flujo actual de valor

Recorrido de una remesa electrónica cobrada en efectivo:

1. **Remitente → remesadora:** el remitente paga el envío en dólares más una comisión.
2. **Remesadora:** convierte a pesos con su propio tipo de cambio, que incluye un margen sobre el tipo de cambio de referencia.
3. **Remesadora → punto de pago:** asigna el pago a una red de cobro (sucursal o tienda de conveniencia) y genera una referencia con vencimiento.
4. **Receptor → punto de pago:** se traslada al punto, hace fila y presenta la referencia y una identificación oficial. *Este paso responde a una obligación normativa: identificar a quien cobra, por prevención de lavado de dinero.*
5. **Punto de pago → receptor:** entrega el efectivo, descuenta su comisión y respeta su tope por operación (en OXXO, $3,000 MXN por referencia). Si el monto es mayor, el receptor necesita varias referencias o varias visitas.

**Intermediarios explícitos:** remesadora (pasos 1–3) y red de puntos de pago (pasos 3–5). Cada uno cobra y cada uno pone sus condiciones.

**Vía informal:** el receptor manda sus dólares digitales a un desconocido que le entrega pesos en efectivo, o al revés. No hay intermediario, pero una parte entrega primero sin garantía.

### Fricciones identificadas

| Fricción | Paso | Qué la causa | A quién afecta |
| --- | --- | --- | --- |
| Costo acumulado de 4–6% | 1, 2 y 5 | Comisión de envío, margen en el tipo de cambio y comisión de retiro, cobrados por intermediarios distintos. | Receptor y remitente |
| Traslado y fila | 4 | Los puntos de pago son pocos y lejanos para quien vive fuera de zonas comerciales. | Receptor |
| Topes y vencimientos | 3 y 5 | Límites por referencia y vencimiento a 48 h; montos grandes exigen varias visitas. | Receptor |
| Exclusión por no tener cuenta | Alternativa bancaria | La opción más barata exige una cuenta formal. | Receptor sin banco |
| Riesgo de fraude en el cambio informal | Vía informal | Una parte entrega primero y no hay a quién reclamar. | Receptor y contraparte |
| Efectivo ocioso | Fuera del flujo | El comerciante de barrio no tiene forma de ofrecer cambio con seguridad. | Comerciante |

### Oportunidad e hipótesis

**Oportunidad priorizada:** el riesgo de fraude en el cambio informal entre personas. El cambio entre personas ya resuelve casi todas las demás fricciones: es cercano, no tiene topes, no exige cuenta y cuesta menos que la ventanilla. Lo único que lo frena es que alguien tiene que confiar primero en un desconocido. Si se quita ese riesgo, una red de comercios de barrio podría ofrecer cambio con la cercanía y el precio de la vía informal y con la seguridad de la formal.

**Hipótesis:** *es una hipótesis, no una certeza.* Un contrato de escrow en Stellar/Soroban retendría los dólares digitales del usuario y solo los liberaría al comerciante cuando se confirme que el efectivo se entregó en mano, por ejemplo escaneando un código QR. Si el comerciante no cumple a tiempo, el dinero regresaría solo al usuario. Cada intercambio completado quedaría en un registro público que funciona como reputación del comercio.

**Qué cambiaría para el usuario:** cambiaría su dinero a unas cuadras de su casa en minutos, pagando una comisión de 1.9–2.5% que fija cada comercio en lugar de cerca de 5.5%, sin cuenta bancaria y sin arriesgarse a perder su dinero. El comerciante ganaría una comisión por el efectivo que ya tenía en caja.

### Criterio de pertinencia

Nos apoyamos en dos criterios de la Sesión 1.

**1. Se elimina un intermediario que hoy concentra la confianza.** Hoy el usuario tiene dos opciones: confiar en una remesadora, que cobra por ser la parte confiable, o confiar en un desconocido, que no da ninguna garantía. Una base de datos tradicional no resuelve esto: si MicoPay guardara los fondos y decidiera cuándo liberarlos, solo se reemplazaría a la remesadora por otra empresa en la que hay que confiar. Con un contrato de escrow en una red pública, la regla de liberación (entrega confirmada o devolución al vencer) está escrita en código que cualquiera puede revisar, y ni el usuario, ni el comercio, ni MicoPay pueden quedarse con el dinero por su cuenta.

**2. Partes que no confían entre sí comparten un histórico que no puede alterarse.** El usuario elige a un comercio que no conoce. Lo que le da confianza es saber cuántos intercambios ha completado ese comercio. Si ese historial viviera en la base de datos de una empresa, la empresa podría editarlo o borrarlo. En un registro distribuido, cada intercambio queda escrito de forma permanente y verificable por cualquiera, así que la reputación no depende de que alguien la administre honestamente.

Una integración entre sistemas existentes tampoco alcanza: los sistemas de remesas y bancos son justo los intermediarios de los que este usuario está excluido o que le cobran de más.

### Supuestos y riesgos

**Supuesto 1: hay comercios de barrio dispuestos a ofrecer el servicio.** Tienen que tener efectivo suficiente en caja, aceptar cobrar en dólares digitales y ver la comisión como un ingreso que vale la pena. *Lo invalidaría* que el efectivo disponible sea muy poco, o que el comercio no quiera quedarse con dólares digitales y prefiera no participar.

**Supuesto 2: el usuario puede recibir dólares digitales y usar una app.** El flujo supone que la remesa o el pago llega como stablecoin a una billetera en el teléfono del receptor. *Lo invalidaría* que los remitentes no tengan una forma fácil y barata de enviar en stablecoins, o que el receptor no tenga un teléfono con internet o no se sienta seguro usando la app.

**Supuesto 3: el modelo cabe en la regulación mexicana.** Un comercio que entrega efectivo a cambio de dólares digitales podría quedar sujeto a reglas de prevención de lavado de dinero o a requisitos para operar con activos virtuales. *Lo invalidaría* que esas obligaciones hagan inviable que un comercio pequeño participe, o que exijan identificar a cada usuario con un costo que borre el ahorro frente a la ventanilla.

**Riesgo adicional:** si la comisión final, sumando la del comercio y la de la red, no queda claramente por debajo del 4–6% actual, el usuario no tiene motivo para cambiar de hábito.
