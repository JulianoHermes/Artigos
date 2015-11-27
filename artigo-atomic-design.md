#### Unoesc Chapecó
#### Pós-graduação em Desenvolvimento Web, Cloud e dispositivos móveis - WebMob
#### Disciplina: HTML5+CSS3
#### Professor: Jean Carlo Nascimento
#### Acadêmico(a): Juliano Gustavo Hermes
#### E-mail: {j.hermes09@gmail.com}
## Atomic Design
#####Resumo:
Atomic Design é uma metodologia, proposta por Brad Frost, com o objetivo de facilitar o desenvolvimento do front-end de sites e sistemas web.</br>
Com o crescimento da web foram adotadas diversas metodologias de desenvolvimento incluindo desenvolvimento de front-end, eis que o mais complicado nesses
casos é que as metodologias apresentavam varios problemas, pois, ou eram dedicadas a sistemas especificos, não podendo ser aplicadas a outros sistemas
ou eram muito abstratas, tornando assim dificil demonstrar um resultado para o cliente final antes que o sistema esteja concluido, ou muito complexo
e desgastante, ainda mais levando em consideração que existem pequenos projetos que não tem pessoas ou grupos de desenvolvimento completamente dedicados
a criação de metodologias de desenvolvimento próprias, entre outras dificuldades encontradas nas metodologias atuais e design patterns existentes. </br>
Então se voltando para química Brad tirou a inspiração para a metodologia de desenvolvimento "Atomic Design", onde o sistema seria como um ser ou objeto
que é composto de objetos menores que por sua vez são compostos por objetos menores até o menor objeto possivel, e ele aplicou essa visão ao modelo
tendo assim a seguinte estrutura:</br>
<img src="http://bradfrost.com/wp-content/uploads/2013/06/atomic-design.png">

#####1) O que é?
é uma metodologia de design que visa facilitar a visualização e o entendimento do projeto não apenas para o programador mas para toda a cadeia de
pessoas que participa do projeto. essa metodologia vêm desde o abstrato que seriam os atomos até as páginas de uma maneira lógica e intuitiva que
é fácil de entender e fácil de aplicar.
#####2) Como funciona
o Atomic Design funciona da seguinte maneira, você inicia se preocupando e desenvolvendo partes micro se preocupando fazer aquela micro funcionalidade
boa e parte para a próxima etapa juntando essas funcionalidades e continua agrupando até possuir o resultado final.
então vamos por partes
######Átomo:
o átomo é a menor parte de um sistema, sendo por exemplo as tags html, cada tag é um átomo, e tem seu comportamento. 
######Molécula:
A molécula é um agrupamento de átomos que tem um objetivo comum, ou seja, você agrupa tags como label's, input's, button's, que tenham por objetivo
realizar uma tarefa comum.
######Orgânismo:
O orgânismo é mais complexo pois, existem um agrupamento de moléculas que possuem funções específicas mas possuem uma ligação entre si, no caso você
teria uma molécula resposável pelo controle de postagem de um cometário e outra destinada a exibição dos comentários ou de um comentário.
######Template:
Nesta parte você começa a ter uma visão mais palpável do sistema é algo que você pode apresentar para o cliente e ele vai entender que se trata
do sistema, nesta etapa o foco é agrupar os orgânismos de uma maneira que de visão do produto final.
######Página:
A página é o ultimo estado no qual, você já tem um produto com informações reais no qual é possível a iteração do cliente com o produto. Nesse
estágio pode ser modificado o template gerado com a finalidade de se adequar ao sistema, pois aqui se encontram problemas em relação ao conteúdo 
que vai existir no site, entre outros problemas.
#####3) Para que usar
para facilitar o desenvolvimento de sistemas e a reutilização desses orgânismos e moléculas já criadas.
#####4) Onde usar?
por ser uma metodologia de design pode ser aplicada á qualquer criação desse tipo, entretanto teve sua criação voltada para design em sites e sistemas web.
#####5) Exemplos:
######Átomo:
<img src="http://bradfrost.com/wp-content/uploads/2013/06/atoms.jpg">
######Molécula:
<img src="http://bradfrost.com/wp-content/uploads/2013/06/molecule.jpg">
######Orgânismo:
<img src="http://bradfrost.com/wp-content/uploads/2013/06/organism2.jpg">
######Template:
<img src="http://bradfrost.com/wp-content/uploads/2013/06/template1.jpg">
######Página:
<img src="http://bradfrost.com/wp-content/uploads/2013/06/page1.jpg">

#####6) Referências
[tableless.com.br](http://tableless.com.br/o-que-e-design-atomic/)</br>
[www.phase2technology.com](https://www.phase2technology.com/blog/your-frontend-methodology-is-all-of-them-atomic-design-patternlab/)</br>
[bradfrost.com](http://bradfrost.com/blog/post/atomic-web-design/)
