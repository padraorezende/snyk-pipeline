
## 🔑 Secrets

É necessário criar os seguintes secrets e configurar a integração com o GitHub Actions:

- API_URL
- DOWNLOAD_URL
- GIT_USER_EMAIL
- GIT_USER_NAME
- SNYK_AUTH_TOKEN
- TOKEN

## 🚀 Intruções 

Para criar os secrets em seu repositório do GitHub, siga as etapas abaixo:

1. Abra o repositório em questão no GitHub.

2. Clique na guia "Settings" (Configurações) na parte superior do repositório.

3. Na página de configurações, clique em "Secrets and variables" (Segredos e variáveis) no menu lateral esquerdo.

4. Clique no botão "New repository secret" (Novo segredo do repositório).

5. Será exibido um formulário para adicionar um novo segredo. Insira o nome do segredo no campo "Name" (Nome) e o valor do segredo no campo "Value" (Valor).

6. Clique em "Add secret" (Adicionar segredo) para salvar o segredo.

7. Repita as etapas 4 a 6 para adicionar todos os segredos necessários.

Certifique-se de nomear os segredos exatamente como estão sendo referenciados no arquivo YAML. Por exemplo, se no arquivo YAML está sendo usado `secrets.SNYK_AUTH_TOKEN`, então você deve criar um segredo com o nome `SNYK_AUTH_TOKEN` no GitHub.


## ⚠️ Observações

Além disso, substitua as seguintes variáveis no arquivo Markdown:

- GITHUB_API_URL: https://api.github.com/repos/{substitua_pelo_repositorio}/issues
- DOWNLOAD_URL: https://github.com/{substitua_pelo_repositorio}/raw/master/results.pdf

Certifique-se de substituir {substitua_pelo_repositorio} pelo nome do seu repositório GitHub.

Dessa forma, o arquivo estará devidamente interligado com as configurações do GitHub Actions e os segredos serão acessados corretamente durante a execução do fluxo de trabalho.