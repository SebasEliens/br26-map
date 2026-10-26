# 🇧🇷 br26-map

**[→ Ver mapa](https://sebaseliens.github.io/br26-map/)**

Visualização da variação relativa de votos entre o 1° e o 2° turno das eleições presidenciais brasileiras de 2026.

**Métrica por estado/município:**

```
(Lula 2T − Lula 1T) − (Flávio 2T − Flávio 1T)
```

normalizada pelo total de votos válidos. Vermelho = Lula ganhou mais votos relativos; azul = Flávio ganhou mais.

## Dados

- Votos por estado: [TSE API de resultados](https://resultados.tse.jus.br) (ambos os turnos disponíveis)
- Votos por município: [TSE dados abertos](https://dadosabertos.tse.jus.br) — `votaçao_secao_2026_BR.zip`
- Geometrias: [tbrugz/geodata-br](https://github.com/tbrugz/geodata-br)

## Execução local

```bash
uv sync
uv run jupyter lab election_map.ipynb
```
