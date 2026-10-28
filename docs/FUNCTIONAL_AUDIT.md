# Auditoria funcional e evidências

## Fonte
Especificação fornecida pelo usuário para IAIRON Ultimate v1.0.0. Trata-se de implementação independente orientada por requisitos. Não houve leitura de instruções privadas nem acesso ao agente original.

## Documentado na especificação recebida
Prompts ultrarrealistas; comunicação PT-BR; prompts EN; identidade do avatar; referência fotográfica; brief incompleto; inspiração em modelos anteriores; fotografia cinematográfica.

## Exemplos históricos relatados pela especificação
Corporativo, estúdio, lifestyle, turismo, aventura, esporte, coleções extensas, revisão de costas/perfil, explicação técnica e expansão de descrição. Os artefatos históricos não acompanharam a especificação: sua execução não foi confirmada independentemente. Não confundir relato com evidência medida.

## Implementado nesta versão
Seis camadas, todos os modos do núcleo, seis referências, quatro exemplos, 18 casos de aceitação, validador estrutural e CI. A presença dessas instruções é verificável nos arquivos; eficácia do comportamento depende de execução no host.

## Dependente de testes
Equivalência com original; precisão facial por modelo; Freepik atual; coleções de 30/50; análise multimodal em diferentes hosts; geração direta opcional. Nenhum desses itens é declarado aprovado apenas porque os arquivos existem.

## Rastreabilidade
Criação e realismo → núcleo e photography-foundations; identidade → avatar-identity; estúdio → studio-lighting; geografia → location-realism; séries/revisão → prompt-patterns; diagnóstico → troubleshooting. Casos T01–T18 cobrem esses grupos em testes de aceitação.
