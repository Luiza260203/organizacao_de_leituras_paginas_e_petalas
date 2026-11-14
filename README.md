# organizacao_de_leituras_paginas_e_petalas
O Páginas &amp; Pétalas é uma aplicação web minimalista e artística projetada para ajudar leitores a organizarem sua vida literária sem atritos. a plataforma permite que os usuários acompanhem os livros que desejam ler, os que estão lendo no momento e seu histórico de leituras concluídas.

# 🌸 Páginas & Pétalas: Aplicativo de Organização Literária
<img width="1900" height="852" alt="image" src="https://github.com/user-attachments/assets/d585126d-bddb-4e14-b746-7fa2693c1bb2" />

📖 O **Páginas & Pétalas** é uma aplicação web minimalista e artística projetada para ajudar leitores a organizarem sua vida literária sem atritos. Com um design baseado em tons pastel e elementos botânicos, a plataforma permite que os usuários acompanhem os livros que desejam ler, os que estão lendo no momento (com uma barra de progresso interativa baseada no número de páginas) e seu histórico de leituras concluídas. A interface principal apresenta um painel de conquistas com o total de páginas e livros lidos, além de um motor de busca integrado para encontrar novas obras facilmente.

> Link de Acesso: https://ginas-e-p.lovable.app
---

## 💔 A Dor Escolhida e a Oportunidade de Negócio

*   **A Dor:** Leitores assíduos e estudantes universitários frequentemente perdem o controle do que estão lendo ou desejam ler. Plataformas tradicionais tornam-se redes sociais poluídas, repletas de fricção de usabilidade e focadas na interação social, deixando de lado a simplicidade do registro e a recompensa visual do progresso individual.
*   **Por que é um bom negócio:** O nicho de leitores no Brasil é vasto, mas o segmento de leitores frequentes (especialmente o público universitário e jovem adulto) é altamente engajado. Uma ferramenta que ofereça uma experiência "single-player" impecável foca na **retenção diária** através da gamificação sutil (atualizar páginas lidas). Essa alta retenção permite a monetização futura através de parcerias B2B (editoras e autores independentes) e doações da comunidade, sem depender de anúncios intrusivos.

---

## 📊 Tamanho de Mercado (TAM/SAM/SOM)

*   🌍 **TAM (Brasil):** 93,4 milhões de leitores.
*   🗺️ **SAM (Minas Gerais):** 8,6 milhões de leitores.
*   📍 **SOM (Viçosa - MG):** 33,6 mil leitores potenciais (operando como laboratório universitário/MVP).

## 🧩 Business Model Canvas (Resumo)

*   **👥 Segmentos de Clientes:** Leitores ávidos, estudantes universitários e entusiastas da literatura.
*   **🎁 Proposta de Valor:** Plataforma sem atrito, esteticamente agradável, com foco no progresso individual e gestão visual das leituras.
*   **📣 Canais:** Instagram, marketing boca a boca no campus (UFV), Book influencers.
*   **🤝 Relacionamento:** Automação self-service e co-criação com a comunidade *early adopter*.
*   **💰 Fontes de Receita:** Doações (Pix, Apoia.se), parcerias B2B (patrocínio de lançamentos) e afiliados (Amazon).
*   **⚙️ Recursos Principais:** Plataforma web (Supabase/React), design UI/UX e APIs de dados (Google Books).
*   **🛠️ Atividades Principais:** Desenvolvimento do produto (foco no *Core Loop*), marketing de conteúdo literário.
*   **🔗 Parcerias:** Booktokers/Bookstagrammers, editoras independentes, provedores de APIs.
*   **💸 Estrutura de Custos:** Infraestrutura em nuvem, ferramentas de marketing e horas de desenvolvimento.

---

## 🧪 A Tese do MVP e o que ficou manual (de propósito)

**A Tese Principal:** 
O MVP testa a premissa de que a **recompensa visual** de ver uma barra de progresso se encher, aliada a um painel que soma as "páginas lidas", é o gatilho psicológico para fazer o usuário retornar ao app.

---

## 🤖 O Mega Prompt e Ajustes

Para gerar a base do projeto no Lovable, utilizamos o seguinte Mega Prompt focado em UI/UX e regras de negócio:

