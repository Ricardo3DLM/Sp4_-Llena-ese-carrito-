Info. Proyecto de Sprint 4: "¡Llena ese carrito!"

Análisis de datos y data wrangling.

La base de datos contiene información sobre productos de super mercado y sus clientes.
Tablas de Datos (5):

instacart_orders.csv: cada fila corresponde a un pedido en la aplicación Instacart.
	'order_id': número de ID que identifica de manera única cada pedido.
	'user_id': número de ID que identifica de manera única la cuenta de cada cliente.
	'order_number': el número de veces que este cliente ha hecho un pedido.
	'order_dow': día de la semana en que se hizo el pedido (0 si es domingo).
	'order_hour_of_day': hora del día en que se hizo el pedido.
	'days_since_prior_order': número de días transcurridos desde que este cliente hizo su pedido anterior.

products.csv: cada fila corresponde a un producto único que pueden comprar los clientes.
	'product_id': número ID que identifica de manera única cada producto.
	'product_name': nombre del producto.
	'aisle_id': número ID que identifica de manera única cada categoría de pasillo de víveres.
	'department_id': número ID que identifica de manera única cada departamento de víveres.

order_products.csv: cada fila corresponde a un artículo pedido en un pedido.
	'order_id': número de ID que identifica de manera única cada pedido.
	'product_id': número ID que identifica de manera única cada producto.
	'add_to_cart_order': el orden secuencial en el que se añadió cada artículo en el carrito.
	'reordered': 0 si el cliente nunca ha pedido este producto antes, 1 si lo ha pedido.

aisles.csv
	'aisle_id': número ID que identifica de manera única cada categoría de pasillo de víveres.
	'aisle': nombre del pasillo.

departments.csv
	'department_id': número ID que identifica de manera única cada departamento de víveres.
	'department': nombre del departamento.


Conclusiones:

Después de hacer la limpieza de datos, gráficos para visualizarlos, e identificado el comportamiento de los clientes frecuentes,
se puede decir que los clientes prefieren porductos saludables, orgánicos, y frutas. Por el comportamiento de la mayoría de los 
clientes se podría inferir que se trata de una población muy consciente de su salud física, aunque posiblemente vegetariana. En 
ninguna lista de top 20 se observan productos de carne.

El horario de compra más popular es por lo general entre las 11:00 y las 15:00, sin importar mucho el día de la semana de acuerdo
a la comparación que se hizo entre el miércoles y el sábado.

Casi todos los clientes piden un máximo de 31 productos, siendo 8 productos por orden la mediana del muestreo. Desafortunadamente,
la gran mayoría de los clientes hace de uno a tres pedidos solamente, sería importante desarrollar estrategias de retención, como 
descuentos y/o membresías, para incentivar la fidelidad de los clientes.

Siendo que la popularidad de las bananas es incomparable, se podría usar este producto para crear estrategias de retención y retorno
de clientes.
