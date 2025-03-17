## Análise de Sentimento e Mineração de Opinião

Este documento descreve o processo de análise de sentimento aplicada ao texto fornecido, inspirado na abordagem do Azure Cognitive Services. A seguir, apresento alguns prints simulados, o fluxo de trabalho e insights obtidos durante o processo.

---

## 1. Descrição do Processo

### Entrada do Texto

- **Texto Fornecido:**  
  Texto foi retirado do primeiro capítulo de Dom Casmurro.

- **Objetivo:**  
  Aplicar técnicas de mineração de opinião para extrair sentimentos e nuances da narrativa.

### Etapas da Análise

1. **Pré-processamento:**  
   O texto foi segmentado e preparado para análise, identificando frases e expressões de interesse.
   
3. **Extração de Sentimentos:**  
   Utilizando a abordagem inspirada no Azure Cognitive Services, foram avaliados:
   - **Sentimento Global:** Pontuação geral ligeiramente positiva.
   - **Aspectos Positivos:** Humor, ironia e apreço estético (como a menção aos versos).
   - **Aspectos Negativos:** Tensão nas interações e desaprovação dos personagens secundários.
     
4. **Mineração de Opinião:**  
   Foram detalhados os aspectos emocionais e estilísticos, segmentando a narrativa em elementos que contribuem para a compreensão do impacto emocional.

---

## 2. Prints

Usando a Analise de Sentimentos com a Mineração de Opiniões tivemos o seguinte analise geral:

![image](https://github.com/user-attachments/assets/f95ace17-1190-4645-9625-f04a54cabab6)

Tivemos 31 analises de frases porém infelizmente a nova versão do site da Azure não permite eu ler esses dados de forma fácil. Gerando uma mini tela no canto, não permitindo eu expandir ela. Porém com o Arquivo em JSON tivemos a seguinte 

| ID  | Sentimento do Documento | Confiança Positiva | Confiança Neutra | Confiança Negativa | Texto da Sentença | Sentimento da Sentença | Confiança Positiva | Confiança Neutra | Confiança Negativa |
|----|------------------------|-------------------|-----------------|-------------------|------------------|---------------------|-------------------|-----------------|-------------------|
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Uma noite destas, vindo da cidade para o Engenho Novo... | neutral             | 0.07              | 0.88            | 0.05              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Cumprimentou-me, sentou-se ao pé de mim... | positive            | 0.96              | 0.03            | 0.01              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | A viagem era curta, e os versos pode ser que não fossem inteiramente maus. | negative            | 0.00              | 0.00            | 1.00              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Sucedeu, porém, que, como eu estava cansado... | negative            | 0.00              | 0.00            | 1.00              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Tanto bastou para que ele interrompesse a leitura... | negative            | 0.10              | 0.19            | 0.71              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | - Continue - disse eu acordando. | neutral             | 0.01              | 0.98            | 0.01              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | - Já acabei - murmurou ele. | negative            | 0.00              | 0.06            | 0.93              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | - São muito bonitos. | neutral             | 0.27              | 0.73            | 0.00              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Vi-lhe fazer um gesto para tirá-los outra vez do bolso... | neutral             | 0.01              | 0.96            | 0.03              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Estava amuado. | neutral             | 0.09              | 0.70            | 0.22              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | No dia seguinte entrou a dizer de mim nomes feios... | negative            | 0.00              | 0.00            | 1.00              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Os vizinhos, que não gostam dos meus hábitos... | negative            | 0.03              | 0.13            | 0.84              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Nem por isso me zanguei. | negative            | 0.01              | 0.43            | 0.56              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Contei a anedota aos amigos da cidade... | positive            | 0.96              | 0.03            | 0.01              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | - Vou para Petrópolis, Dom Casmurro; | neutral             | 0.01              | 0.96            | 0.03              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | A casa é a mesma da Renânia; | neutral             | 0.03              | 0.97            | 0.00              |
| 1  | mixed                  | 0.22              | 0.08            | 0.7               | Vê se deixas essa caverna do Engenho Novo... | neutral             | 0.02              | 0.95            | 0.03              |


## 3. Conclusão

Achei a análise feita pela IA bem interessante, mas um ponto importante para mim é o custo. Fico um pouco preocupado com o impacto financeiro que uma análise em larga escala poderia gerar e ainda gosto de pensar em soluções que não dependam exclusivamente de IA.

Por exemplo, ao analisar se uma loja de varejo está recebendo feedback positivo dos clientes, a avaliação por número de estrelas já fornece um bom indicativo. No entanto, a IA pode contribuir identificando os motivos dos feedbacks negativos, como problemas de durabilidade, atendimento ou tempo de entrega.

Mas se o custo for alto, será que não valeria mais a pena desenvolver um bot sem IA que busque por palavras-chave para identificar essas tendências?

