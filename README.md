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
# Visão Geral do Projeto
Construa uma aplicação web responsiva chamada "Páginas & Pétalas", um aplicativo de organização de leitura bonito, artístico e minimalista. O objetivo é fornecer uma experiência sem atritos para os usuários rastrearem o que querem ler, o que estão lendo e o que já leram. Toda a interface, textos, botões e alertas do aplicativo devem ser gerados em Português do Brasil.

## Stack de Tecnologia e Configuração de Backend
- Frontend: React, Tailwind CSS, shadcn/ui, Framer Motion.
- Ícones e Arte: Lucide React para ícones da interface. Use CSS ou padrões sutis de SVG no fundo para os elementos florais.
- Backend e Cloud: Supabase (Auth com Google OAuth, PostgreSQL com RLS).
- API Externa: Integração com a Google Books API.

## Design System e UI/UX
- Tema e Vibe: Artístico, botânico e aconchegante.
- Paleta de Cores (Tons Pastel): Fundo Creme suave (#FCF9F2), destaques em Verde Sálvia, Rosa Antigo e Lavanda Suave. Texto em Cinza chumbo.
- Tipografia: Serif elegante para títulos e Sans-Serif limpa para corpo.
- Detalhes: Sombras suaves, cantos arredondados e acentos florais.

## Funcionalidades Principais
1. Autenticação: Tela de login e onboarding sem atrito.
2. Motor de Busca: Barra proeminente conectada à Google Books API.
3. As 3 Estantes: Quero Ler, Lendo e Lidos.
4. Rastreamento: Input de páginas atuais calculando porcentagem com barra de progresso animada.
5. Avaliação: Modal "Livro Concluído" pedindo nota (1 a 5 estrelas) e nota privada (texto).
6. Dashboard: Mural de conquistas (Livros Lidos, Páginas Lidas).
```
Seguido por alguns prompts para ajustes:
> Quando eu busco por título, autor ou ISBN, aparece "Não coseguimos buscar agora. Tente novamente."

> Quero adicionar um mecanismo de nota para cada livro lido, só que em vez de 1 a 5 estrelas, serão de 1 a 5 flores.

> Adicione a possibilidade de dar nota de forma intuitiva na tela de livros lidos, podendo também alterar notas já dadas, e se for adicionado um pequeno comentário sobre a leitura, ele também aparece discretamente perto a capa do livro.

<img width="1898" height="897" alt="image" src="https://github.com/user-attachments/assets/0224f40e-79f9-4ad8-9cbc-be6cf41f295f" />
<img width="1067" height="531" alt="image" src="https://github.com/user-attachments/assets/20132920-3c41-4a2e-8154-ec172b826bdb" />


