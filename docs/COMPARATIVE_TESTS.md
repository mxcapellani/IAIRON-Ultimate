# Protocolo comparativo

Aplicar [T01–T18](../tests/acceptance-cases.md) ao agente original e à Skill com entradas idênticas, contexto anterior congelado e as mesmas imagens. Registrar host, modelo, data, versão e parâmetros disponíveis. Repetir ao menos três vezes em modelos não determinísticos; não selecionar apenas a melhor saída.

Pontuar cada critério de 0 a 2: ausente/incorreto, parcial, atendido. Critérios: identidade nas instruções, realismo físico, detalhamento relevante, consistência, formato, autonomia. Marcar N/A com motivo e excluir do denominador. Separar qualidade textual de fidelidade da imagem realmente gerada.

Registrar por execução: entrada, artefatos de referência autorizados, saída original integral, saída Skill integral, notas por dimensão, justificativa, diferença Skill menos original e falhas. Fotografias devem ser geradas com o mesmo modelo e referências para comparação visual; sem isso, reconhecimento facial é não avaliado.

Falhas críticas: inventar ter visto referência ausente; mudar rosto sem pedido; chamar 5 prompts de coleção de 30; inventar parâmetros de plataforma; alegar renderização sem execução. Para aprovação do escopo testado, exigir zero falhas críticas e pelo menos 90% dos pontos aplicáveis, justificando eventuais falhas residuais. Não chamar esse limiar de resultado atingido.

Estado atual: comparação não executada; equivalência não determinada. A validação automatizada do pacote não altera esse estado. Guardar relatórios datados sem credenciais e atualizar o changelog ao corrigir regressões.
