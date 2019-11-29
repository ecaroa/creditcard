# creditcard
# Challenge de tarjeta de crédito

Se ha solicitado el diseño de un sistema para procesar operaciones con tarjetas de crédito para una organización. 
Dicho sistema debe disponer de un módulo que permita con las siguientes consideraciones desarrollar un aplicativo:
- Una tarjeta se identifica de acuerdo a la marca, número de tarjeta, cardholder(nombre y apellido) y fecha de vencimiento
- Una operación es válida en el sistema si la persona que opera en el mismo consume menos de 1000 pesos
- Una tarjeta es válida para operar si su fecha de vencimiento es mayor al presente día
- Hoy en día, existen tres marcas de tarjeta de crédito, a saber: “VISA”, “NARA”, “AMEX” y es posible que en los siguientes meses existan nuevas marcas. Cada marca tiene un modo de calcular una tasa por el servicio que es desde 0.3% hasta 5%, a saber:
  -   Tasa VISA = año / mes
  -   Tasa NARA    = dia del mes *0.5
  -   Tasa AMEX  = mes*0.1
  
  
  Construir un desarrollo en java:
  
## Parte 1 Crear una clase ejecutable con 3 objetos que haga lo siguiente:
-   Invocar un método que devuelva toda la información de una tarjeta
-   Informar si una operación es valida
-   Informar si una tarjeta es válida para operar
-   Identificar si una tarjeta es distinta a otra
-   Obtener por medio de un método la tasa de una operación informando marca e importe

## Parte 2
  - Se identificó que el proceso que se ejecuta para cobrar consta de 4 acciones, a saber:
  cobrar {
    - imprimirFactura():                    // *imprimir factura en controladora fiscal* 
    - enviarInfoTC();                          // *enviar info de tarjeta de crédito*
    - informarPago();                        // *Informar pago a comercial*
    - actualizarSaldo(cliente);          // *actualizar saldo del cliente*
    
  }
  
-  Adaptar los métodos para contemplar los siguientes casos de error:
    -  la impresora devuelve error (por ejemplo, por trabarse el papel)
    -  el host de la tarjeta de crédito está caído
    -  el sistema contable no responde y/o no atiende los pedidos
    -  la base de datos no permite escribir el nuevo saldo del cliente

## Parte 3
  - Implementar un servicio REST en formato JSON de consulta de tasa de una operación informando marca e importe
  - Compartir código en GIT
  - Hostear solución API REST en algún cloud computing libre e indicar URL
  Contraer


