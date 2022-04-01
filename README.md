# Comando Delete Oracle
#### Este comando nos permite eliminar una fila de tabla de la cual vamos a especificar por algun campo determinado.

```sql
 create table agenda(
  apellido varchar2(30),
  nombre varchar2(20),
  domicilio varchar2(30),
  telefono varchar2(11)
 );
 ```

```sql
 insert into agenda(apellido,nombre,domicilio,telefono) values 
   ('Alvarez','Alberto','Colon 123','4234567');
 insert into agenda(apellido,nombre,domicilio,telefono) values 
   ('Juarez','Juan','Avellaneda 135','4458787');
 insert into agenda(apellido,nombre,domicilio,telefono) values 
   ('Lopez','Maria','Urquiza 333','4545454');
 insert into agenda(apellido,nombre,domicilio,telefono) values 
   ('Lopez','Jose','Urquiza 333','4545454');
 insert into agenda(apellido,nombre,domicilio,telefono) values 
   ('Salas','Susana','Gral. Paz 1234','4123456');
 ```
 ```sql
 select * from agenda;
 ```
 
 | apellido            | nombre               |   domicilio   |   telefono   |
 | --------------------| :----------------:| --------:| ----------:|
 | Alvarez            | Alberto               |   Colon 123   |   4234567   |
 | Juarez            | Juan               |   Avellaneda 135   |   4458787   |
 | Lopez            | Maria               |   Urquiza   |   4545454   |
 | Lopez            | Jose               |   Urquiza   |   4545454   |
 | Salas            | Susana               |   gral. Paz 1234   |   4123456   |
 
 > Comando Delete, Siempre tener en cuenta que se debe usar la clausula **where**.
 ```sql
 delete from agenta where nombre = 'Juan'
 ```
 ```sql
 select * from agenta;
 ```
  | apellido            | nombre               |   domicilio   |   telefono   |
 | --------------------| :----------------:| --------:| ----------:|
 | Alvarez            | Alberto               |   Colon 123   |   4234567   |
 | Lopez            | Maria               |   Urquiza   |   4545454   |
 | Lopez            | Jose               |   Urquiza   |   4545454   |
 | Salas            | Susana               |   gral. Paz 1234   |   4123456   |
 
 > Delete toda la tabla, tener cuidado siempre con esto ya que podemos arruinar toda la bd
  ```sql
 delete from agenta'
 ```
 ```sql
 select * from agenta;
 ```
 | apellido            | nombre               |   domicilio   |   telefono   |
 | --------------------| :----------------:| --------:| ----------:|
 
