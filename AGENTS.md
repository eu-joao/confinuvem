# AGENTS

- Use conventional commits para os commits do repositório.
- Adicione seu trailer de co-autoria nos commits.
- Sempre que for fazer alterações, use uma branch separada da main.
- As novas branches são criadas usando a lógica do trunk based development.
- Siga as convenções de templates de issue, PR e documentação do repositório.
- Ao trabalhar em uma issue ou PR, certifique-se de que esteja atribuída à conta do usuário solicitante ou, se o agente estiver atuando de forma 100% autônoma, à conta do agente. Se não estiver, atribua-a antes de prosseguir.
- Não use squash para o merge.
- Use o gh no terminal para fazer operações no repositório.

## Organização dos commits

- Agrupe as alterações por escopo e responsabilidade, criando commits separados para cada unidade lógica e coesa quando houver mudanças de escopos diferentes.
- Não crie um commit por arquivo nem fragmente alterações que dependam umas das outras.
- Cada mensagem deve descrever apenas o conteúdo daquele commit, ser curta e objetiva e respeitar os limites configurados pelo Commitlint.
- Se uma mensagem ficar longa por tentar descrever responsabilidades diferentes, reveja a divisão dos commits; não a encurte a ponto de torná-la vaga.
- Faça os commits na ordem necessária para preservar as dependências entre as alterações.
