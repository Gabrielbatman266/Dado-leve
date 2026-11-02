# Dado Leve 🎲

Dados de RPG em 3D com física própria, feitos para rodar liso até em celular fraco.
Sem bibliotecas: o motor 3D (WebGL) e a física cabem num único `docs/index.html`.

## Baixar

- **APK Android:** aba [Releases](../../releases/tag/latest) → `DadoLeve.apk`
  (gerado automaticamente pelo GitHub Actions a cada push).
- **No navegador:** ative o GitHub Pages em *Settings → Pages → Branch `main` / pasta `/docs`*.

## O que tem

- d4, d6, d8, d10, d12, d20 e d% (d100 = dezena + unidade), até 24 dados na mesa
- Física leve: impulsos por vértice, atrito, quique nas bordas, dados batem entre si
- **Toque** na mesa para rolar · **arraste** para arremessar na direção do dedo
- **Segure um dado parado** para rolar só ele de novo
- Dado que para torto tomba suave na face mais próxima (nada de re-arremesso)
- **Chacoalhe o celular** como um copo de dados
- Vantagem / desvantagem (o d20 descartado fica apagado)
- Modificador +/−, combos salvos (Ataque, Bola de Fogo…), segure um combo para apagar
- Dados explosivos: tirou o máximo, rola mais um e soma
- Crítico (20 natural) e falha crítica (1) com efeito, som e vibração
- **6 temas completos** — cada um muda interface, mesa, material, luz, fonte, som, efeitos e frases:
  - **Taverna** — feltro verde, velas, dados de rubi
  - **Cripta** (sombrio) — lajes rachadas, névoa, luz de vela tremulando, dados de ossário · "O ABISMO SORRI" / "CONDENADO"
  - **Noir** (investigativo) — escrivaninha sob a luminária, sombra de persiana, granulado de filme, ficha "Caso nº", marcadores de evidência amarelos · "CASO RESOLVIDO" / "PISTA FALSA"
  - **Cósmico** — nebulosas, dados arcanos com números que brilham, batida de cristal
  - **Neon** — grade cyberpunk, números acesos, som de sintetizador · "HACK PERFEITO" / "CURTO-CIRCUITO"
  - **Pirata** — mapa do tesouro, dados de latão · "TESOURO!" / "MOTIM!"
- 13 materiais e 8 mesas para combinar como quiser
- Histórico com estatísticas (média do d20, críticos, falhas)
- Modo ultra leve; o motor dorme quando nada está se mexendo (economiza bateria)

## Estrutura

```
docs/index.html        o jogo inteiro (HTML + CSS + JS, ~50 KB)
app/                   casca Android (WebView) que carrega docs/ como assets
.github/workflows/     compila o APK e publica na release "latest"
```
