# Dicionário de Variáveis — Tábuas de Vida Abreviadas (2019–2024)

Este documento descreve todas as colunas presentes nos arquivos em formato CSV disponibilizados nas pastas `data/tabuas_fator_f/` e `data/tabuas_ajustadas_mii/`.

---

## 1. Identificação e Estrutura Demográfica
- `ano`: Ano de referência das estimativas (2019 a 2024)
- `regiao`: Âmbito geográfico (`Brasil`, `Norte`, `Nordeste`, `Sudeste`, `Sul`, `Centro-Oeste`)
- `sexo`: Categoria de sexo (`Feminino`, `Masculino`)
- `raca_nome` / `raca_cor`: Categoria de cor ou raça (`População geral`, `Branca`, `Preta`, `Parda`, `Amarela`, `Indígena`)
- `idade` / `age_x`: Idade exata no início do grupo etário (0, 1, 5, 10, ..., 80 anos)
- `fx_etaria` / `faixa_etaria`: Rótulo do intervalo de idade (`0`, `1-4`, `5-9`, ..., `80+`)

---

## 2. Denominadores e Taxas
- `populacao` / `populacao_corrigida`: População de exposição (sem ajuste IBGE vs. MII)
- `obitos`: Número de óbitos registrados/corrigidos no SIM
- `Fator_F`: Fator de correção de mortalidade por raça (método Fator F)
- `nMx` / `nMx_observada` / `nMx_original`: Taxa central bruta de mortalidade
- `nMx_tabua` / `nMx_final`: Taxa central efetivamente utilizada na construção da tábua

---

## 3. Funções da Tábua de Vida
- `ni`: Amplitude do intervalo etário em anos (1, 4 ou 5 anos; 999 no grupo aberto)
- `ai`: Anos médios vividos no intervalo pelos falecidos (a0, a1, ax)
- `qi`: Probabilidade de morte no grupo etário (qx)
- `li`: Sobreviventes à idade exata x (radix = 100.000)
- `di`: Óbitos teóricos ocorridos no grupo etário
- `Li`: Anos-pessoa vividos pela coorte no intervalo
- `Ti`: Total de anos-pessoa vividos acumulados acima da idade x
- `ei` / `e0` / `ex`: Expectativa de vida à idade x (e0 = expectativa de vida ao nascer)
