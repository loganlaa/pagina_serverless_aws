1. Crie a página index.html (com script para ativar funcao lambda ao clicar no botao)



2. Crie uma bucket no S3 para hospedar esse código
  2.1 - Habilite em "PROPRIEDADES" a "Hospedagem de site estático"
  2.2 - Em "PERMISSOES", desative "Bloquear acesso público"
  2.3 - Em "PERMISSOES" --> "Política do bucket", cole o código do arquivo .json para permitir o acesso de leitura a todos
  2.4 - Salve

![bucket_hospedagem](https://github.com/user-attachments/assets/6a946d51-aa88-445e-bb97-7d0f7259a56b)

![bloqueio_pub](https://github.com/user-attachments/assets/b7e1f9b0-4fe9-4f9c-8982-002c14856bbc)


3. Crie a funcao LAMBDA
  3.1 - Usar um esquema
  3.2 - Nome do esquema: Create a microservice that interacts with a DDB table PYTHON
  3.3 - Criar uma função a partir da política da AWS templates
    3.3.1 - Permissões de microsserviço simples
    3.3.2 - Permissões de somente leitura de objetos do Amazon S3
  3.4 - Criar uma API
  3.5 - API HTTP
  3.6 - ATIVAR CORS (compartilhamento de recursos entre origens)
  3.7 - Criar Funcao
  3.8 - Adiciona o código backend (lambda_function.py)

![Captura de tela 2024-08-15 133057](https://github.com/user-attachments/assets/8845d9dc-b11b-4c8e-967e-c8ec8e7b356f)

![Captura de tela 2024-08-15 133112](https://github.com/user-attachments/assets/d628e67e-a294-4045-88bf-70f7cfd4e178)

![Captura de tela 2024-08-15 133203](https://github.com/user-attachments/assets/6daff39d-a58f-4fd8-ac85-5b4acab1fb8e)

![codigo_func](https://github.com/user-attachments/assets/19444c3f-5a36-49f1-80f9-e0770bdb127f)


4. Gerar URL da Funcao
   4.1 - Vá na funcao criada
   4.2 - Configuracoes -- Criar URL da Funcao

![Captura de tela 2024-08-15 134049](https://github.com/user-attachments/assets/bd0fa87d-00bd-4eb9-99ee-1121f6b5606c)

   
5. Colocar a URL da Funcao no codigo HTML da página


6. Adicionar a página na Bucket do S3


    
