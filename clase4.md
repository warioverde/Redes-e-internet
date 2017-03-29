# capa 3 
- protocolo ip (protocolo mas usado aqui)
la capa 3 se encarga del enrutamiento.
manda paquetes pero en "best efford". las cabeceras ip contienen las direcciones de las maquinas de origen y destino.
estas son usadas por los routers. la version actual es la ipv4 . que usa direcciones de 32 bits.
sus desventajas son que las ip son escasas y se desperdician.
- hay 3 tipos de redes
  -clase A -->solo son 127 (redes)--->asigna el primer octeto
  -clase B -->solo son 16384(redes)--> asigna el primer y segundo octeto
  -clace C--->solo son 2 millones(redes)--->asigna los 3 primeros octetos-->solo son 254 ips
  la direccion de RED son los octetos de cada red y el resto se llena con ceros
  ej 120.0.0.0 -->red de tipo A
  
  para solucionar la escases de ip se crearon las direcciones privadas ---> no son accesibles desde el exterior.
  
  # NAT 
  el nat es el puente entre el las ips privadas y internet es el NAT.
  - los routers tienen ip's publicas en general.
  el router toma un paquete con ip privada y la cambia can su ip publica.
  el router tiene los registros de ip de origen y destino en una TABLA NAT
  si sale el 0.0.0.0 es cuando el pc esta arrancando, es la ruta por default.
  
   - direcciones especiales
    -120.0.0.0 es la direccion de la red --> primera ip
    -120.255.255.255 direccion de difucion hace como un hub--> ultima ip
    -127.0.0.1 es la direccion de la maquina (llopback)
    
   # direccion de ip fija
   - las ip fijas estan hechas para los servicios de internet
   - yo tengo ip dinamica y lo hace un protocolo llamado DHCP
   
  #hoy
   - en el dia de hoy las ip son classless "sin clase"
    para saber que parte de la ip es red y que parte es host. se inventaron las subredes , las cuales tienen mascaras de subred
    -la mascara
    la mascara tiene que ver con las divicion , se ocupa 2^x >= divisiones.
