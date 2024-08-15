# **WEBSITE ESTÁTICO SERVERLESS HOSPEDADO NA AWS**

### 1. Crie a página index.html (com script para ativar funcao lambda ao clicar no botao)



### 2. Crie uma bucket no S3 para hospedar esse código
1. Habilite em **"PROPRIEDADES"** a *"Hospedagem de site estático"*
2. Em **"PERMISSOES"**, desative *"Bloquear acesso público"*
3. Em **"PERMISSOES"** --> *"Política do bucket"*, cole o código do arquivo .json para permitir o acesso de leitura a todos
4. Salve

![bucket_hospedagem](https://github.com/user-attachments/assets/6a946d51-aa88-445e-bb97-7d0f7259a56b)

![bloqueio_pub](https://github.com/user-attachments/assets/b7e1f9b0-4fe9-4f9c-8982-002c14856bbc)


### 3. Crie a funcao LAMBDA
1. Usar um esquema
2. Nome do esquema: **Create a microservice that interacts with a DDB table PYTHON**
  
  ![Captura de tela 2024-08-15 133057](https://github.com/user-attachments/assets/8845d9dc-b11b-4c8e-967e-c8ec8e7b356f)
  
3. Criar uma função a partir da política da AWS templates

  ![Captura de tela 2024-08-15 133112](https://github.com/user-attachments/assets/d628e67e-a294-4045-88bf-70f7cfd4e178)
    
4.  Criar uma API
5.  _**API HTTP**_
6. ATIVAR _**CORS (compartilhamento de recursos entre origens)**_
7. Criar Funcao

  ![Captura de tela 2024-08-15 133203](https://github.com/user-attachments/assets/6daff39d-a58f-4fd8-ac85-5b4acab1fb8e)

8. Adiciona o código backend (lambda_function.py)

![codigo_func](https://github.com/user-attachments/assets/19444c3f-5a36-49f1-80f9-e0770bdb127f)


### 4. Gerar URL da Funcao
1. Vá na funcao criada
2. Configuracoes -- Criar URL da Funcao

![Captura de tela 2024-08-15 134049](https://github.com/user-attachments/assets/bd0fa87d-00bd-4eb9-99ee-1121f6b5606c)

   
### 5. Colocar a URL da Funcao no codigo HTML da página


### 6. Adicionar a página na Bucket do S3

## RESULTADO
![Captura de tela 2024-08-15 152610](https://github.com/user-attachments/assets/de222fe9-6af7-44d4-8795-479fab223db6)

![Captura de tela 2024-08-15 152631](https://github.com/user-attachments/assets/312f6b7b-a2ed-44e4-bf18-a74c90336329)


    
