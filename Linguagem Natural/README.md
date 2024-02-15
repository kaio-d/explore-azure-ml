<h1>Azure - Machine Learning</h1>
<p align="center">
Exercício de aprendizado de Máquinas utilizando o Azure para aprendermos sobre o Processamento de linguagem natural
</p>

## 📎 Introdução

- Nesse laboratório trabalhamos com dois conceitos extremamente importantes, sendo eles o Speech Studio na qual utilizamos a função de fala para texto e o Language Studio, sendo capaz de analisar determinado comentário e definifir emoções.


## Utilizando o Speech Studio
<img src="../Linguagem Natural/inputs/speech-studio.png">
<p>Ao utilizar o Speech Studio pude perceber que logo de ínicio temos opções de diversos idiomas, um detalhe sobre o estudo do caso é que quando trabalhamos com fala temos que ter em mente o conceito de análise em tempo real que acaba se diferenciando muito da tradução. Minha experiência ao utilizar o Speech Studio foi que logo de cara pude perceber que algumas palavras a IA tem mais dificuldades para interpretar, porém nunca foge muito da palavra, não captando alguma letra ou coisa do tipo.</p>
<p>Assim como os outros recursos temos um painel bem parecido, sendo possível utilizar algum aúdio salvo em determinado local ou utilizarmos o microfone, conforme monstrado na imagem eu utilizei o microfone e gerei diversas palavras tendo um acerto de quase 100%.</p>

## Language Studio
<img src="../Linguagem Natural/inputs/entrada.PNG">
<p>Ao utilizar o Language Studio utilizamos a função de análisar um comentário com base nos sentimentos, como texto de refência eu optei por utilizar o já oferecido na documentação da Microsoft, sendo um comentário bem pequeno é logo de cara já conseguimos formular uma opnião sobre o caso.</p>
<p>Ao utilizar a função de análise é interessante que a IA possuí alguns pontos bem interessantes para chegar em uma conclusão, sendo eles <strong>Declaração, Entidade e Intenção</strong>, conforme na imagem abaixo ela análisa esses pontos de entrada e gera uma análise que no nosso caso foi negativa</p>
<img src="../Linguagem Natural/inputs/analise.PNG">
<p>É interessante reparar que na sentença TIRED Hotel e poor service ele consegue chegar em uma sentença negativa de 98% e 1 % neutro. Em estudo de caso podemos destacar que quando trabalhamos com diversos comentários essa ferramenta pode ser extremamente útil para demonstrar os pontos fortes e fracos de determinado comércio ou afins.</p>