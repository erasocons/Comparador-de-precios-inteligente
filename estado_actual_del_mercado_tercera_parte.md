# Estado actual del mercado (tercera parte): Madurez tecnológica y brecha de la IA conversacional

Mientras la primera parte abordó las limitaciones generales del mercado y la segunda clasificó a los actores locales según su digitalización y logística, esta tercera parte evalúa el nivel tecnológico de los comparadores en Colombia frente al estándar global de asistentes de inteligencia artificial. Actualmente, ninguna plataforma colombiana opera como un agente conversacional puro que entreviste al usuario antes de armar la ruta óptima de compra; en su lugar, el ecosistema local se reparte entre motores de búsqueda tradicionales, herramientas de *scraping* y optimizadores matemáticos de listas manuales.

---

## 1. Ranking tecnológico de comparadores en Colombia

Ordenados de mayor a menor sofisticación según su arquitectura de datos, automatización e integración de inteligencia artificial:

| Plataforma | Nivel Tecnológico | Arquitectura y Cobertura | Herramientas Avanzadas | Interfaz Chat IA | Optimiza División de Compra | Escáner Código de Barras |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **PillePrecios** | Alto (IA Generativa + Scraping Paralelo) | Búsquedas paralelas instantáneas en 11 comercios (Alkosto, Falabella, Éxito, Amazon, D1, Homecenter). | Único en Colombia con análisis de IA en interfaz para evaluar hasta 5 productos (pros, contras, confianza y tendencia de precios). | No | No | No |
| **Oferty** | Alto (Ciencia de Datos y Scraping Masivo) | Infraestructura de *ScraperLabs* con extracción masiva en tiempo real para tecnología y supermercados. | Limpieza automática de variantes (modelos, capacidades, referencias) mediante algoritmos para evitar mezclar artículos distintos. | No | Parcial (datos) | No |
| **Price It** | Medio-Alto (Optimización Matemática) | App móvil nativa enfocada en supermercados (Éxito, D1, Ara, Ísimo, Carulla, Olímpica, Jumbo). | Calcula combinaciones de compra por tienda o división de canasta, incluye comparador de marcas equivalentes y mapa cercano. | No | Sí | Sí |
| **AhorryGo** | Medio (Geolocalización Multicanal) | Rastreo web en 30 cadenas físicas y *hard discounters* (incluyendo D1, Ara y Dollarcity). | Cruce de inventario por barrio sin registro, lectura de QR de facturas electrónicas (DIAN) y modo "Mercar en vivo". | No | Parcial | Sí (QR facturas) |
| **Pillelo** | Medio-Bajo (Monitoreo Asíncrono) | Rastreador web conectado a 22 tiendas nacionales e internacionales. | Tareas programadas (*cron jobs*) para seguimiento histórico de precios, listas de deseos y alertas por correo. | No | No | No |
| **SuperPrecios** | Básico (Consulta Directa) | App ligera en 7 cadenas principales con cobertura en 26 ciudades (incluyendo Cali y Palmira). | Consulta rápida en pasillo con actualización de precios cada 6 horas, sin IA ni optimización de listas. | No | No | Sí |

---

## 2. Clasificación por niveles de madurez tecnológica (Colombia vs. Estándar Global)

| Nivel | Tipo de Plataforma | Obtención de Datos | Funcionamiento y Capacidades | Ejemplo Colombia | Ejemplo Global |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Nivel 1: Básico** | Búsqueda aislada en tienda individual | Servidores y bases de datos propias de cada cadena. | Muestra únicamente el inventario de un comercio; obliga a abrir múltiples pestañas y calcular manualmente. | App Éxito, D1, Alkosto | Walmart App |
| **Nivel 2: Agregador** | Comparación manual multi-tienda | Convenios comerciales/APIs (delivery) o *web scraping* básico y *feeds* públicos. | Agrupa comercios cercanos, pero requiere buscar y comparar producto por producto sin optimizar el carrito total. | Rappi, Pillelo, SuperPrecios | Google Shopping clásico |
| **Nivel 3: Optimizador** | Cálculo matemático de canasta completa | *Web scraping* diario sin convenios comerciales + *crowdsourcing* (datos y facturas de usuarios). | Calcula combinaciones para ahorrar hasta un 20% comprando en una tienda o dividiendo la lista entre varias. | Price It, AhorryGo | Basket, Flipp |
| **Nivel 4: Agente IA** | Asistente conversacional y compra autónoma | Modelos LLM + *Shopping Graph* en vivo e integración con pasarelas de pago. | Entrevista al usuario sobre presupuesto y necesidades, arma recetas/listas y ejecuta compras automáticas (*Agentic Checkout*). | *PillePrecios* (solo resume candidatos ya elegidos) | Google AI Mode, Perplexity Shopping, Alexa for Shopping |

