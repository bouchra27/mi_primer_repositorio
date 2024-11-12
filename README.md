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
 
