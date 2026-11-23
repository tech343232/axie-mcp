---
name: axie
description: Método de trabajo de AXIE para encontrar ofertas que funcionan y keywords nuevas en la Biblioteca de Anuncios de Meta, usando las herramientas axie_* (extensión AXIE de Chrome). Úsala cuando el usuario pida buscar ofertas, páginas de venta, TSL, landings, anunciantes, nichos o palabras clave de anuncios en algún país, o mencione AXIE, Loot o Sweep.
---

# AXIE — cómo trabajar

AXIE es la extensión de Chrome del usuario. Las herramientas `axie_*` le ordenan abrir la
Biblioteca de Anuncios de Meta y recolectar datos. El usuario suele ser **novato**: habla simple,
sin tecnicismos, y nunca le pidas que configure nada técnico.

## 1. Antes de lanzar
- Llama `axie_estado`. Si no está conectada, explícale en una línea: abrir Google Chrome con AXIE
  activada y esperar unos segundos; si sigue igual, cerrar Claude por completo y abrirlo de nuevo.
- **Traduce la búsqueda al idioma del país**: Brasil → portugués ("emagrecer"), EE. UU. → inglés
  ("weight loss"), México/Colombia/España → español. País = código de 2 letras (BR, US, MX, CO, ES, AR).
- Si el usuario no dice país, pregúntalo una sola vez (o usa ALL si dice "todos").

## 2. Qué herramienta usar
| El usuario quiere… | Herramienta | Límite sugerido |
|---|---|---|
| ofertas, páginas de venta, TSL, landings, "qué está funcionando" | `axie_loot` | 100 |
| keywords, ideas, entender un nicho | `axie_sweep` | 150 |
| "todo" / no sabe qué buscar | `axie_sweep` → elige la mejor keyword → `axie_loot` | — |

Para una primera prueba rápida usa límite 30.

## 3. Mientras corre
Los trabajos tardan minutos. Si la respuesta dice `corriendo`, cuéntale el avance en una línea
("AXIE va por 40 links…") y vuelve a llamar `axie_resultado` con el mismo `trabajo_id`.
No lances otro trabajo mientras uno está activo.

## 4. Cómo entregar resultados

**Loot (páginas de venta)**
1. Top anunciantes: los que tienen MÁS links/anuncios primero (más anuncios = oferta que funciona).
2. Agrupado por plataforma (Hotmart, Systeme.io, Lovable, dominios propios…).
3. "Revisa primero estas 3", con el link completo y una razón corta.

**Sweep (keywords)**
1. Organiza los copys por NICHO.
2. Por nicho: FRASES CLAVE para buscar en la Biblioteca y PALABRAS CLAVE DE 3 TÉRMINOS.
3. Mantén el idioma original de los anuncios, quita emojis, ignora ruido.
4. Termina recomendando la mejor keyword para correr `axie_loot`.

## 5. Si algo falla
- 0 resultados → sugiere otra palabra en el idioma del país u otro país.
- "Se cerró la ventana" → pídele que no cierre ni minimice la ventana de AXIE mientras trabaja.
- "Ocupado" → espera el trabajo actual (`axie_resultado`) o cancélalo (`axie_cancelar`).
