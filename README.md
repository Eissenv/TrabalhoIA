# Projeto de Chatbot com Classificação de Imagens

Este projeto implementa um chatbot do Telegram que classifica imagens enviadas pelo usuário como contendo a letra A ou B.


## Estrutura de Arquivos

treinamento.ipynb: Contém todas as funções relativas ao treinamento dos modelos, tratamento e visualização das imagens.

chatbot.ipynb: Configura o bot e define as funções de resposta para imagens e outras mensagens.

Imagens/: Pasta onde estão localizadas todas as imagens utilizadas para treinar o modelo.

Modelos/: Pasta onde estão localizados os modelos gerados através de treinamento.ipynb.

Teste-Visualizacao/: Pasta onde coloco imagens para testes isolados.

## Execução:

1. Clone esse repositório e coloque os arquivos dentro de uma pasta chamada "TrabalhoIA" no google drive. 

    Caso queira utilizar outra pasta, lembre de mudar os caminhos utilizados durante o treinamento e o chatbot. Veja um exemplo de caminho dentro de treinamento.ipynb: 

    ```python
    # Diretório das imagens
    data_dir = '/content/drive/MyDrive/TrabalhoIA/Imagens'
    ```
---
2. Comece executando o arquivo de treinamento até a parte "Armazenamento dos Modelos".
---
3. Após finalizar o treinamento crie um bot no Telegram e obtenha o token através do BotFather. Esse token deve ser colocado em chatbot.ipynb, na seguinte parte:

    ```python
    # Token do bot do Telegram
    TOKEN = 'YOUR-TOKEN-HERE'
    ```
4. Verifique se o caminho para o modelo que deseja utilizar está correto em chatbot.ipynb: 
    ```python
    # Caminho para o modelo salvo
    model_path = '/content/drive/MyDrive/TrabalhoIA/Modelos/efficientnet_b2.pth'
    ```

5. Execute todo o código de chatbot.ipynb. O bot funcionará após a execução da main().

