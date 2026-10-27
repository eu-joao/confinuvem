# AGENTS.md

Instruções para agentes de IA (e referência rápida para a equipe) neste repositório.

## Contexto

Repositório de documentação da ConfiNuvem, projeto da disciplina de Empreendedorismo do IFPB, Campus Esperança (curso de Análise e Desenvolvimento de Sistemas). Não há código, build, testes nem dependências: todo o conteúdo é Markdown e imagens. Idioma: português do Brasil.

## Estrutura

- `plano-de-negocios.md`: plano de negócios.
- `plano-de-marketing.md`: plano de marketing, que corresponde à seção 3 do plano de negócios.
- `diagrama-modelo-de-negocios.md`: diagrama do modelo de negócios.
- `protocolo-de-migracao-e-atividades-chave.md`: protocolo de migração e atividades-chave.
- `rascunho-plano-de-negocios.md`: rascunho do plano de negócios. Não é a versão de referência.
- `imagens/`: imagens usadas pelos documentos.

Antes de criar um arquivo ou pasta nova, confirme que a estrutura acima realmente não comporta o conteúdo.

## Convenções de escrita

- Escrever em português do Brasil, em tom formal e objetivo, adequado a trabalho acadêmico.
- Títulos em Markdown sem cor, sem emoji e sem ornamentos. Não numerar títulos, exceto nas seções do plano de negócios que já seguem numeração (por exemplo, 3.1, 3.2 no plano de marketing); nesses casos, manter o padrão existente.
- Preferir parágrafos curtos, listas com marcadores ou numeradas conforme o conteúdo e tabelas apenas para dados comparáveis. Sem tabelas decorativas.
- Nomes de arquivos em minúsculas, sem acentos, separados por hífen.
- Lista de integrantes sempre em ordem alfabética.
- Data da capa dos documentos formais: `OUTUBRO/2026`.
- Slogan oficial: "Confiança na nuvem". A logo vigente é a nuvem azul com check sobre fundo escuro.
- Estimativas de valores (pró-labore, marketing, custo variável, lucro e investimentos) devem ser mantidas como estão. Só alterar se a equipe pedir explicitamente.
- Não inventar dados, números, fontes ou citações. Se faltar informação, sinalizar a lacuna em vez de preencher.

## Fluxo de Git

### Integração na main

- Não usamos Pull Requests. As mudanças são integradas por merge direto na `main`.
- Branches são opcionais e devem ser curtas: criar para uma mudança específica, integrar e apagar em seguida.
- Sincronizar com a `main` antes de integrar, para evitar conflitos.

### Commits

Usamos Conventional Commits, com a mensagem em português:

```
tipo(escopo opcional): descrição curta no imperativo

Corpo opcional explicando o porquê da mudança.

Co-authored-by: Claude <noreply@anthropic.com>
```

Tipos mais usados neste repositório:

- `docs`: criação ou alteração de conteúdo dos documentos.
- `fix`: correção de erro de conteúdo, número ou formatação.
- `style`: ajuste de formatação sem mudar o sentido.
- `refactor`: reorganização de seções ou arquivos sem mudar o conteúdo.
- `chore`: tarefas de manutenção do repositório (estrutura de pastas, arquivos de configuração).

Regras:

- Descrição em minúsculas, sem ponto final, com até 72 caracteres.
- Um commit por mudança lógica. Não misturar assuntos diferentes.
- Quando o trabalho tiver participação de IA, incluir o trailer `Co-authored-by: Claude <noreply@anthropic.com>` no final da mensagem. A co-autoria deve ser mantida sempre que possível.

## Regras para agentes

- Não definir autor nos commits ou patches. O autor principal é quem aplica a mudança, com o `user.name` e o `user.email` do próprio Git.
- Ao propor alterações em arquivos do repositório, entregar um arquivo `.patch` e um `commit-msg.txt` com a mensagem no padrão acima, incluindo o trailer de co-autoria.
- Fazer mudanças pequenas e focadas. Não reformatar arquivos inteiros nem reescrever seções que não faziam parte do pedido.
- Não apagar nem sobrescrever o `rascunho-plano-de-negocios.md` sem pedido explícito.
- Não adicionar código, dependências, badges ou arquivos de configuração sem pedido explícito.
- Em caso de dúvida sobre conteúdo do negócio (valores, público-alvo, decisões da equipe), perguntar em vez de assumir.
