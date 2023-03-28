Cliente(cod_cliente#)

Proveedor(cod_proveedor#)

Producto(cod_producto#, cantidad, cod_proveedor [REF Proveedor], unidades, fecha_encargo)

Pedido(cod_pedido#, fecha_pedido, cod_producto [REF Producto], num_unidades)