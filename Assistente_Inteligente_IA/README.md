Neste laboratório, construi um assistente inteligente de IA. Criei uma base de conhecimento e um agente. Anexei a base de conhecimento ao agente e , em seguida, adicionei um rupo de ações. teste o agente para responder perguntas, extraidas da base de conhecimento, e realizar ações atraves do grupo de açções. 

Para auxiliar os usuários com ações (em vez de apenas dar respostas), um grupo de ações, o agente pode invocar funções do aews lambda (ou outras chamadas de api) para executar as funções necessárioas para o usuário. Essas ações podem ser interadas totalmente aos sistemas existentes da empresa para fornecer uma experiência completa e fluída para os usuários, desde o envio da solicitação até a aprovação e conclusão. 

Iniciei com o S3.
<img width="934" height="651" alt="image" src="https://github.com/user-attachments/assets/1bd2f618-04e9-4aa4-b732-0f210e63e07d" />

No bucket, lab-bucket, selecione o arquivo criado para o agent-prompt.txt. Clique em OPEN. 

<img width="647" height="575" alt="image" src="https://github.com/user-attachments/assets/5f380da4-d782-439c-9741-03f700b48ca4" />

<img width="932" height="471" alt="image" src="https://github.com/user-attachments/assets/cc6be42f-8766-4842-853c-ab366d14ade4" />

Escolha do modelo para vetorização dos Embeddings.

<img width="824" height="688" alt="image" src="https://github.com/user-attachments/assets/1e7f5d02-c56b-4c94-83b3-32c1a847926b" />

Importante fazer essa configuração do Método de criação dos vetores

<img width="610" height="562" alt="image" src="https://github.com/user-attachments/assets/5c90a02d-f614-4699-acf2-597c37c57e67" />

Após criar o modelo de vetorização dos Embeddings, sincronize com a fonte de dados. 

<img width="619" height="391" alt="image" src="https://github.com/user-attachments/assets/4<img width="273" height="522" alt="image" src="https://github.com/user-attachments/assets/f22add78-86af-4977-8260-cb237edfe924" />
7bd6380-c491-4cc5-b8da-243093432f2d" />

<img width="617" height="376" alt="image" src="https://github.com/user-attachments/assets/f208e02b-b91c-444e-8b8c-122d426a2f58" />

Busque no canto esquerdo, pelos AGENTES

<img width="273" height="522" alt="image" src="https://github.com/user-attachments/assets/6332262b-075b-44bf-8dc4-a8d4a22562b2" />

Clique para criar agente. 

Dê um nome ao seu agente. Nesse momento, tem como vc habilitar a colaboração entre múltiplos agentes. 

<img width="678" height="829" alt="image" src="https://github.com/user-attachments/assets/4a0edea3-016c-4cdf-94a4-0b31df935e7c" />

Mude o perfil de serviço para o existente

<img width="283" height="642" alt="image" src="https://github.com/user-attachments/assets/1426d6a3-b47f-4544-b8a4-7440d5d51d79" />

Escolha Bedrock_Agent_Role

<img width="380" height="536" alt="image" src="https://github.com/user-attachments/assets/b9d8b396-4c85-44c0-930a-5ac3e98c9250" />

Para modificar o modelo clique na canetinha do modelo (fullscreen)

<img width="826" height="735" alt="image" src="https://github.com/user-attachments/assets/e0497840-ad66-4354-aa6b-6b0f11c97a05" />

<img width="826" height="723" alt="image" src="https://github.com/user-attachments/assets/4577101a-71d1-4fdc-ac98-f2bfc0080d87" />

No modelo, é que se customiza as instruções para o Agente:

<img width="285" height="388" alt="image" src="https://github.com/user-attachments/assets/8d4d352c-f17f-4820-85d2-ead868f4e103" />

You are a professional HR Assistant responsible for helping employees with HR-related policy questions. Follow these guidelines:

1. Primary Responsibilities:
- Answer questions about HR policies using all knowledge bases available
- Maintain professional and friendly tone
- Protect confidential information

