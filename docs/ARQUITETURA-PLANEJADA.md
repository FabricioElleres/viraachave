# Arquitetura planejada — ViraChave Financeiro

## Princípios
- Modularidade e validação server-side para operações sensíveis.
- Menor privilégio e separação dos dados por usuário.
- RLS em todas as tabelas com dados privados.
- Segredos apenas em ambiente de servidor.
- Valores monetários armazenados em unidades precisas (por exemplo, centavos inteiros) e formatados em BRL na interface.
- Datas com regras explícitas de fuso e calendário.
- Cálculos financeiros com premissas visíveis e testes.
- Logs sem dados financeiros pessoais desnecessários.

## Domínios previstos
profiles, preferences, transactions (income/expense), categories, debts, debt_payments, budgets, goals, payoff_plans, subscriptions, billing_events, ai_usage, admin_settings e audit_events.

O esquema final deve ser validado antes das migrations. Tabelas, permissões e fluxos não estão implementados neste commit.

## Quitação
- Avalanche: priorizar a maior taxa conhecida.
- Bola de neve: priorizar o menor saldo.
- Quando juros ou capacidade de pagamento forem desconhecidos, mostrar limitações e evitar previsões assertivas.
- Nunca sugerir que alimentação, moradia ou saúde sejam sacrificadas para cumprir uma meta.

## Assinaturas
O estado de assinatura deve ser confirmado no backend por webhook validado do provedor. Um redirecionamento no navegador não autoriza recursos pagos. Não armazenar dados de cartão.

## Segurança e privacidade
Implementar consentimento e transparência adequados, exportação e exclusão de dados, retenção mínima necessária e avaliação de obrigações LGPD. Não declarar conformidade sem análise e testes.

## Status
Este documento descreve intenções, não uma implementação já ativa.
