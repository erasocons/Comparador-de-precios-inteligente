# Comprar sin Vueltas (Prototipo: Cero Scroll)

**Comprar sin Vueltas** es una interfaz intermedia y motor de comparación diseñado para eliminar la fricción y el *scroll* innecesario al comprar productos de consumo masivo en plataformas de *delivery* (iniciando con Rappi en Colombia).

## 🎯 ¿Qué busca resolver este proyecto?

Actualmente, el ecosistema de compras en línea se encuentra fragmentado: las aplicaciones de *delivery* ofrecen conveniencia y pago integrado, pero carecen de herramientas eficientes para comparar precios reales entre múltiples comercios o incluso dentro de una misma tienda[cite: 5]. El usuario se ve obligado a navegar carruseles horizontales infinitos y calcular manualmente qué opción conviene más[cite: 5].

El objetivo de este prototipo es **devolverle el control al comprador** mediante un flujo automatizado que permite:

1. **Consultar sin fricción:** Obtener los catálogos reales de tiendas disponibles según la ubicación/dirección exacta del usuario, evitando la navegación manual.
2. **Normalizar la información:** Estandarizar presentaciones y cantidades de texto libre (ej. precio por unidad, gramo o mililitro) para comparar productos equivalentes de forma justa.
3. **Ordenar por valor real:** Aplicar criterios de ordenamiento que no existen nativamente en la plataforma:
   * Menor precio total global.
   * El producto más económico dentro de cada tienda.
   * Relación calidad-precio según las preferencias del usuario.
4. **Decidir rápido y comprar directo:** Presentar los resultados en una vista limpia e interactiva donde el usuario compare al instante y salte directamente al enlace del producto para finalizar su compra.

## 🏗️ Arquitectura del Prototipo (5 Etapas)

1. **Captura de contexto:** Ingreso de producto y ubicación/dirección exacta.
2. **Adquisición de datos crudos:** Extracción automatizada mediante Python de las respuestas reales de catálogo.
3. **Limpieza y normalización:** Estructuración uniforme de tiendas, precios, unidades y enlaces.
4. **Motor de ordenamiento:** Aplicación de filtros y algoritmos de comparación por precio y valor.
5. **Interfaz intermedia:** Visualización clara y accionable para el usuario final.