### Capacidades clave del Nivel 4 (Estándar Global aún ausente en Colombia)
* **Consultoría conversacional previa:** Herramientas como *Google AI Mode*, *Perplexity Shopping* y *Alexa for Shopping* funcionan mediante entrevistas ("Tengo $1.500.000 para un monitor ergonómico" o "Arma desayunos saludables para 5 días con este presupuesto"), filtrando especificaciones técnicas o recetas con inventario real antes de mostrar precios.
* **Compra agéntica autónoma (*Agentic Checkout*):** Plataformas como *Google Universal Cart* monitorean productos en segundo plano con condiciones exactas (talla, color, precio máximo) y ejecutan el pago automáticamente en cuanto el precio cae dentro del límite fijado.
* **Visión artificial y mercados secundarios:** Aplicaciones como *Phia* o *Buyhatke* analizan fotos o enlaces para comparar artículos nuevos y de segunda mano, aplicar cupones automáticamente y detectar descuentos falsos mediante historiales de precios.

---

## 3. El vacío actual: Los dos filtros desconectados

En Colombia existe una brecha operativa porque las herramientas actuales operan "al revés" o de forma aislada. Mientras *Price It* y *AhorryGo* resuelven el cálculo matemático de una lista ya creada, *PillePrecios* exige que el usuario investigue y seleccione primero los productos candidatos para luego generar un resumen con IA. Para lograr una experiencia integral se requiere conectar dos filtros hoy separados:

1. **Filtro 1 — Cognitivo o de Intención (Inteligencia Artificial):** Traduce una necesidad abierta en una lista técnica de compras. Entrevista al usuario (presupuesto, cantidad de personas, restricciones o uso) y calcula porciones exactas o especificaciones técnicas.
2. **Filtro 2 — Logístico y Económico (Geolocalización + Optimización):** Cruza esa lista técnica con los inventarios reales cercanos a la dirección del usuario, sustituye marcas por equivalentes más económicos y calcula la combinación óptima de tiendas y tiempos de entrega.

---

## 4. Caso práctico: Comprar ingredientes para una cazuela de mariscos (10 personas)

| Aspecto | Escenario A: Compra Tradicional (Sin filtros) | Escenario B: Con 1 Filtro (Solo IA o Solo Optimizador) | Escenario C: Con 2 Filtros Integrados (Agente Integral) |
| :--- | :--- | :--- | :--- |
| **Flujo de trabajo** | Buscar receta para 4 personas, multiplicar por 2.5 a mano y buscar ingrediente por ingrediente en apps de supermercados y Rappi. | **Solo Filtro 1 (ChatGPT/Gemini):** Entrega cantidades exactas, pero obliga a buscar precios manualmente.<br>**Solo Filtro 2 (Price It/AhorryGo):** Encuentra dónde es más barato, pero exige llevar la lista ya calculada. | Una sola instrucción ("Cazuela para 10 personas mañana, presupuesto medio, 2 alérgicos al maní"). La IA hace 2 preguntas rápidas, cruza inventarios locales, sustituye marcas costosas y arma el carrito listo para pagar. |
| **Tiempo invertido** | 45 – 60 minutos | 20 – 30 minutos | **3 – 5 minutos (Ahorro del ~90%)** |
| **Precisión** | Baja (alto riesgo de error en proporciones y olvidos) | Media (depende de qué filtro se utilice) | **Alta (porciones y restricciones calibradas)** |
| **Ahorro económico** | Nulo (compra en la primera tienda disponible) | Medio (optimiza receta o precio por separado) | **Máximo (optimiza ambos factores en conjunto)** |
| **Carga mental** | Alta (toda la logística recae en el usuario) | Media (requiere pasos manuales intermedios) | **Mínima (el usuario solo supervisa y aprueba)** |