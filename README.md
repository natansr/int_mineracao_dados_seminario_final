
Seminário Final da disciplina Introdução a Mineração de Dados do curso Big Data Analytics da Faculdade SENAC/DF

# Classificação de Documentos para Desambiguação de Nomes de Autores (AND)

## Introdução
Nesse tutorial vamos fazer o fine-tuning de um modelo transformer (BERT) para Classificação Multiclasse de documentos.

Vamos utiliza-lo para performar e resolver o problema de Desambiguação de Nomes de Autores (AND) de determinado repositório bibliográfico digital ou dataset.

## Fluxo do Notebook
O notebook será dividido em seções separadas para fornecer uma caminhada organizada através do processo utilizado. Este processo pode ser modificado para casos de uso individuais. As seções são:

1. Importando Bibliotecas Python e preparando o ambiente
2. Importando e Pré-processando os dados do domínio
3. Preparando o Conjunto de Dados e o Carregador de Dados
4. Criando a Rede Neural para Ajuste Fino
5. Fine Tuning e ajuste do Modelo
6. Validando o Desempenho do Modelo
7. Salvando o modelo e artefatos para Inferência Futura

## Detalhes Técnicos
Este script utiliza várias ferramentas projetadas por outras equipes. Detalhes das ferramentas utilizadas abaixo. Certifique-se de que esses elementos estejam presentes em sua configuração para implementar com sucesso este script.

### Modelo de Linguagem Usado:
O SciBERT é um modelo de linguagem baseado em transformers, desenvolvido especificamente para tarefas relacionadas ao domínio científico.

- Postagem no Blog
- Artigo de Pesquisa
- Documentação para Python

### Dados:
Estamos utilizando o conjunto de dados AMiner para desambiguação de nomes, disponível no repositório UCI Machine Learning Repository. Este conjunto de dados é usado para resolver o problema de desambiguação de nomes, onde o mesmo nome pode se referir a diferentes pessoas em diferentes contextos.

- Artigo de Pesquisa
- Documentação
- Download

## Requisitos de Hardware:
- Python 3.6 e superior
- Pytorch, Transformers e todas as bibliotecas de Machine Learning padrão do Python
- Configuração habilitada para GPU

## Objetivo do Script:
O objetivo deste script é ajustar o SciBERT/BERT para ser capaz de classificar um título e resumos de documentos (publicações) em classes de autores.

## Ambiente de Execução
Este notebook foi executado no Google Colab utilizando uma instância com GPU NVIDIA A100 para acelerar o treinamento e inferência do modelo.

## Testes Iniciais
Os testes iniciais foram executados com instâncias de um único autor, por exemplo, 'Hongbin Liang', com 16 classes. Não foram treinados todos os dados do dataset para inferência de classes de todos os autores com nomes ambíguos. Portanto, é melhor performar para um autor em questão que esteja com nome ambíguo no dataset.

## Contexto Acadêmico
Este projeto foi realizado como parte do projeto final da disciplina de Introdução a Mineração de Dados da Especialização em Big Data Analytics da Faculdade SENAC/DF.

## Apresentação
A apresentação relacionada a este projeto está disponível na pasta "beamer" deste repositório.

## Contato
Para qualquer dúvida ou sugestão, por favor entre em contato pelo email natan5souza@gmail.com.
