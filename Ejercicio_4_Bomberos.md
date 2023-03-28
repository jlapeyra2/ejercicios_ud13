ParqueBomberos(cod_parque#, nombre, dirección, teléfono, categoría)

Coche(num_coche#, marca, modelo, num_matrícula, fecha_compra, fecha_ult_rev, cod_parque [REF ParqueBomberos])

Equipo(cod_equipo#, nombre)

PeticiónServicio(codPetServ#, tipo_serv, gradoUrgencia, cod_eq [REF Equipo])

ParqueRecibePetición(cod_parque# [REF PrqueBomberos], codPetServ# [REF PeticiónServicio], fecha, hora)

Bombero(cod_bom#, nombre, apellidos, fecha_nac, dni, dirección, teléfono, cod_parque [REF ParqueBomberos], cod_eq [REF Equipo], puesto)

Periodo(fecha_inicio#, fecha_fin#)

Turno(cod_turno#, descripción)

BomberoTrabajaEn(cod_bom# [REF Bombero], cod_turno [REF Turno], fecha_inicio, fecha_fin)  [fecha_inicio,fecha_fin REF Periodo]

