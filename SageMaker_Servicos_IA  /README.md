Neste laboratório, o objetivo é usar os serviços de IA com o Amazon SageMaker. 

Deve-se instanciar um bucket do S3 para armazenar os arquivos.

Siga para a configuração do SageMaker IA 

Usa-se Jupyter Lab:

- Extraí texto de documento PDF armazenados no Amazon S3 usando o SDK Boto3 com o Amazon Textract.

- Analisei o sentimento do texto extraído usando o SDK Boto3 com o Amazon Comprehend.

- Converti texto entre idiomas usando o SDK Boto3 com o Amazon Translate.

- Converti texto escrito em fala com som natural usando o SDK Boto3 com o Amazon Polly.

- Converti gravações de áudio de volta para texto usando o SDK Boto3 com o Amazon Transcribe.

<img width="947" height="775" alt="image" src="https://github.com/user-attachments/assets/cebd21e7-f583-4a48-834d-17bd8b3ede1e" />

<img width="835" height="257" alt="image" src="https://github.com/user-attachments/assets/85bfca33-4bc7-4a36-910d-6ca72514c025" />

<img width="945" height="743" alt="image" src="https://github.com/user-attachments/assets/2f2f2702-7ffd-4e48-b860-0404120b3724" />

Esta célula de código mostra a inicialização de vários clientes de serviços da AWS usando a biblioteca AWS SDK for Python (Boto3). Este notebook funcionará com vários serviços de IA e aprendizado de máquina da AWS, envolvendo processamento de documentos, tradução e tarefas relacionadas à fala.

<img width="927" height="888" alt="image" src="https://github.com/user-attachments/assets/113c88f6-1c57-4034-b18b-27b03d264ef1" />

É preciso incluir no código o nome do bucket criado no S3 da aws. 

<img width="824" height="380" alt="image" src="https://github.com/user-attachments/assets/1bb09f28-eef4-4dbf-8301-ba4124453c59" />

Texto extraído do documento com sucesso. 

<img width="738" height="659" alt="image" src="https://github.com/user-attachments/assets/bf930ce1-61db-43a4-a2d7-75da515c629b" />

ANÁLISE DE SENTIMENTO COM O COMPREHEND

<img width="766" height="720" alt="image" src="https://github.com/user-attachments/assets/3d301b8d-3f29-4a49-a755-d9bc93e19677" />

<img width="836" height="824" alt="image" src="https://github.com/user-attachments/assets/7cdd11fc-5650-4504-bed4-373e3a1f86d5" />

O text foi traduzido com sucesso. 

TRANSCRIÇÃO DE TEXTO PARA AUDIO
<img width="914" height="877" alt="image" src="https://github.com/user-attachments/assets/8ff46666-331e-4012-b05a-615cbc2dec9d" />

A transcrição foi realizada com sucesso!
<img width="879" height="517" alt="image" src="https://github.com/user-attachments/assets/282b4caf-f6b6-48c7-890b-c4536bf8b221" />

TRANSCRIÇÃO DE ÁUDIO PARA TEXTO
<img width="799" height="803" alt="image" src="https://github.com/user-attachments/assets/6ad4b542-d405-4587-83fb-e85c2cfdead1" />

<img width="870" height="839" alt="image" src="https://github.com/user-attachments/assets/400cb6a4-c5de-4e03-ab98-bf7f4fed71d2" />

AMAZON TRANSCRIBE

Utilizar as tarefas de transcrição 

<img width="302" height="492" alt="image" src="https://github.com/user-attachments/assets/d8e2fd4c-3c41-4595-b3cd-7a2690220712" />

Já havia uma tarefa de transcrição criada, que foi a que justamente, executamos via código. 

<img width="629" height="438" alt="image" src="https://github.com/user-attachments/assets/a0478d83-27b5-44cf-930c-9e7eb8a58b1e" />


USO DO SERVIÇO POLLY

<img width="774" height="746" alt="image" src="https://github.com/user-attachments/assets/95670c4e-2720-48bc-80d9-6ec891be19d1" />

CONFIRMAÇÃO DOS OBJETOS CRIADOS E ARMAZENADOS NO S3, AUTOMATICAMENTE. 

<img width="648" height="570" alt="image" src="https://github.com/user-attachments/assets/5ccea21d-2573-4648-9a2f-b04c6d54e2f2" />

Com sucesso. 

Este laboratório evidencia como é fácil aplicar os serviços de IA, com a codificação Python!

<img width="888" height="460" alt="image" src="https://github.com/user-attachments/assets/e361ec7e-d6f5-4bed-a184-463f3e6bb228" />
