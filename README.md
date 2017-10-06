#### Implantação do GitFlow
O objetivo aqui é organizar os commits em branchs padrões, gerando menos conflitos na base. Otimizar as tarefas entre a equipe e descentralizar os testes de releases.
O modelo que mais se aproxima da forma atual de trabalho é o GitFlow. Em detalhes abaixo:


![ ](https://github.com/tiagosabadini/fluxo-trabalho/blob/master/docs/git-flow-image.png)

## Descrição dos Branches
- **Master**: A Branch em nível de produção. Todo código produzido deverá se juntar à master após realizar uma bateria de testes;
- **Hotfixes**: Correções urgentes. São branches criadas a partir da master e não precisam passar pela develop devido à sua urgência na correção. Por convenção, essas branches recebem o prefixo **hotfix/**;
- **Release**: (não implementada);
- **Develop**: Todas as outras Branches serão enviadas para a develop para serem testadas juntas. Após esta etapa, é realizada a junção à branch master;
- **Feature**: Branches criadas a partir da develop para novas funcionalidades do sistema. Possuem o prefixo **feature/**. Exemplo: **feature/novo-layout**. Após testes, estas branches são enviadas à develop para, posteriormente serem incluídas na master.
