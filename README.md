# Análise de Sentimentos com Language Studio no Azure AI

## Visão Geral

O Sentiment and Opinion Mining é um recurso do Language Studio, do Azure AI, que permite identificar sentimentos positivos, negativos e neutros em textos. Este repositório apresenta um estudo prático dessa ferramenta, com exemplos de testes realizados.

## Objetivo

Este projeto tem como objetivo explorar a capacidade do Language Studio para análise de sentimentos e mineração de opiniões, demonstrando como essa tecnologia pode ser aplicada na interpretação de textos.

## Tabela de Conteúdo

- [Configuração Inicial](#configuração-inicial)
- [Testando a Ferramenta](#testando-a-ferramenta)
- [Resultados Obtidos](#resultados-obtidos)
- [Conclusão e Insights](#conclusão-e-insights)

## Configuração Inicial

Antes de utilizar o Language Studio, é necessário configurar um recurso no Azure Language Service. Siga os passos abaixo:

1. Acesse o portal do Azure: [Azure Portal](https://portal.azure.com/)
    ![Imagem1 - Acesando Portal](/assets/img/image01.png)

2. Crie um novo recurso Language Service selecionando a opção "Create ou Criar".
     ![Imagem2 - criar o recurso](/assets/img/image02.png)

3. Não precisa selecionar nada, só clique em: "Continue to create your resource".
    ![Imagem3 - continue create](/assets/img/image03.png)

4. Preencha as opções corretamente e Clique em: "Examinar + criar".
     ![Imagem1 - Criar](/assets/img/image04.png)

### Conectando ao Language Studio

1. Acesse o [Language Studio](https://language.cognitive.azure.com/).


2. Na página inicial, clique em "Select a resource".
    ![Imagem1 - selecionando resource](/assets/img/image06.png)

3. Escolha o recurso criado e configure como padrão.

## Testando a Ferramenta

Com o recurso configurado, podemos testar a ferramenta na seção "Analyze Sentiment and Mine Opinions", localizada na aba "Classify Text" do Language Studio.

![Imagem1 - Classify Text](/assets/img/image07.png)


Para este experimento, utilizei um trecho do livro da bíblia - Salmos 23 - para verificar como a ferramenta classifica diferentes sentenças.

![Imagem1 - Texto - salmo 23](/assets/img/image08.png)

## Resultados Obtidos
Os testes realizados indicaram uma classificação mista, com predominância de sentimentos positivos, mas com algumas sentenças sendo classificadas como negativas. A taxa de confiança foi moderada, refletindo que a ferramenta teve mais facilidade em identificar sentimentos claros de consolo e confiança, mas encontrou dificuldades ao interpretar trechos com metáforas ou sentimentos mais sutis, como no caso do "vale da sombra da morte".

- **Texto analisado:** Salmo 23
- **Classificação geral:** Mista (com predominância de sentimentos positivos)
- **Confiança:** 66 % em média

![Imagem1 - resutado 1](/assets/img/image10.png)


![Imagem1 - resultado 2](/assets/img/image11.png)


## Conclusão e Insights

A análise de sentimentos pode ser útil para entender emoções expressas em textos, como é o caso do Salmo 23, onde a ferramenta conseguiu identificar sentimentos de confiança, consolo e segurança. No entanto, observamos que a ferramenta apresentou dificuldades em interpretar com precisão algumas partes do texto, especialmente em trechos que envolvem metáforas e um contexto mais profundo, como o "vale da sombra da morte".

Uma abordagem mais avançada, capaz de considerar o contexto geral do salmo e correlacionar as sentenças de maneira mais eficaz, poderia melhorar os resultados. Além disso, o uso combinado com outras ferramentas de IA, que possam entender melhor nuances poéticas e espirituais, pode tornar a análise mais precisa.

Este repositório faz parte do aprendizado adquirido no Bootcamp Microsoft Azure AI Fundamentals, da DIO.
