MEU FINANCEIRO — PRIMEIRA VERSÃO

O ZIP contém:
- index.html: telas de login, painel, lançamentos e reservas.
- styles.css: layout responsivo para computador e celular.
- app.js: cálculos, lançamentos e integração com Supabase.
- supabase.sql: tabelas e políticas de segurança (cada conta vê somente os próprios dados).

CONFIGURAÇÃO
1. Crie um NOVO projeto no Supabase para o financeiro.
2. No Supabase, abra SQL Editor > New query.
3. Abra supabase.sql, copie todo o conteúdo, cole no SQL Editor e clique em Run.
4. Em Project Settings > API, copie Project URL e a chave publishable (ou anon).
5. Abra app.js e substitua:
   COLE_AQUI_A_URL_DO_PROJETO pela URL do seu projeto.
   COLE_AQUI_A_CHAVE_PUBLICAVEL pela chave publishable/anon.
6. Salve os arquivos e publique a pasta em um serviço de hospedagem estática (por exemplo, GitHub Pages ou Netlify).
7. Abra o site e crie sua conta. Se a confirmação de e-mail estiver ativa, confirme pelo e-mail antes de entrar.

IMPORTANTE
- Não use nem publique a chave service_role/secret no navegador.
- A renda fixa de R$ 2.500 e a média semanal de Uber de R$ 175 aparecem como referência inicial; registre as entradas reais para os totais ficarem corretos.
- Cada usuário tem seus próprios registros protegidos por RLS.
- O saldo mensal considera entradas menos despesas e valores destinados às reservas.
- Esta versão não conecta automaticamente ao banco nem importa transações: os lançamentos são inseridos manualmente.
