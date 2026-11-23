# AKCIT
Modelo Estrutuado de Revisão de Escopo (Scoping_Review_Hallucination_Detection_Mitigation_LLMs).

Este arquivo documenta o protocolo de busca, triagem, extração de dados e síntese quantitativa dos estudos primários (Primary Studies - PS).

Estrutura das Abas:
• quantitative-infos: Painel resumo com os números gerais da revisão (total de artigos retornados nas bases, duplicatas removidas, artigos incluídos/excluídos por fase e métricas consolidadas).
• ps-and-paper: Lista mestre dos Estudos Primários (Primary Studies) incluídos na revisão final, contendo ID único do estudo (PS-01, PS-02...), título, autores, ano, veículo de publicação (conferência/periódico) e DOI.
• 1-automated-search: Registro bruto da busca automatizada nas bases de dados científicas (ex: IEEE Xplore, ACM, Scopus, Web of Science), incluindo a string de busca utilizada, data da coleta e status inicial de triagem (título/resumo).
• 2-selection-and-extraction: Aplicação detalhada dos critérios de inclusão e exclusão (leitura completa) e extração dos dados técnicos relevantes para responder às questões de pesquisa.
• technique-per-benchmark: Matriz de mapeamento cruzando as técnicas/abordagens propostas nos estudos com os datasets ou benchmarks utilizados na avaliação experimental.
• temporal-distribution-ps: Análise da distribuição temporal dos estudos primários selecionados por ano de publicação (base para gráficos de evolução da área).

Fluxo de Preenchimento
1. Coleta (1-automated-search): Inserir os metadados exportados das bases e registrar a decisão da 1ª triagem.
2. Seleção e Extração (2-selection-and-extraction): Filtrar os aprovados na etapa anterior, aplicar critérios de elegibilidade e extrair os dados.
3. Catalogação (ps-and-paper): Atribuir um código identificador único (PS-XX) para cada estudo aprovado na etapa 2.
4. Síntese (technique-per-benchmark e temporal-distribution-ps): Mapear os cruzamentos técnicos e verificar a distribuição por ano usando os IDs definidos.
5. Consolidação (quantitative-infos): Conferir os totais e taxas de inclusão (preferencialmente via fórmulas automáticas vinculadas às demais abas).

Boas Práticas e Convenções:
• Não altere os IDs (PS-XX): Eles servem como chave primária para cruzar informações entre as abas.
• Células com fórmulas: Evite sobrescrever valores na aba quantitative-infos e temporal-distribution-ps caso estejam automatizados.
• Controle de versão: Ao atualizar dados ou critérios, registre a data e a alteração realizada.
