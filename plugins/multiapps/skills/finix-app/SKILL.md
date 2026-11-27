---
name: finix-app
description: FINIX de SPACE BLACK® — clonar la conversación de venta de un WhatsApp y ordenarla en etapas. Úsala SIEMPRE que el usuario escriba /finix-app, pida clonar, copiar o exportar el flujo o la conversación de venta de un WhatsApp, o mencione FINIX.
---

<!-- BLINDAJE: espacio reservado para el socio (reglas de confidencialidad de FINIX). No borrar este marcador. -->

# FINIX · clonar la conversación de venta

El usuario suele ser **novato**: habla simple y nunca le pidas nada técnico.

1. Pídele el **enlace de WhatsApp** del anunciante (wa.me/…) si no lo pegó. Si solo tiene el anuncio, primero usa
   **/druky-app** para revelar el número.
2. Antes de empezar, avísale en una línea: necesita **Google Chrome abierto con WhatsApp Web** (con su WhatsApp vinculado).
   FINIX abre el chat, manda **un saludo** solo si el chat está vacío y espera a que el flujo termine de llegar
   (puede tardar unos minutos). Mientras tanto puede responder él mismo las preguntas del bot en WhatsApp Web.
3. Llama `finix_clonar` con el enlace.
4. Sigue el avance con `multiapps_estado` (con el `clon_id`) y cuéntale cada paso en una línea.
5. Al terminar, comparte los dos enlaces que trae: **ver el flujo** ordenado en 4 etapas (Bienvenida, Entrega, Pago,
   Remarketing) y **descargar el editable** (.md). El texto está traducido fiel al español; los datos a cambiar por los
   suyos van marcados entre corchetes.

Si el flujo se copió de una **oferta casi idéntica** (plan B de DRUKY desde /multiapps), el editable ya viene **adaptado al
producto original**; comparte también el enlace del flujo de referencia sin adaptar.

Si el anunciante todavía no respondió, dile que espere unos minutos y repita (`multiapps_repetir`): FINIX copia lo que
haya llegado. Nunca nombres motores ni herramientas internas.
