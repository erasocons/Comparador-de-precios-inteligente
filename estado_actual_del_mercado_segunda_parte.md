# Estado actual del mercado (segunda parte)

Este documento complementa el diagnóstico del mercado de compras en línea en Colombia. Mientras la primera parte analizó las limitaciones generales de las plataformas actuales y la oportunidad de integrar un asistente de inteligencia artificial para planear y ejecutar compras, esta segunda parte desglosa en detalle cómo operan los actores reales del ecosistema: por un lado, los comercios según su nivel de digitalización y, por otro, las plataformas externas de *delivery* y comparación de precios, junto con los principales aprendizajes y brechas que hoy condicionan al consumidor.

---

## Parte 1: Los proveedores de productos (Comercios y nivel de digitalización)

La posibilidad de comparar precios y comprar en línea depende directamente de qué tan digitalizado tiene su catálogo cada tipo de comercio en Colombia:

* **Proveedores pequeños (Tiendas de barrio, minimercados locales y fruvers independientes):** No cuentan con páginas web ni catálogos digitales en línea. Sus precios e inventarios son invisibles para los buscadores automatizados, por lo que quedan por fuera de cualquier comparación digital y solo operan mediante venta presencial o domicilios informales por teléfono o WhatsApp.
* **Proveedores medianos y grandes (Cadenas con presencia web y posibilidad de scraping):** Cuentan con tiendas en línea, aplicaciones propias o catálogos públicos donde es técnicamente viable extraer precios (*scraping*) o establecer convenios. En este grupo entran:
  * **Hard discount y supermercados masivos:** Tiendas D1, Ara, Ísimo, Éxito, Carulla, Jumbo, Metro, Olímpica, Súper Inter y Surtimax.
  * **Cadenas regionales clave (especialmente en el Valle del Cauca y suroccidente):** Mercamio, Cañaveral, La Montaña Agromercados y Mercatodo.
  * **Droguerías, hogar y conveniencia:** Farmatodo, Cruz Verde, La Rebaja, Locatel, Dollarcity, Homecenter y Alkosto.

---

## Parte 2: Proveedores externos (Domiciliarios y herramientas de búsqueda multinegocio)

Sobre la oferta de los comercios operan las plataformas tecnológicas y redes logísticas externas, que en Colombia se dividen en tres grupos funcionales:

### Grupo 1: Aplicaciones de delivery y compra directa (Proveedores de domiciliarios + pasarela)
Son plataformas que aportan la flota de repartidores, la logística de última milla y la pasarela de pago integrada para comprar en supermercados y tiendas cercanas, aunque sin comparación automática de listas completas:
* **Rappi:** Permite buscar un producto y ver qué tiendas asociadas alrededor de tu ubicación lo tienen disponible para compra directa, pero no permite ordenar los resultados por precio (ni siquiera dentro de cada comercio), obligando a revisar manualmente.
* **DiDi (DiDi Food / Tiendas):** Permite buscar artículos en tiendas cercanas y, a diferencia de Rappi, sí deja ordenar los productos por precio una vez entras a cada comercio; sin embargo, no compara automáticamente la suma total de varios productos entre distintas tiendas.
* **Uber (sección Súper / Tiendas):** Permite buscar productos en comercios asociados cercanos a tu dirección y hacer la compra directa en la aplicación, funcionando bajo una lógica similar de revisión manual tienda por tienda.
* *(Nota: También existen operadores logísticos puros de última milla como Mensajeros Urbanos o Picap, que proveen únicamente el equipo de domiciliarios para despachos de comercios, sin funcionar como vitrina comparadora para el usuario).*

### Grupo 2: Buscadores por producto individual (Scraping y redirección)
Son herramientas multinegocio que extraen precios en vivo de los catálogos web de los proveedores medianos y grandes, pero no procesan pagos ni tienen domiciliarios. Te muestran el precio por artículo y te envían al sitio oficial del comercio:
* **Pillelo:** Consulta en tiempo real los precios de un artículo específico en unos 22 comercios (como Ara, D1, Olímpica, Éxito, Carulla, Farmatodo y Cruz Verde) y te redirige al enlace de compra de cada tienda. Permite alertas de precio, aunque su lista gratuita es limitada (hasta 10 productos).
* **PillePrecios:** Funciona como buscador paralelo de artículos sueltos en cadenas con tienda en línea (Éxito, Jumbo, Olímpica, Alkosto, etc.), enviándote a la web del supermercado sin optimizar el carrito completo ni sumar domicilios.
* **Tiendeo / Ofertia:** Enfocados en geolocalización de folletos y ofertas vigentes. Te muestran qué sucursal cercana tiene un producto en promoción y su ubicación en el mapa, pero la compra es presencial o externa.

