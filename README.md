Dictionario
 ## tabla Cities
 |campo| tipo| descripcion|
 |-----|-----|------------|
 |+cit_pk|int| primary key.
 |+cit_nam| vachar(47)| nombre de la ciudad.
 |+cit_pco| vachar(5)| código postal.
 |+cit_di2_fk|smaillint| código de provincias.
 ## tabla administrative_division2
 |campo| tipo| descripcion |
 |-----|-----|-------------|
 |+adm_di2_pk|smaillint| código provincias.
 |+adm_di2_nam| vachar(22)| nombre de la provincia.
 |+adm_di2_di1_fk| smaillint| código de comunidades autonomas.
 ## tabla administrative_division_1
 |campo|tipo| descripcion|
 |-----|----|------------|
 |+adm_div1_pk|smaillint|código de la comunidad autonoma.
 |+adm_div1_nam|varchar(27)| nombre de la comunidad autonoma.
 |+adm_div1_cou_fk|char(3)|código de paises.
  ## tabla paises
  |campo|tipo| descripcion|
  |-----|-----|-----------|
  |+cou_iso|char(3)|código de paises.
  |+cou_nam_esp|nvarchar(44)|nombre de país en espanol.
  |+cou_nam_eng|nvarchar(44)|nombre de país en inglés.
  |+cou_nam_fra| nvarchar(42)|nombre de país en francés.
  |+cou_ddi|nvarchar(5)|código internacional de teléfono.

  ## tabla direcciones
  |campo|tipo| descripcion |
  |-----|----|--------------|
  |+dir_pk|int|primary key.
  |+dir_street|char|nombre de la calle.
  |+dir_num|type|numero de la calle.
  |+dir_city|fk| código postal.

  ## tabla del port
  |campo|tipo|descripcion|
  |----|-----|-----------|
  |+por_pk|int|primary key.
  |+por_dir_fk|int|direccion.
  |+por_nam|vachar(150)|nombre del puerto.
  |+por_tel|int|numero de teléfono.
  |+por_email|int|email del puerto.
  |+por_aut_fk|smaillint|código de la autoridad.

  ## tabla de la autoridad
  |campo|tipo|descripcion|
  |-----|----|-----------|
  |+aut_pk|smaillint|primary key.
  |+aut_nam|vachar(150)|nombre de la autoridad.
  |+aut_dir_fk|int|direccion.
  |+aut_tel|int|numero de teléfono.

  ## tabla Rol authority
  |campo|tipo|descripcion|
  |-----|----|-----------|
  |+rol_aut_pk|int|primary key.
  |+rol_aut_rol_fk|int|rol.
  |+rol_aut_aut_fk|int|autoridad.
  |+rol_aut_ini|int|fecha del inicio.
  |+rol_aut_end|int|fecha del fin.

  ## tabla roles
  |campo|tipo| descripcion|
  |-----|------|----------|
  |+rol_pk|int|primary key.
  |+rol_per_fk|int|personas.
  |+rol_res_fk|int|responsabilidad.

  ## tabla rol_port
  |campo|tipo|descripcion|
  |-----|-----|-----------|
  |+rol_por_pk|int|roles.
  |+rol_por_rol_fk|int|roles.
  |+rol_por_por_fk|int| puertos
  |+rol_por_ini|int|fecha del inicio.
  |+rol_por_end|int|fecha de fin.

  ## tabla responsabilidad
  |campo|tipo| descripcion|
  |-----|-----|-----------|
  |+res_pk|int|primary key.
  |+res_nam|vachar(50)|resposnsabilidades

  ## tabla personas
  |campo|tipo| descripcion|
  |-----|-----|-----------|
  |+per_pk|int| primary key.
  |+per_nam|vachar(50)|nompre de la persona
  |+per_ap1|vachar(50)|apellido1
  |+per_ap2|vachar(50)|apellido2

 
