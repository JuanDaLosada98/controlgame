# uml taller 1
## Uml servidor de eclipse
## Interfaz
- main(String[]):void En este metodo se ejecutara toda la aplicacion
- Settings():void
- Setup():void: Aqui se definen todas las variables y cosas que ejecutara la aplicacion
- Draw():void: Aqui se corre toda la parte grafica es mostrada en el lienzo
- MouseClicked():void: Este metodo permetira comenzar con el juego
- KeyPressed():void: Este metodo permite la jugabilidad
## Logica

- Logica(PApplet): Constructor de la clase
- crearPersonajes():void: 
- pintarPersonajesPrincipales():void
- pintarPersonajesSecundarios():void
- pintarEnemigos():void
- primerNivel():void
- segundoNivel():void
- tercerNivel();void
- pintarNiveles():void
- crearVideos():void 
- pintarVideos():void
- eventosDelMouse():void
- eventosDelTeclado():void
- otrosEventos():void
- validarChoqueConBonus():void
- validarAtaqueAEnemigos():void
- validarAtaqueAJugador():void
- validarRecogidaDeObjetos
- pintar():void

## Personaje
- Personajes(PApplet, int,int,PImage[]):
- run():v oid
- getPosX():void
- getPosY():void
- animar():void
- pintar():void
- movimiento():void

## PersonajePrincipal
- PersonajePrincipal(PApplet, int,int,PImage[],int,int):
- movimientosEspeciales():void
- añadirObjeto(Objeto):void
- bajarVida(int):void
- subirVida(int):void
- sumarMonedas():void
- pintarObjetoDePersonaje():void
- ataque():void
- animacion(int):void
## Liszard
- liszard(PApplet, int,int,PImage[],int,int):
- pintar():void
## LilG
- lilG(PApplet, int,int,PImage[],int,int):
- pintar():void 
## PersonajeEnemigo
- PersonajeEnemigo(PApplet, int,int,PImage[]):
- movimientosEspeciales():void
- bajarVida():void
- ataque():void
- animacion(int):void
- movimientosAutomaticos():void 
## Rebrad
- rebrad(PApplet, int,int,PImage[]):
- pintar():void## Radking
## Nivel
- Niveles(PApplet, int, int, Movie,PImage[]):
- crearVideos():void
- pintarVideos():void
- validacionMovimiento():void
- run():void
- movimientoDeMapa():void
- validarEtapa1():boolean
- validarEtapa2():boolean
- pintar():void

## Nivel1
- Nivel1(PApplet,x,y,Movie,PImage[]):

## Nivel2
- Nivel2(PApplet,x,y,Movie,PImage[]): 
## Nivel 3
- Nivel(PApplet,x,y,Movie,PImage[]): 
## Objeto
- Objeto(PApplet,int,int,PImage[]):
- getPosX():int
- getPosY():int
- animar():void
- pintar():void
## Objeto1
- Objeto(PApplet,int,int,PImage[]):
- pintar():void
## Objeto2
- Objeto(PApplet,int,int,PImage[]):
- pintar():void
## Objeto3
- Objeto(PApplet,int,int,PImage[]):
- pintar():void
## Servidor
- run():void: Este es hilo por el cual se establece conexion con los clientes
- enviar():void: Envia los datos obtenidos al servidor
- Receptor
- Receptor(Socket):void:
- run():void: Es el hilo por el cual se reciben los mensajes de los clientes

# Uml Android

### Main
+ **onCreate (Bundle):void:** Con este metodo se inicia la aplicacion
+ **Botones():void:** Con este metodo se obtiene las diferentes acciones de los personajes

### Cliente
+ **Cliente(PApplet, int, int) : void:** Construcctor del cliente
+ **run( ):** Recibe los datos enviados por parte del servidor
+ **enviar():void** Envia los datos obtenidos de las acciones en los botones al servidor 

### Receptor

+ **Receptor(Socket):void:** Constructor del receptor
+ **run():** es el hilo que recibe datos enviados desde el servidor
+ **enviar():void:** Envia los datos obtenidos por las acciones de los botones al servidor.


