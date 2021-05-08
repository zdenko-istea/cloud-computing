# Cloud Computing

## Qué es Cloud Computing?

Llamamos cloud computing al concepto de poder brindar distintos servicios o soluciones a traves de internet.

## Características generales (capas, tipos de nubes, tarificación,etc)

* Primero y principal cabe destacar que en cloud computing tenemos 2 tipos de nube importantes, las nubes publicas que es un servicio hosteado por distintos proveedores como pueden ser Amazon, Google, Microsoft, IBM, Alibaba, entre otros como tambien tenemos las nubes privadas que es un servicio similar al que nos puede ofrecer algunas de estas empresas con la diferencia de que esta nube las vamos a hostear dentro de nuestro propio datacenter o infraestructura.
Vamos a poner de ejemplo a AWS y Open Stack donde ambos nos pueden ofrecer soluciones de computo como instancias, soluciones de red, storage de bloques o de archivos, etc.

* Hay 3 capas importantes dentro de cloud computing en referencia al tipo de soluciones que nos puede ofrecer, IaaS, PaaS y SaaS.

* Con respecto a como estas distintas soluciones son cobradas al fin del dia la respuesta es que depende del servicio en su gran parte aunque asi tambien del proveedor del mismo, poniendo de ejemplo AWS con su servicio de Instancias EC2, el cobro de las mismas es por hora de utilizacion aunque tienen distintos tipos de descuentos segun el tipo de instancia ya que podemos hacer una reserva de 3 años y asi obtener un gran descuento o por ejemplo usar spot instances que son un tipo de subasta donde nosotros definimos un maximo de dinero a gastar por la misma y mientras que el valor por hora de la misma se encuentre dentro de nuestro limite tendremos acceso a la misma.

## Tipos de servicios ofrecidos

Como mencionamos ya en el punto anterior respecto a las capas, esto tambien nos brinda una diferenciacion dentro de lo que son los servicios ofrecidos ya que usando a AWS como ejemplo (principalmente por ser uno de los mas grandes) nos ofrece infraestructura como servicio en forma de instancias, recursos de red, de almacenamiento, etc como asi tambien plataformas como servicio donde solo tenemos que poner nuestro codigo y AWS se encargara de hacer el deploy, por otro lado tienen servicios SaaS como por ejemplo RDS que es el servicio de bases de datos de AWS donde solo tendremos que configurarlo para utilizarlo pero AWS se encargara de ser quien lo administre a mas bajo nivel dejando que nosotros solo nos tengamos que preocupar por como lo utilizamos. En resumen, algunos de los servicios basicos ofrecidos por estas empresas pueden ser soluciones de procesamiento de datos, almacenamiento, red, bases de datos, etc.

## Ventajas y desventajas

* Una de las ventajas a mi opinion es la mas importante es la facilidad con la que uno puede levantar infraestructura, supongamos el caso de que quiero levantar un server en mi casa no? Tengo que hacer la compra del equipo o los distintos componentes lo cual puede tardar varios dias, ni mencionemos el caso en que algo llegue fallado y tengamos que cambiarlo, hasta el armado, configuracion y demas del equipo, supongamos que pueden pasar al menos 7 dias para que yo pueda levantar un sitio estatico no? Cloud computing viene a cambiar el panorama, es cuestion de abrir una cuenta en AWS, configurar el metodo de pago y empezar a desplegar nuestros programas, sitios o lo que querramos crear, llamese AWS, digital ocean, GCP, Azure, cualquier empresa de cloud computing.

* Por otro lado costos, es mucho mas accesible pagar solo por lo que estamos utilizando que el hardware fisico que generalmente tenemos que comprar de mas en caso de que querramos escalar nuestros servicios.

* La confiabilidad de que si mi internet se cae, se me corta la luz en mi casa o algun otro problema local esto no afecte la disponibilidad de mis servicios en la nube, incluso por ejemplo AWS tiene distintas opciones de alta disponibilidad que nos permiten que se caiga un datacenter entero y nuestro servicio ni se entere ya que esta corriendo en multiples datacenter.

Pero no todo es color de rosas, algunas desventajas son por ejemplo lo facil que es olvidarse un servicio prendido un fin de semana y despertarte un lunes con 200USD de mas que no calculaste en tu presupuesto o la curva de aprendizaje que tiene adentrarse en el mundo del cloudcomputing, pero como vemos no son cosas que con la suficiente dedicacion para aprender a utilizarlo sean un gran problema o algo que nos desmotive a utilizar cloud computing. 