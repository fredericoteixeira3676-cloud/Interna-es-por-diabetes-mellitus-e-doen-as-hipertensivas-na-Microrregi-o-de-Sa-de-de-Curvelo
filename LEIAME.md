# Internações por diabetes mellitus e doenças hipertensivas na Microrregião de Saúde de Curvelo (MG), 2008–2025

Estudo ecológico descritivo de série temporal. Compara a Microrregião de Saúde de Curvelo (11 municípios) com Minas Gerais, usando dados públicos do SIH/SUS e estimativas populacionais do IBGE/TCU, ambos obtidos pelo TABNET/DATASUS em 05/11/2026.

- Local de residência do paciente, ano de processamento da AIH.
- Causas: diabetes mellitus (CID-10 E10–E14) e doenças hipertensivas (I10–I15), em conjunto e separadamente.
- Municípios: Augusto de Lima, Buenópolis, Corinto, Curvelo, Felixlândia, Inimutaba, Monjolos, Morro da Garça, Presidente Juscelino, Santo Hipólito e Três Marias.

## Sobre os arquivos da pasta `Dados`

Todos os arquivos são tabelas (.csv) exportadas diretamente do TABNET. A única diferença entre eles é o nome:

- A subpasta `Corrigidos` reúne os arquivos que foram renomeados para facilitar a identificação.
- Os arquivos fora dessa subpasta são tabelas do mesmo tipo, mantidas com o nome original de download (por exemplo, `sih_cnv_nrmg...` e `ibge_cnv_pop...`) ou com o nome da extração (`Extração 1`, `Extração 3`, `Extração 4`). Não foram renomeados, mas fazem parte dos dados do estudo.

O conteúdo exato de cada tabela está escrito nas primeiras linhas do próprio arquivo (título, município ou macrorregião selecionados, Lista de Morbidade CID-10 e período).

### O que há nas tabelas

| Conteúdo | Observação |
|---|---|
| Internações, dias de permanência e valor total por município e ano | Diabetes + hipertensão em conjunto, e diabetes isoladamente |
| Internações por macrorregião de saúde e ano | Conjunto e só hipertensão (referência de Minas Gerais) |
| Internações por faixa etária e sexo | Microrregião, jan/2008–ago/2026 |
| Todas as causas, por município e ano, e por capítulo da CID-10 | Contexto hospitalar |
| Todas as categorias da Lista de Morbidade CID-10 por ano (microrregião: `sih_cnv_nrmg223940138_99_83_78.csv`; Minas Gerais: `sih_cnv_nrmg224134138_99_83_78.csv`) | Comparação com outras causas (seção 3.3 do artigo); jan/2008–ago/2026 |
| Extrações só de hipertensão (valor, dias, faixa etária, macrorregião) | Usadas para verificar a subtração |
| População estimada (IBGE/TCU) por município e macrorregião | 2008–2023 (série histórica) e 2024–2025 (versão atual) |

### Pontos de atenção para quem for reutilizar os dados

- A hipertensão da microrregião foi obtida por subtração (diabetes + hipertensão − diabetes). A subtração foi verificada célula a célula contra extrações só de hipertensão (dias e valor), sem divergências.
- O perfil por idade e sexo inclui jan–ago/2026, pois o TABNET não permitiu restringir essa extração a 2008–2025.
- O TABNET informa que os dados dos últimos seis meses estão sujeitos a atualização; por isso 2026 foi excluído das análises de tendência.
- A população apresenta quebras metodológicas (por exemplo, valores idênticos em 2022 e 2023).
- O valor das AIH segue a Tabela SUS e não é o custo real da internação.
