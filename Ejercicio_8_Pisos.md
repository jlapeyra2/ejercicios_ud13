Piso(puerta#, dni, nombre, apellidos, dirección, código_postal, localidad, provincia, teléfono)

Cargo(código_cargo, nombre, funciones)

Ostenta(puerta# [REF Piso], código_cargo [REF Cargo], fecha_posesión)

Anotación(código_anotación#, fecha, importe)

IngresoRecibo(código_anotación#, fecha, importe, mes, pagado, puerta [REF Piso])

DetalleRecibo(número_línea#, concepto, importe)

IngresoExtra(código_anotación#, fecha, importe, concepto)

TipoGastoFijo(código_tipo_gasto#, nombre, descripción)

GastoFijo(código_anotación#, fecha, importe, fecha_inicio, fecha_fin, consumo, código_tipo_gasto [REF TipoGastoFijo])

GestoVariable(código_anotación#, fecha, importe, fecha_factura, concepto, número_factura)



