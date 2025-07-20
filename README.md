# Gerador de Dicas para Entrevistas com IA (Gemini & Streamlit)

Este projeto implementa um aplicativo web interativo que gera dicas de entrevista personalizadas para candidatos a emprego. Ele aproveita o poder do modelo Google Gemini (gemini-2.5-flash) para atuar como um coach de carreira, fornecendo orientações específicas com base nas informações fornecidas pelo usuário.

## Visão Geral

Preparar-se para uma entrevista pode ser desafiador. Este aplicativo visa simplificar esse processo, oferecendo conselhos sob medida. O fluxo de trabalho é o seguinte:

1.  **Entrada do Usuário:** Através de uma interface amigável do Streamlit, o usuário insere:
    * O nome da empresa.
    * A posição para a qual está se candidatando.
    * Seus pontos fortes.
    * Seus pontos fracos.
2.  **Construção do Prompt:** Um `PromptTemplate` é utilizado para formatar essas informações em uma instrução clara e específica para o modelo Gemini, definindo seu papel como "coach de carreira".
3.  **Geração das Dicas:** O modelo Gemini recebe o prompt e gera um conjunto de dicas de entrevista adaptadas, focando em como destacar os pontos fortes e como abordar os pontos fracos de forma construtiva.
4.  **Exibição da Resposta:** As dicas geradas são apresentadas de volta ao usuário na interface do Streamlit.

## Estrutura do Projeto

* `interview_tips_generator.py`: O script principal do aplicativo Streamlit.

## Tecnologias Utilizadas

* **Python 3**
* **Streamlit**: Para construir a interface web interativa.
* **LangChain Google Generative AI (`langchain_google_genai`)**: Para interagir com o modelo Gemini.
* **LangChain PromptTemplate**: Para criar prompts estruturados.
* **Google Gemini API**: Para o modelo de linguagem (`gemini-2.5-flash`).


## Uso do Aplicativo

Na interface do Streamlit, você encontrará campos de texto para inserir os detalhes da entrevista. Preencha-os e, assim que todos os campos estiverem preenchidos, o modelo será invocado e as dicas de entrevista personalizadas aparecerão abaixo.


## Exemplo de uso:

<img width="1920" height="952" alt="Image" src="https://github.com/user-attachments/assets/dfdeafab-75e5-4e94-94f1-6355b016f79b" />

<img width="1919" height="905" alt="Image" src="https://github.com/user-attachments/assets/da495e13-3cec-4858-a8e7-fe7dc440c85f" />

<img width="1913" height="902" alt="Image" src="https://github.com/user-attachments/assets/0855edf6-3257-40c4-b9a1-c3277d422bf1" />

<img width="1910" height="891" alt="Image" src="https://github.com/user-attachments/assets/b9d6d5fc-2dbc-4f52-a638-2cba9b69be04" />

<img width="1902" height="897" alt="Image" src="https://github.com/user-attachments/assets/3ae80223-3e5a-4702-9858-12038fd4476b" />

<img width="1919" height="933" alt="Image" src="https://github.com/user-attachments/assets/318c949f-06c7-48a9-a450-ed8df25458d4" />