2. When handling HR policy questions:
- Include relevant policy references only from available knowledge bases
- If the information is not in the knowledge bases, recommend consulting HR department

3. Limitations:
- Defer sensitive matters to HR department

4. Response Format:
- Be concise and clear
- Confirm understanding before proceeding
- Provide next steps when applicable

Always maintain professionalism and confidentiality in all interactions.

<img width="262" height="364" alt="image" src="https://github.com/user-attachments/assets/e745d3d5-3574-4827-aad9-23ff007666d9" />

Customizar a base de conhecimento do Agente

<img width="262" height="364" alt="image" src="https://github.com/user-attachments/assets/c074f3fa-c4cf-4dfb-bf96-36c07f078ecf" />

<img width="317" height="465" alt="image" src="https://github.com/user-attachments/assets/bcb58c88-c151-415f-b8a6-0fdd41ab6ea5" />

Algumas funcionalidades so funcionam em fullscreen

<img width="244" height="410" alt="image" src="https://github.com/user-attachments/assets/e5112c55-4e6d-4df9-bb0b-07453c18fa57" />

Preparar o agente.

<img width="605" height="652" alt="image" src="https://github.com/user-attachments/assets/65d065dc-c31b-4ed2-a8a7-857768bce910" />

Clique em Testar

se nao funcionar, vá em configurações adicionais e habilite entrada do usuário. 

<img width="986" height="281" alt="image" src="https://github.com/user-attachments/assets/c67ffe29-1092-44e3-9709-e377b59374be" />

O agente parece funcionar bem com a base de conhecimentos fornecida

<img width="410" height="619" alt="image" src="https://github.com/user-attachments/assets/caab2d7f-8129-49db-98f6-616d257ab709" />

<img width="402" height="584" alt="image" src="https://github.com/user-attachments/assets/180f6e46-764f-4b28-ae80-b2b931d96894" />

Preparando o GRUPO DE AÇÕES 

Dè um nome ao grupo de ações e depois modifique a invocação do grupo por uma ação Lambda. Selecione uma função criada por você, que nesse caso foi a submit_benefit. 

<img width="513" height="647" alt="image" src="https://github.com/user-attachments/assets/cea1dfe5-d4f4-4b8c-8d4b-a88b45079c2c" />

Configure a função do grupo de ação com o nome submit_benefits (mesmo da funçao lambda)

<img width="316" height="762" alt="image" src="https://github.com/user-attachments/assets/1c5880cd-bafd-44c9-a813-386f1442c14c" />


Adicionar parâmetros 

<img width="252" height="301" alt="image" src="https://github.com/user-attachments/assets/935b97e0-4740-4bbd-a4c3-2276e4722a4c" />

Crie, prepare e teste. 

<img width="260" height="431" alt="image" src="https://github.com/user-attachments/assets/4697f492-d6e9-4a70-b27d-bf56fbce8c41" />

<img width="235" height="397" alt="image" src="https://github.com/user-attachments/assets/a44d55ef-65f9-4f55-96f2-51bcb68a0d70" />

<img width="266" height="357" alt="image" src="https://github.com/user-attachments/assets/8c46bc2b-71d7-4b6e-9214-6f9dc4009f10" />

<img width="280" height="377" alt="image" src="https://github.com/user-attachments/assets/d1c3c90b-4392-4fd1-a236-67ebb76b44aa" />

Revisar e Codificação das Configurações da Função Lambda

<img width="924" height="597" alt="image" src="https://github.com/user-attachments/assets/7a88b963-fc62-4500-90c5-10d99feafce8" />

DynamoDB para armazenamento das interações do Agente

<img width="934" height="851" alt="image" src="https://github.com/user-attachments/assets/4d2db63a-b4d4-4b44-8711-a9367659085a" />

<img width="872" height="469" alt="image" src="https://github.com/user-attachments/assets/24bd7061-c320-487f-890b-7337697b6ba4" />
