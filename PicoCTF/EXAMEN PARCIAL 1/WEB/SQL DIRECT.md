descripcion:
Connect to this PostgreSQL server and find the flag!

solucion:
postgres usa una sintaxis de comandos diferentes... pero es algo complicada, 
despues de conectarnos a la base de datos use \l que es para listar las tablas

despues \dt para los comandos de la tabla

select * from flags;

y tendremos la bandera
picoCTF{L3arN_S0m3_5qL_t0d4Y_31fd14c0}