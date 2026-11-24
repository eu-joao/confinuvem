# Protocolo de Migração e Atividades Chave

## Visão Geral

A ConfiNuvem oferece um **portfólio modular de 5 serviços** para migração, modernização e gestão de ambientes cloud (Google Cloud, AWS), com foco em segurança, conformidade LGPD e parceria de longo prazo. Os serviços podem ser contratados **individualmente** (avulso) ou em **Pacote Integrado** com desconto.

| # | Serviço | Nome comercial | Modelo | Dependência |
|---|---------|----------------|--------|-------------|
| 1 | Avaliação de ambiente | **Diagnóstico ConfiNuvem** | Avulso / Gratuito (lead) | Nenhuma |
| 2 | Planejamento de migração | **Plano de Migração ConfiNuvem** | Projeto (hora) | Requer 1 |
| 3 | Execução da migração | **Migração ConfiNuvem** | Projeto (hora) | Requer 2 |
| 4 | Capacitação de equipes | **Trilha ConfiNuvem** | Avulso / Pacote (hora) | Recomendado pós-3 |
| 5 | Gestão contínua (MSP) | **ConfiNuvem Care** | **Mensal recorrente (faixas)** | Independente |

> **Pacote Integrado (Protocolo ConfiNuvem):** Contratação conjunta dos serviços 1–4 com 10% de desconto. Inclusão do serviço 5 (12 meses) adiciona 15% de desconto sobre o total.

---

## Catálogo de Serviços — Escopo e Entregáveis

### 1. Diagnóstico ConfiNuvem (Avaliação)

**Escopo:** Levantamento de inventário (bancos, documentos, sistemas), volumetria, análise de riscos de segurança, verificação de conformidade LGPD/ANPD, avaliação de maturidade cloud, identificação de dependências técnicas.
**Entregáveis:**

- Relatório de Diagnóstico (PDF, 10–15 páginas)
- Mapa de calor de riscos (crítico/alto/médio/baixo)
- Estimativa de esforço (horas) e investimento (R$) para migração
- Recomendação de provedor e arquitetura alvo preliminar
**Duração:** 4–8 horas
**Precificação:** Gratuito (ação comercial — seção 3.5 do plano de marketing) ou R$ 58,49/h avulso.

### 2. Plano de Migração ConfiNuvem (Planejamento)

**Escopo:** Definição de arquitetura alvo (Google Cloud, AWS, Supabase, NeonDB), seleção de ferramentas de segurança (Acronis, HashiCorp Vault) e monitoramento, elaboração de cronograma detalhado (Gantt), cálculo de TCO (Total Cost of Ownership), plano de rollback, matriz de riscos e mitigações, definição de janelas de cutover.
**Entregáveis:**

- Documento de Planejamento de Migração (PDF, 20–30 páginas)
- Cronograma Gantt com marcos e responsáveis
- Orçamento detalhado por fase e recurso
- Matriz de riscos (probabilidade × impacto × mitigação)
- Arquitetura alvo (diagrama + descrição)
**Duração:** 8–16 horas
**Precificação:** R$ 58,49/hora (serviços especializados).
**Requer:** Diagnóstico prévio (serviço 1 ou equivalente fornecido pelo cliente).

### 3. Migração ConfiNuvem (Execução)

**Escopo:** Provisionamento de infraestrutura no provedor escolhido, configuração de segurança (VPC, IAM, criptografia), migração de bancos de dados (dump/restore, replicação, CDC), migração de documentos/arquivos (transferência validada), validação de integridade e performance, cutover planejado com janela de rollback, testes de aceitação (UAT) com o cliente.
**Entregáveis:**

- Ambiente em produção no provedor cloud
- Relatório de Execução de Migração (PDF)
- Checklist de Validação (itens testados, resultados, assinaturas)
- Credenciais, acessos e documentação de operação básica
- Guia de rollback (se necessário)
**Duração:** 20–80 horas (conforme volumetria, número de bancos, complexidade)
**Precificação:** R$ 58,49/hora (serviços especializados).
**Requer:** Plano de Migração aprovado (serviço 2).

