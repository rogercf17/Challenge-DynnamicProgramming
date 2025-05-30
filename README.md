# Sistema de Gerenciamento de Exames Médicos - Dimensionamento de Amostras

## Identificação do Grupo
- **Turma:** 2ESPW
- **Integrantes:**
  - Fernanda Rocha Menon - RM: 554673
  - Gabriel Machado Lacerda - RM: 556714
  - Luiza Macena Dantas - RM: 556237
  - Roger Cardoso Ferreira - RM: 557230

---

## Descrição da Solução
Este projeto simula um **sistema automatizado para gerenciamento e análise de exames médicos**, focando no **dimensionamento de amostras de patologia**, conforme apresentado no **Desafio 2** do case DASA e na disciplina de Dynamic Programming.

Utilizamos estrutura de dados com dicionários aninhados e listas, funções especializadas para análise, validação, exportação de relatórios e visualização gráfica. 

Além disso, aplicamos **técnicas de programação dinâmica** para otimizar operações, garantindo eficiência e precisão.

---

## Hipóteses e Dados Considerados
- Medidas das amostras simuladas em **centímetros**.
- Cada exame possui **3 medidas** para cálculo do volume.
- Volume aproximado calculado como **produto das medidas**.
- Referência de medidas consideradas normais: entre **0.5 cm e 2.5 cm**.
- Simulação de **22 pacientes**, cada um com um conjunto de medidas.
- Utilização de técnicas de análise estatística para identificação de inconsistências.
- Aplicação de **Programação Dinâmica (DP)** via `@lru_cache`.

---

## Funcionalidades do Sistema
- Cálculo de volume das amostras com **memoization**.  
- Filtros por medidas críticas.  
- Soma total dos volumes com **função recursiva**.  
- Busca binária de exames por ID.  
- Validação de medidas (Dupla checagem automatizada).  
- Análise estatística: média e desvio padrão das medidas.  
- Exportação de relatórios `.txt` e `.csv`.  
- Geração de **gráfico de barras** com volumes.   
- Medição de **tempo de execução** e **uso de memória** com `time` e `tracemalloc`.

---

## Como Executar
1. **Pré-requisitos:**
- **Python 3.x** instalado.
- As seguintes bibliotecas são utilizadas:
| Biblioteca | Instalação |
|------------|------------|
| `matplotlib` | `pip install matplotlib` |
| `csv` | Built-in (não precisa instalar) |
| `statistics` | Built-in |
| `functools` | Built-in |
| `logging` | Built-in |
| `time` | Built-in |
| `tracemalloc` | Built-in |

2. **Instale as dependências:**
```bash
pip install matplotlib
```

3. **Execute o script:**
```bash
python nome_do_script.py
```

4. **Saídas geradas automaticamente:**
- `relatorio_exames.txt` → relatório em texto.
- `relatorio_exames.csv` → relatório em CSV.
- `grafico_volumes.png` → gráfico de barras.
- Mensagens de log informativas.
- Relatório no terminal com análise completa.

---

## Técnicas de Dynamic Programming Aplicadas
| Técnica | Aplicação |
|---------|----------|
| Memoization | `@lru_cache` no cálculo de volume. |
| Recursividade | Soma total dos volumes. |
| Busca eficiente | Busca binária por ID. |
| Análise algorítmica | Estudo de O-grande em cada função. |
| Monitoramento | Tempo e memória analisados. |

---

## Estruturas de Dados
- Lista de dicionários: representa exames e medidas.  
- List Comprehension: filtros otimizados.  
- CSV e TXT: para relatórios estruturados.

---

## Normas e Boas Práticas
- Código modular e comentado.  
- Uso de logging para rastreamento.  
- Tratamento de exceções.  
- Exportações automatizadas.  
- Foco na eficiência computacional.

---

## Cenário Real
Este sistema atende ao **Case 2 da DASA** sobre **Dimensionamento de Amostras**, oferecendo uma solução automatizada para reduzir erros e inconsistências humanas, além de melhorar a eficiência do processo.

---

## Referências
- Python 3.x Official Documentation  
- `functools.lru_cache` — Memoization in Python  
- `matplotlib` — Data Visualization  
- DASA Case — Desafio 2025 FIAP  
