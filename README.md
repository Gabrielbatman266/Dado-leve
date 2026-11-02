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
- **Toque num dado parado** para rolar só ele de novo
- **Chacoalhe o celular** como um copo de dados
- Vantagem / desvantagem (o d20 descartado fica apagado)
- Modificador +/−, combos salvos (Ataque, Bola de Fogo…), segure um combo para apagar
- Dados explosivos: tirou o máximo, rola mais um e soma
- Crítico (20 natural) e falha crítica (1) com efeito, som e vibração
- 9 materiais (Rubi, Safira, Esmeralda, Osso, Obsidiana, Gelo translúcido, Lava, Arcano, Sortido)
- 3 mesas (Feltro, Taverna, Abismo) — o som da batida muda com a mesa
- Histórico com estatísticas (média do d20, críticos, falhas)
- Modo ultra leve; o motor dorme quando nada está se mexendo (economiza bateria)

## Estrutura

```
docs/index.html        o jogo inteiro (HTML + CSS + JS, ~50 KB)
app/                   casca Android (WebView) que carrega docs/ como assets
.github/workflows/     compila o APK e publica na release "latest"
```
