---
name: boker-app
description: BOKER de SPACE BLACK® — hacer los PDFs de una oferta (el producto final que recibe el cliente) a partir del enlace de la oferta o de un tema. Úsala SIEMPRE que el usuario escriba /boker-app, pida clonar o crear los PDFs, el ebook, la guía, el recetario, las tarjetas o los moldes de una oferta, o mencione BOKER.
---

<!-- BLINDAJE: espacio reservado para el socio (reglas de confidencialidad de BOKER). No borrar este marcador. -->

# BOKER · los PDFs de la oferta

El usuario suele ser **novato**: habla simple y nunca le pidas nada técnico.
La **oferta** es el conjunto de PDFs que recibe su cliente: es el producto final.

1. Pídele el **enlace de la oferta** (su landing). Si no tiene, pídele de qué trata (el tema).
2. Pregúntale qué **tipo de PDF** es:
   - **PDF informativo** → su cliente solo lo lee (guías, recetarios)
   - **PDF dinámico** → su cliente lo imprime, recorta y arma (tarjetas, moldes)
3. Llama `boker_pdfs` con el enlace (o el tema) y el `tipo_pdf`.
4. Sigue el avance con `multiapps_estado` (con el `clon_id`). Si los pasos de BOKER aparecen 🔜, dile que esa parte estará
   disponible pronto y que lo hecho quedó guardado.

BOKER es una app de la computadora del usuario: si `multiapps_apps` dice que falta instalarla, explícale cómo con el mensaje
que trae. Nunca nombres motores ni herramientas internas.