### 4. Trilha ConfiNuvem (Capacitação)

**Escopo:** Treinamento em segurança da informação (gestão de senhas, phishing, engenharia social, noções de LGPD/ANPD), operação diária do ambiente cloud (console do provedor, monitoramento básico, backup/restore Acronis, gerenciamento de segredos no Vault), boas práticas de governança e custos (tagging, orçamentos, alertas).
**Entregáveis:**

- Sessões de treinamento (remoto via videoconferência ou presencial)
- Material didático: apostila PDF + vídeos curtos (5–10 min cada)
- Certificado de Conclusão "Trilha ConfiNuvem" por participante
- Avaliação de conhecimento (quiz) com relatório para gestão
**Duração:** 4–16 horas (conforme número de turmas, profundidade e tamanho da equipe)
**Precificação:** R$ 58,49/hora (serviços especializados); incluída no Pacote Integrado.
**Modalidades:** Inclusa no pacote, avulsa para equipe do cliente, ou recorrente para onboarding de novos colaboradores.

### 5. ConfiNuvem Care (Gestão Contínua / Managed Services)

**Escopo:** Gestão proativa do ambiente cloud do cliente pós-migração (ou de ambiente existente).
**Entregáveis e SLA por faixa:** Ver seção 3.6 do plano de marketing (tabelas de faixas Básico/Pro/Enterprise).
**Modelo:** Recorrente mensal (MRR), 3 faixas de preço.
**Independência:** Pode ser contratado sem ter feito a migração com a ConfiNuvem.

---

## Protocolo de Migração Integrado (Serviços 1–4 em sequência)

Quando contratados como **Pacote Integrado**, os serviços 1 a 4 seguem este fluxo com dependências explícitas:

```mermaid
flowchart TD
    A[1. Diagnóstico<br/>Avaliação] --> B[2. Planejamento<br/>Plano de Migração]
    B --> C[3. Execução<br/>Migração]
    C --> D[4. Capacitação<br/>Trilha ConfiNuvem]
    D --> E[5. Gestão Contínua<br/>ConfiNuvem Care<br/>(opcional, recorrente)]
    style A fill:#e1f5fe
    style E fill:#fff3e0
```

### Detalhamento por etapa (Pacote Integrado)

#### Etapa 1 — Avaliação (Diagnóstico ConfiNuvem)

- **Entrada:** Acesso a inventário parcial, entrevistas com stakeholders, acesso read-only a sistemas (se houver).
- **Atividades:** Inventário técnico, volumetria, análise de segurança, LGPD, maturidade cloud, dependências.
- **Saída:** Relatório de Diagnóstico + Mapa de Riscos + Estimativa.
- **Critério de aceite:** Cliente aprova relatório e autoriza (ou não) continuidade.

#### Etapa 2 — Planejamento (Plano de Migração ConfiNuvem)

- **Entrada:** Relatório de Diagnóstico aprovado.
- **Atividades:** Arquitetura alvo, ferramentas, cronograma Gantt, TCO, rollback, matriz de riscos.
- **Saída:** Documento de Planejamento + Cronograma + Orçamento + Matriz de Riscos.
- **Critério de aceite:** Cliente aprova plano e orçamento; assina ordem de execução.

#### Etapa 3 — Execução (Migração ConfiNuvem)

- **Entrada:** Plano aprovado, credenciais de acesso, janelas de manutenção acordadas.
- **Atividades:** Provisionamento, configuração segurança, migração dados/bancos, validação, cutover, UAT.
- **Saída:** Ambiente em produção + Relatório de Migração + Checklist + Credenciais.
- **Critério de aceite:** Checklist de validação 100% verde; cliente assina termo de recebimento.

