Reto: ### Static ain't always noise

Descripcion: Can you look at the data in this binary: [static](https://mercury.picoctf.net/static/ff4e569d6b49b92d090796d4631a2577/static)? This [BASH script](https://mercury.picoctf.net/static/ff4e569d6b49b92d090796d4631a2577/ltdis.sh) might help!

Solucion:
Despues de descargar ambos archivos en kali, y hacer un cat en el script de BASH, le di permisos de ejecucion al script... ya que lo que hace es sacar el codigo y las cadenas de texto encontradas en el static...
```

chmod +x ltdis.sh

./ltdis.sh static

Y luego me dice que las cadenas de texto encontradas estan en xxxx archivo, asi que le di un cat con un grep directamente...
```

```
cat static.ltdis.strings.txt | grep "pico"
1020 picoCTF{d15a5m_t34s3r_ccb2b43e}
```