### Grupo 3: Optimizadores de canasta completa (Cálculo de lista total)
Son herramientas diseñadas para ingresar toda tu lista de mercado y calcular en qué supermercado te sale más barata la suma total de esos productos, aunque tampoco tienen pasarela de pago ni calculan tarifas de domicilio:
* **Price It:** Permite armar la lista completa de mercado (o escanear códigos de barras en tienda) y calcula cuánto cuesta el carrito entero en cadenas como Éxito, Carulla, D1, Ara, Ísimo, Jumbo y Olímpica, indicándote qué supermercado (o combinación de supermercados) te genera el mayor ahorro.
* **AhorryGo:** Usa tu ubicación para identificar las tiendas que realmente tienes cerca y compara el costo total de tu lista entre unas 30 cadenas nacionales y regionales (incluyendo Mercamio, Súper Inter, Cañaveral, D1, Ara y Éxito), nutriéndose tanto de catálogos públicos como de facturas subidas por usuarios.
* **Los Precios:** Permite ingresar tu lista o recetas y usa un motor de planeación que sugiere sustituciones de marcas y te indica en qué tiendas comprar para minimizar el gasto total de la canasta.

---

## Resumen del estado actual: Comprar barato y rápido en Colombia

El panorama actual evidencia una brecha de mercado (*trade-off* entre tiempo y dinero) para el consumidor colombiano:

| Grupo de Apps | Ejemplo | ¿Optimiza canasta completa? | ¿Suma costo de domicilio / distancia? | ¿Compra directa en la app? | Resultado para el usuario |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **1. *Delivery* y compra directa** | Rappi, DiDi, Uber | No (comparación manual tienda por tienda) | Sí (calcula envío y distancia al pagar) | Sí | Ahorra tiempo, pero pagas sobrecostos por falta de transparencia y precios inflados. |
| **2. Buscadores con redirección** | Pillelo, PillePrecios, Tiendeo / Ofertia | No (solo compara producto por producto) | No | No (envía a web externa o tienda física) | Útil para compras puntuales, lento para hacer un mercado completo. |
| **3. Optimizadores de lista** | Price It, AhorryGo, Los Precios | Sí (calcula la suma total más barata) | No | No (debes ir a la tienda o pedir aparte) | Ahorra dinero (promedio 20%–22%), pero exige invertir tiempo desplazándote o pidiendo en cada app. |

---

## Conclusiones del panorama

1. **Ausencia de una solución integral ("La ecuación incompleta"):** Hoy en Colombia no existe una plataforma que resuelva la fórmula completa (Costo total de la canasta + Tarifa de domicilio + Distancia = Compra en un clic). Quien prioriza gastar el menor tiempo posible (Grupo 1) sacrifica dinero porque Rappi oculta el ordenamiento por precio y DiDi exige revisar tienda por tienda manualmente; quien prioriza comprar lo más barato (Grupo 3) descubre fácilmente dónde ahorrar hasta un 20%, pero debe invertir tiempo desplazándose físicamente o comprando en los canales propios de cada cadena.
2. **Desconexión entre la capa de datos y la capa logística:** Los comparadores que tienen la inteligencia de precios (Grupos 2 y 3) carecen de flotas de domiciliarios y pasarelas de pago transaccionales, mientras que las empresas con capacidad logística (Grupo 1 y operadores de última milla) no tienen incentivos comerciales para mostrar qué tienda es más barata, ya que su modelo de negocio depende de comisiones por venta y acuerdos preferenciales con comercios específicos.
3. **El punto ciego del comercio de proximidad (barrio):** Incluso si se lograra integrar hoy a todos los actores digitales, el sistema dejaría por fuera a las tiendas de barrio y fruvers pequeños (Parte 1), que en muchos casos ofrecen los precios más bajos en productos frescos y de consumo diario a menor distancia, pero cuya falta de digitalización impide incluirlos en cualquier motor automatizado de ahorro y tiempo.