#### Etapa 4 — Capacitação (Trilha ConfiNuvem)

- **Entrada:** Ambiente em produção, equipe do cliente indicada.
- **Atividades:** Agendamento turmas, condução treinamentos, entrega material, aplicação quiz, emissão certificados.
- **Saída:** Material didático (PDF/vídeo) + Certificados + Relatório de aproveitamento.
- **Critério de aceite:** 80%+ dos participantes com aprovação no quiz; material entregue.

#### Etapa 5 — Gestão Contínua (ConfiNuvem Care) — Opcional

- **Entrada:** Contrato de gestão assinado, acesso ao ambiente.
- **Atividades:** Onboarding (inventário, configuração agentes), operação contínua (backup, Vault, monitoramento, suporte, manutenção, relatórios).
- **Saída:** Dashboard mensal + Relatórios trimestrais + Atendimento SLA.
- **Critério de aceite:** SLA contratual cumprido (disponibilidade, tempo resposta, relatórios).

---

## Atividades-Chave por Serviço

| Serviço | Atividades-Chave Principais |
|---------|----------------------------|
| **1. Diagnóstico** | Levantamento de inventário, análise de volumetria, assessment de segurança, verificação LGPD/ANPD, avaliação maturidade cloud, elaboração de relatório e mapa de riscos. |
| **2. Planejamento** | Definição de arquitetura alvo, seleção de provedor e ferramentas (Acronis, Vault, monitoramento), cronograma Gantt, TCO, plano de rollback, matriz de riscos, validação com cliente. |
| **3. Execução** | Provisionamento IaC, configuração rede/segurança, migração bancos (dump/replica/CDC), migração documentos, validação integridade/performance, cutover, UAT, documentação. |
| **4. Capacitação** | Desenho currículo (segurança, operação, governança), preparação material (PDF/vídeo), condução sessões, quiz avaliação, emissão certificados, relatório gestão. |
| **5. Gestão Contínua** | Onboarding técnico, configuração backup (Acronis), Vault (políticas/rotação), monitoramento/SIEM (alertas, dashboards), suporte N1/N2 (ticket, SLA), manutenção (patches, otimizações), relatórios mensais/trimestrais, revisão compliance LGPD. |

---

## Modelo de Contratação e Precificação Resumo

| Serviço | Modelo | Preço Base | Observação |
|---------|--------|------------|------------|
| 1. Diagnóstico ConfiNuvem | Hora / Gratuito (lead) | R$ 0 / R$ 58,49/h | Gratuito = ação comercial |
| 2. Plano de Migração | Projeto (hora) | R$ 58,49/h | 8–16 h típicas |
| 3. Migração ConfiNuvem | Projeto (hora) | R$ 58,49/h | 20–80 h típicas |
| 4. Trilha ConfiNuvem | Hora / Pacote | R$ 58,49/h | 4–16 h típicas |
| 5. ConfiNuvem Care | Mensal (faixas) | Básico R$ 10.547,88 / Pro R$ 12.368,66 / Enterprise R$ 17.531,10 | MRR de referência; depende das premissas da seção 3.6 do plano de marketing |
| **Pacote Integrado (1–4)** | Projeto (hora c/ desconto) | 10% desconto vs. avulso | 36 h de referência = R$ 1.895,08 |
| **Pacote + Care 12m** | Misto | 15% desconto sobre o total avulso | R$ 127.771,15, usando Care Pro |

---

## Referências

- Plano de Marketing — Seção 3.2 (Catálogo), 3.3 (Precificação serviços especializados), 3.6 (ConfiNuvem Care).
- Plano de Negócios — Missão/Visão, 5W2H, SWOT, Concorrentes.
- ANPD — Resolução CD/ANPD nº 2/2022 (tratamento diferenciado pequeno porte).
- Acronis, HashiCorp, Google Cloud, AWS — Pricing pages (set/2026).