```markdown
## Visão Geral do Projeto

Construa uma aplicação web responsiva chamada "Páginas & Pétalas", um aplicativo de organização de leitura bonito, artístico e minimalista. O objetivo é fornecer uma experiência sem atritos para os usuários rastrearem o que querem ler, o que estão lendo e o que já leram. Toda a interface, textos, botões e alertas do aplicativo devem ser gerados em Português do Brasil.

## Stack de Tecnologia e Configuração de Backend

Frontend: React, Tailwind CSS, shadcn/ui, Framer Motion (para barras de progresso animadas e transições de modais suaves).

Ícones e Arte: Lucide React para ícones da interface. Use CSS ou padrões sutis de SVG no fundo para os elementos florais.

## Backend e Cloud (Integração Nativa do Lovable):

Use Supabase para todo o backend.

Configure o Supabase Auth com Google OAuth (Login Social) para um onboarding de 1 clique.

Configure um banco de dados Supabase PostgreSQL com Row Level Security (RLS) para que os usuários só possam ler/escrever seus próprios livros.

API Externa: Integre com a Google Books API para a busca de livros.

## Design System e UI/UX

Tema e Vibe: Artístico, botânico e aconchegante.

Paleta de Cores (Tons Pastel):

Fundo: Creme suave ou off-white (#FCF9F2).

Destaques: Verde Sálvia (#A3B19B), Rosa Antigo (#D9A5B3), Lavanda Suave (#C8B8D1).

Texto: Cinza chumbo escuro (não usar preto puro) para melhor legibilidade e conforto visual.

Tipografia: Use uma fonte Serif elegante para os títulos (como Playfair Display ou Merriweather) e uma Sans-Serif limpa para os textos em geral.

Detalhes de Estilo: Use sombras muito suaves, cantos bem arredondados (rounded-2xl ou rounded-3xl) e acentos florais sutis no fundo da página ou nas bordas dos cards.

## Funcionalidades Principais (Core Features)

1. Autenticação e Onboarding

Implemente uma tela de login bonita apenas com o botão de "Entrar com Google".
Onboarding sem atrito: Após o login com sucesso, redirecione o usuário instantaneamente para a página "Início/Busca" para adicionar seu primeiro livro.

2. Motor de Busca de Livros

Crie uma barra de pesquisa proeminente e com design elegante.
Ao pesquisar, busque os dados na API do Google Books.
Exiba um grid de resultados mostrando: Capa do Livro, Título, Autor e Total de Páginas.
Cada card de resultado deve ter um botão rápido ou menu dropdown para adicionar o livro em uma das três estantes: "Quero Ler", "Lendo" ou "Lidos".

3. As 3 Estantes (Schema do Banco de Dados e UI)

Crie uma tabela no Supabase para os livros dos usuários com os campos: id, user_id, google_books_id, title, author, cover_url, total_pages, status (quero_ler, lendo, lidos), pages_read, rating, private_note.
Quero Ler: Grid simples com as capas e títulos dos livros.
Lendo: A estante mais interativa (foco no rastreamento).
Lidos (Histórico): O arquivo de livros concluídos.

4. Rastreamento de Progresso (Core Loop)

Para livros no status "Lendo", exiba uma Barra de Progresso animada e de destaque na página inicial.
Forneça um input numérico simples onde o usuário digita em qual página está atualmente.
O aplicativo deve calcular automaticamente a porcentagem (pages_read / total_pages) * 100 e animar instantaneamente o preenchimento da barra de progresso.

5. Avaliação e Notas Privadas

Quando o usuário atualizar o progresso de um livro para o número total de páginas (pages_read = total_pages), dispare automaticamente um modal bonito de "Livro Concluído!".
Este modal deve pedir ao usuário para:
Dar uma nota de 1 a 5 estrelas (ícones de estrelas interativos).
Escrever uma nota privada (opcional) de texto sobre seus sentimentos/resumo do livro.
Altere automaticamente o status do livro para "Lidos" e salve a nota/avaliação no Supabase.

6. Dashboard do Usuário (Conquistas)

Crie uma seção de resumo do perfil no topo da página inicial exibindo:

Livros Lidos: Contagem total de livros no status "Lidos".
Páginas Lidas: Soma de total_pages de todos os livros "Lidos" + as pages_read atuais dos livros "Lendo". (Faça esse número parecer uma grande conquista visual).
Mural: Uma lista com rolagem horizontal ou grid estilo masonry mostrando apenas as capas dos livros que o usuário já terminou.
Instruções Iniciais de Configuração para o Lovable
Estruture o layout da interface com uma barra de navegação inferior (bottom nav) para mobile e uma barra lateral (sidebar) para desktop contendo: Busca, Minhas Estantes, Perfil.
Configure a conexão com o Supabase e o fluxo de Autenticação primeiro.
Construa o componente de busca da Google Books API.
Conecte a funcionalidade de adicionar à estante com o banco de dados do Supabase.
Aplique o design system em tons pastel/floral em todos os componentes desde o início.
```
Seguido por alguns prompts para ajustes:
> Quando eu busco por título, autor ou ISBN, aparece "Não coseguimos buscar agora. Tente novamente."

> Quero adicionar um mecanismo de nota para cada livro lido, só que em vez de 1 a 5 estrelas, serão de 1 a 5 flores.

> Adicione a possibilidade de dar nota de forma intuitiva na tela de livros lidos, podendo também alterar notas já dadas, e se for adicionado um pequeno comentário sobre a leitura, ele também aparece discretamente perto a capa do livro.

<img width="1898" height="897" alt="image" src="https://github.com/user-attachments/assets/0224f40e-79f9-4ad8-9cbc-be6cf41f295f" />
<img width="1067" height="531" alt="image" src="https://github.com/user-attachments/assets/20132920-3c41-4a2e-8154-ec172b826bdb" />


