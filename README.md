# first-pr-demo

Repositório de prática para aprender o fluxo de Pull Request no GitHub.

## Sobre

Este projeto foi criado para testar o fluxo completo de contribuição via Pull Request: branch, commit, push e revisão.

## uCOPO — gestor de ideias e projetos

`index.html` é uma aplicação web de página única: cola uma ideia (ou várias, uma por linha) e ela é automaticamente:

- **Categorizada** numa sessão da vida (Casa, Capoeira, Finanças) ou num projeto (Phakite, Outros), por palavras-chave no texto.
- **Classificada por relevância** (Baixa / Média / Alta), consoante indica gerar mais bem-estar, mais dinheiro e/ou poupar mais tempo.

Cada ideia pode ser reclassificada manualmente a qualquer momento.

Para usar, basta abrir `index.html` diretamente no navegador — não precisa de build nem de servidor.

**Onde ficam os dados:** aberto como ficheiro (por exemplo, clonado deste repositório), fica tudo no `localStorage` do teu navegador — não há backend nem conta. Publicado como artifact do Claude com a capability `artifact`, a página passa a publicar-se a si própria a cada alteração, e os dados ficam associados a esse artifact (não só ao navegador) — abrir o mesmo link em qualquer dispositivo mostra as mesmas ideias. Nos dois casos, nada é enviado para nenhum servidor terceiro.
