# IaaS (Infrastructure as a service)

## Qué es IaaS?

La IaaS o infraestructura como servicio es una de las 3 formas de cloud computing que vimos en el ejercicio anterior la cual ofrece a los usuarios distintas formas de infraestructura para poder soportar las aplicaciones que desarrollen, pueden ser instancias con su respectivo poder de computo, almacenamiento, dispositivos de red tales como firewalls o nat gateways, etc.

## Servicios ofrecidos en la capa IaaS?

Como mencionamos mas arriba, algunos de los servicios que nos ofrece IaaS son servidores y almacenamiento, seguridad o firewalls de red entre otros.

## Comparacion tarifaria y caracteristicas principales de 3 proveedores de servicios

Para este caso vamos a usar a AWS, a IBM cloud y a Alibaba, para estas comparaciones vamos a utilizar las calculadoras que los 3 proveedores ofrecen y calcular los costos de distintos servicios (teniendo en cuenta que Alibaba solo ofrece servidores/instancias).

Comenzamos con una instancia de linux de 8 gb de ram con unos 2 nucleos:

* En AWS, una instancia on demand de 2 nucleos con 8 gb de ram teniendo un uso del 100% nos costaria al rededor de 49 usd mensuales + 2 usd mensuales por 20gb de disco con hasta 5gb de transferencia de datos, en alibaba por un servicio de las mismas caracteristicas estariamos pagando casi 47 dolares mensuales mientraS que en ibm cloud por un servicio de caracteristicas similares nos estarian cobrando 0.27 usd la hora (aprox 194 usd al mes)

* Con respecto al precio de storage (objetos), ibm ofrece en su servicio de smart tiert un precio de 0.0227 USD por GB mientras que AWS ofrece en su servicio de s3 intelligent - tiering un costo de 0.023 usd por gb en los primeros 50tb al mes con un costo que va reduciendo segun va aumentando el uso (0.022 por los siguientes 450tb y asi) en cambio en alibaba por standard storage nos ofrece un costo de 0.0185 usd por cada gb que utilicemos a partir de los primeros 5gb.

* Por ultimo vamos a comparar el precio de una base de datos mysql utizando como base una instancia de 4 nucleos, 16 gb de ram y 20 gb de almacenamiento ssd con opcion de alta disponibilidad, en Alibaba nos encontramos con un precio de 0.58 dolares la hora mientras que con IBM cloud nos encontramos con un precio mucho mas elebado de 1.496 usd la hora y por ultimo AWS con un precio de casi 0.90 usd por hora

En conclusion podemos ver que Alibaba es el servicio mas barato, seguido por AWS y por ultimo IBM que fue el mas caro y en muchos casos por amplia diferencia.

Si tuviese que elegir personalmente un proveedor, elegiria AWS, ya que en cuestiones de precio si bien no es el mas barato no es el mas caro, cuenta con un soporte de muy alto nivel y es muy facil encontrar profesionales que hayan trabajado con el o tengan experiencia con el mismo, asi como tambien una variedad de servicios y funciones que no vamos a encontrar en ningun otro. Alibaba seria una excelente opcion para clientes con operaciones en china que necesiten hostear sus infraestructura ahi, mientras que IBM corre con la ventaja de que compañias de gran calibre usan sus servicios por lo que puede ofrecer contratos muy beneficiosos para que utilicen IBM cloud.
