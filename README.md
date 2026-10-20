# ViraChave Financeiro

**Produto:** Elleres Sistemas  
**Etapa atual:** Protótipo visual — não é um sistema financeiro em produção.

## Objetivo
Ajudar pessoas no Brasil a compreender e organizar receitas, despesas, dívidas, planos de quitação, metas e reserva de emergência, com linguagem simples e sem julgamentos.

## Status
- [x] Repositório inicializado com documentação.
- [ ] Protótipo React/TypeScript.
- [ ] Revisão visual no Lovable.
- [ ] Autenticação real.
- [ ] Banco de dados e políticas RLS.
- [ ] Cálculos financeiros validados por testes.
- [ ] Integração de pagamentos.
- [ ] Assistente de IA.
- [ ] Testes de segurança, acessibilidade e desempenho.

## Arquitetura prevista
- React + TypeScript para a interface.
- Tailwind CSS e componentes acessíveis.
- Supabase/PostgreSQL e autenticação quando a etapa de backend for iniciada.
- Edge Functions para operações sensíveis.
- Provedor de pagamentos com webhooks verificados quando habilitado.
- Integração de IA somente pelo servidor.

Nenhuma dessas integrações deve ser considerada ativa até ser implementada, configurada e testada.

## Direção visual
- Branco e cinza claro como base.
- Verde elegante para progresso.
- Azul-marinho para confiança.
- Mobile-first, português brasileiro, moeda BRL.
- Interface acessível e sem dados fictícios apresentados como resultados reais.

## Regras importantes
- Dados de demonstração devem estar claramente identificados.
- Nunca usar números fictícios como dados financeiros reais de uma conta.
- Não declarar autenticação, RLS, pagamentos ou conformidade legal como concluídos sem testes.
- Nunca expor segredos no frontend.
- Não publicar em produção enquanto o protótipo estiver em validação.

## Desenvolvimento
O repositório GitHub é a fonte oficial planejada do código. A sincronização com o Lovable ainda precisa ser configurada e verificada.

Desenvolvido por **Elleres Sistemas**.
