# IAIRON Ultimate

Versão 1.0.0 — Cinematic Photography Prompt Engineering.

Skill especializada em converter ideias e referências em prompts fotográficos completos em inglês, com comunicação em português e prioridade para identidade de avatares. Resolve briefs vagos, identidade que deriva e cenas com luz, escala ou anatomia contraditórias.

## Funcionalidades preservadas
Seis camadas: tipo/estilo, sujeito/vestuário, postura/ação, objetos/composição, ambiente, iluminação/atmosfera. Inclui análise de fotografias acessíveis, retrato corporativo, branding, moda, lifestyle, turismo, esporte, natureza, noite e séries completas. Prompts não inventam características físicas de avatares treinados.

## Melhorias Ultimate
Fidelidade máxima, desenho de estúdio, verificação física, realismo de locações, matriz de diversidade editorial e diagnóstico de contradições. Modo guiado mínimo: perguntar apenas o que afeta materialmente o resultado.

## Instalação e ativação
Ver [instalação](docs/INSTALLATION.md). O núcleo está em [.agents/skills/iairon-ultimate/SKILL.md](.agents/skills/iairon-ultimate/SKILL.md). Copie a pasta completa `iairon-ultimate` para a área de skills aceita pelo seu agente. A descoberta e a instalação variam conforme o host; publicar no GitHub não instala automaticamente a Skill no ChatGPT.

Exemplos de pedidos:
- “Use iairon-ultimate para criar um retrato profissional do meu avatar.”
- “Reconstrua a luz desta referência mantendo minha identidade.”
- “Crie 30 prompts completos e distintos para meu branding.”
- “Corrija esse perfil exagerado sem mudar a roupa.”

Entregar referências ao gerador quando o prompt depender delas. Sem suporte a imagem de referência, a fidelidade facial é limitada.

## Estrutura
O núcleo contém seis referências e quatro exemplos completos. `docs/` reúne auditoria, especificação, comparação, instalação e evolução; `tests/` contém 18 casos e um validador; `.github/workflows/validate.yml` automatiza a validação. [Exemplo de estúdio](.agents/skills/iairon-ultimate/examples/studio-portrait.md).

## Compatibilidade, dependências e permissões
O texto principal é portátil e não exige API, chave, geração de imagem ou pesquisa. Visão é opcional para análise real de imagens; pesquisa é opcional para fatos específicos; renderização só ocorre quando solicitada e disponível. Freepik é um destino possível, sem sintaxe proprietária presumida ou compatibilidade de versão comprovada.

O validador usa Python 3.9+ e PyYAML 6.x, declarados em `tests/requirements.txt`. Não depende de serviços externos nem credenciais; a instalação inicial da dependência pode precisar de rede. Actions tem permissão somente de leitura de conteúdo.

## Identidade, evidência e limitações
Não prometer rosto idêntico por texto. Manter referências e atributos fixos; distinguir observação de inferência; não inferir identidade pessoal pela face. Não houve acesso a configurações ocultas nem avaliação empírica do agente original. A especificação recebida é a fonte de reconstrução; exemplos históricos mencionados nela não foram fornecidos para revisão independente.

## Validação e testes
```bash
python -m pip install -r tests/requirements.txt
python tests/validate_skill.py
python tests/test_validator.py
```
O workflow executa esses comandos em push e pull request. Essas verificações são estruturais; os 18 testes comportamentais e as comparações com geradores têm execução separada e não são considerados aprovados automaticamente. Ver [aceitação](tests/acceptance-cases.md) e [comparação](docs/COMPARATIVE_TESTS.md).

## Atualização e contribuição
Revalidar após alterações, registrar mudanças no [changelog](CHANGELOG.md) e seguir [contribuições](CONTRIBUTING.md). Manter casos e evidência de execução separados.

## Licença
MIT, copyright 2026 mxcapellani. Implementação independente sem afiliação oficial ao Freepik ou outros fornecedores.
