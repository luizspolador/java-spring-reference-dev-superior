## Conteúdos do JavaReference:

- <b>Domínio Complexo:</b> foi implementado um projeto denominado DSLearn com objetivo de trabalhar o relacionamento entre as diversas entidades. Nesse caso, o foco não foi criar as diferentes camadas de uma API Rest, mas, entender e aplicar os conhecimentos de ORM no desenvolvilmento do domínio da aplicação.
  
O modelo conceitual do projeto DSLearn é o arquivo denominado <b>modelo-conceitual-com-forum.png<b/>

- <b>Emails transacionais:</b> o projeto SendGrid tem o objetivo de criar um endpoint para testar o envio de e-mail utilizando a ferramenta SendGrid.

Projeto <b>dscatalog-upload-s3:</b> projeto para o upload de arquivos no Amazon AWS S3.
- Necessário criar uma conta na AWS, configurar o IAM (MFA, criar grupo de usuários com permissão ao storage S3), criar um usuário para ser incluído no grupo criado.

- Necessário criar e configurar o bucket no S3. Incluir uma política (acesso de leitura como público) e configurar o CORS para o bucket.

- Para este projeto, necessário configurar variáveis de ambiente, de acordo com application.properties localizado em resources:

aws.access_key_id=${AWS_KEY:empty}

aws.secret_access_key=${AWS_SECRET:empty}

s3.bucket=${DSCATALOG_BUCKET_NAME:empty}

s3.region=${DSCATALOG_BUCKET_REGION:sa-east-1}
