descripcion:
Help us test the form by submiting the username as `test` and password as `test!`

solucion:
Aqui si ocupamos burpsuite, ya que no tiene cookies ni robots.txt el sitio

cuando tenemos la intercepcion de paquetes activa y vamos poniendo el usuario y la contraseña, analizamos los paquetes y vemos una linea algo asi...
GET /next-page/id=cGljb0NURntwcm94aWVzX2Fs HTTP/1.1
con lo cual ese iD, es algo codificado en base64... pero es la primera parte, (se me paso capturar la segunda parte) pero esta dividida en 2 paquetes como quien dice...

asi que burp ya te da el decodificado de base64 y solo es armar la bandera
picoCTF{proxies_all_the_way_df44c94c}