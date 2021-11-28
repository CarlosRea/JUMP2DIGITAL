# JUMP2DIGITAL | Reparto a domicilio

## Sobre JUMP2DIGITAL

Barcelona Digital Talent organiza JUMP2DIGITAL, el primer evento de referencia del talento digital en Barcelona impulsado por Mobile World Capital Barcelona, Ayuntamiento de Barcelona, Generalitat de Catalunya y ACCIÓ , dónde podrás conocer las tecnologías y profesiones digitales más emergentes en este ecosistema, poner a prueba tus habilidades digitales a través de actividades de reclutamiento y conectar con las empresas que están liderando la digitalización del sector.

En este evento tendrá lugar un Hackathon dónde empresas del hub tecnológico de Barcelona buscarán nuevos profesionales con perfil de Frontend, Backend y Data para incorporarlos a sus compañías. ¿Te lo vas a perder? Participa en la primera fase del Hackathon que tendrá lugar del 22 – 28 de noviembre y, si eres una de las 80 personas seleccionadas, conseguirás una plaza en la competición presencial que organizaremos el 10 de diciembre en La Llotja de Barcelona.

## Reto a desarrollar para la fase online
Akadelivers es una empresa de reparto a domicilio especializada en la entrega de paquetes en menos de 1 hora, lo que se denomina (Q-commerce = Quick commerce) Esta empresa tiene una aplicación móvil con la que sus usuarios pueden elegir entre un catálogo de productos de tiendas locales de su ciudad y que les sean entregados en menos de 10 minutos a la dirección que deseen.

Cuando un usuario pide un pedido a través de Akadelivers se le cobra directamente el coste total (coste del producto + gastos de servicio + gastos de envío). Una vez el usuario ha pagado un producto, el repartidor que se encuentre más próximo a la tienda que tiene el producto se acerca a esta, paga el producto, lo recoge y lo lleva a la dirección que el usuario ha elegido. Akadelivers se lo llevara a la dirección indicada.

## Datasets
Variables del dataset:

- order_id: Número de identificación del pedido.

- local_time: Hora local a la que se realiza el pedido.

- country_code: Código del pais en el que se realiza el pedido.

- store_address: Número de tienda en a la que se realiza el pedido.

- payment_status: Estado del pedido.

- n_of_products: Número de productos que se han comprado en ese pedido.

- products_total: Cantidad en Euros que el usuario ha comprado en la app.

- final_status: Estado final del pedido (este será la variable 'target' a predecir) que indicara si el pedido será finalmente entregado o cancelado. Hay dos tipos de estado:

  - CanceledStatus: La entrega se ha cancelado.
  - DeliveredStatus: La entrega se ha realizado correctamente.

Archivos:

- train.csv: Este dataset contiene tanto las variables predictoras como el estado del pedido (TARGET).
- test_X.csv: Este dataset contiene las variables predictoras con las que se tendrá que predecir el estado de un pedido.
- ejemplo_predicciones.csv: Este dataset es un ejemplo de como se debera entregar las predicciones del objetivo número 6 de las tareas a relizar.


## Objetivos
Para las preguntas 1,2,3 y 4 emplea el dataset train.csv Para la pregunta 5 deberás emplear el dataset 'train.csv' y 'test_X.csv'.

¿Cuáles son los 3 paises en los que más pedidos se realizan?
¿Cuáles son las horas en las que se realizan más pedidos en España?
¿Cuál es el precio medio por pedido en la tienda con ID 12513?
Teniendo en cuenta los picos de demanda en España, si los repartidores trabajan en turnos de 8horas.
Turno 1 (00:00-08:00)
Turno 2 (08:00-16:00)
Turno 3 (16:00-00:00)
Qué porcentaje de repartidores pondrías por cada turno para que sean capaces de hacer frente a los picos de demanda. (ej: Turno 1 el 30%, Turno 2 el 10% y Turno 3 el 60%).

Realiza un modelo predictivo de machine learning a partir del dataset 'train.csv' en el cual a partir de las variables predictoras que se entregan en el dataset 'test_X' se pueda predecir si el pedido se cancelará o no (columna 'final_status').
Siendo:

Para simplificar, podeis asignar los valores 'CanceledStatus' a 0 y los valores 'DeliveredStatus' a 1.

0 = CanceledStatus
1 = DeliveredStatus
