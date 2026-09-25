# first-pr-demo

Repositório de prática para aprender o fluxo de Pull Request no GitHub.

## Sobre

Este projeto foi criado para testar o fluxo completo de contribuição via Pull Request: branch, commit, push e revisão.

## uCOPO — gestor de ideias e projetos

`index.html` é uma aplicação web de página única: cola uma ideia (ou várias, uma por linha) e ela é automaticamente:

- **Categorizada** numa categoria (Casa, Capoeira, Finanças, Negócios e Investimentos, Social, Profissional, Sistemas, Aprendizagem — estas duas últimas, mais Casa, com subcategorias) por palavras-chave no texto. Sem correspondência óbvia, fica "por categorizar".
- **Classificada por relevância** (Baixa / Média / Alta), consoante indica gerar mais bem-estar, mais dinheiro e/ou poupar mais tempo.

No topo, a vista **"Dias da Semana"**: uma grelha de 7 dias × 4 períodos (Manhã, Tarde, Noite, Hábito Empilhado), onde cada célula pode ter pílulas de categoria/subcategoria e uma nota de texto livre editável. Por baixo, sempre visíveis, os cartões de categorias (nome + contagem, com uma seta nas que têm subcategorias) servem de fonte para arrastar: arrasta um cartão de categoria ou, depois de o expandir, de subcategoria, para qualquer célula da grelha para lá criar uma pílula; pílulas já colocadas também se arrastam entre células, e um "×" ao passar o rato remove uma. Clicar numa pílula da grelha leva à lista de ideias dessa categoria/subcategoria, em baixo — a escolha de qual ideia trabalhar fica sempre manual. Clicar num cartão de categoria (fora da grelha) navega, como seria de esperar, para os seus cartões de subcategoria ou lista de ideias, com um breadcrumb para voltar atrás em qualquer nível. O botão "Definições" no canto superior abre a gestão de categorias e subcategorias (criar e renomear).

Dentro de uma categoria, as ideias aparecem como lista compacta (uma linha cada): texto, categoria (só na vista "Todas"/"Por categorizar") e prioridade. Passar o cursor (ou tocar, em ecrãs táteis) revela as ações — copiar, concluir/reabrir, editar o texto, eliminar. Clicar no texto abre o detalhe completo (Bem-estar/Dinheiro/Tempo, imagem, categoria/subcategoria num dropdown dependente).

Marcar uma ideia como concluída tira-a de todas as listas e contagens — fica só acessível no botão "Histórico" (ao lado de "Definições"), onde pode ser reaberta a qualquer momento. O campo de pesquisa por cima da lista procura em todas as ideias, de qualquer categoria (incluindo concluídas), independentemente de onde estiveres a navegar.

Cada ideia pode ter uma imagem anexada (print, foto, etc.) — cola-a com Ctrl+V na caixa de texto, usa o botão "Imagem" ao lado de guardar, ou o "+ imagem" no detalhe de uma ideia já criada. As imagens são reduzidas automaticamente antes de serem guardadas.

Para usar, basta abrir `index.html` diretamente no navegador — não precisa de build nem de servidor.

**Onde ficam os dados:** aberto como ficheiro (por exemplo, clonado deste repositório), fica tudo no `localStorage` do teu navegador — não há backend nem conta. Publicado como artifact do Claude com a capability `artifact`, a página passa a publicar-se a si própria a cada alteração, e os dados ficam associados a esse artifact (não só ao navegador) — abrir o mesmo link em qualquer dispositivo mostra as mesmas ideias. Nos dois casos, nada é enviado para nenhum servidor terceiro.
