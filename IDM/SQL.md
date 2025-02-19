## Sintaxis
Una base de datos relacional es un conjunto de tables con filas y columnas, que se relacionan entre ellas mediante los datos.
Para crear una tabla de una base de datos:
```sql
CREATE TABLE Users(
name VARCHAR(128)
email VARCHAR(128)
)
```
Para seleccionar datos de una base de datos:
```sql
SELECT column1,column2,... 
FROM table_name
```
Para seleccionar todas las columnas:
```sql
SELECT * 
FROM table_name
```
Para seleccionar los valores distintos de una columna:
```sql
SELECT DISTINCT column1,column2,...
FROM table_name
```
Si queremos retornar el numero de valores distintos:
```sql
SELECT COUNT(DISTINCT column) 
FROM table_name
```
Filtrar datos:
```sql
SELECT column1,column2,... FROM table_name
WHERE condition
```
Operadores:
	= : igual
	>: mayor que
	<: menor que
	>=: mayor o igual
	<=: menor o igual
	<>: no es igual
	BETWEEN : entre un rango
	LIKE: Busca un patrón
	IN: Especifica varios valores
