# chatbot_imersao_ia

```markdown
# Sistema de Gestão de Crianças Desaparecidas

Este script Python gerencia informações sobre crianças desaparecidas, armazenando os dados em um arquivo JSON e oferecendo as seguintes funcionalidades:

### Funcionalidades:

- **Obter informações de uma criança:**
  - Busca no banco de dados por nome da criança.
  - Exibe as informações da criança, caso encontrada.

- **Inserir nova criança:**
  - Coleta informações sobre a criança desaparecida: nome, idade, etnia, data e hora do desaparecimento, descrição, link da imagem, local do desaparecimento, informações adicionais, contato da polícia e contato da família.
  - Adiciona a nova criança ao banco de dados.

- **Gerar aviso de alerta:**
  - Utiliza um modelo de linguagem (Google Gemini Pro) para gerar um aviso de alerta com as informações da criança desaparecida.
  - Exibe o aviso gerado.

- **Sair:**
  - Salva o banco de dados atualizado no arquivo JSON.
  - Encerra o programa.

## Estrutura do código:

O script carrega o banco de dados JSON em um DataFrame Pandas. Um menu principal oferece as opções disponíveis ao usuário.

- Funções específicas são definidas para cada funcionalidade:
  - `obter_informacoes_crianca`: busca informações de uma criança pelo nome.
  - `inserir_nova_crianca`: coleta dados e adiciona uma nova criança ao banco de dados.
  - `gerar_aviso_alerta`: gera um aviso de alerta utilizando um modelo de linguagem.

Um loop principal processa as escolhas do usuário e chama as funções apropriadas. Ao sair, o DataFrame atualizado é salvo de volta no arquivo JSON.

### Requisitos:

- Python 3
- Pandas
- Google Gemini Pro (para geração de texto)

### Arquivo JSON:

O arquivo JSON armazena as informações das crianças desaparecidas. Cada entrada representa uma criança e contém os seguintes campos:

- nome: Nome da criança
- idade: Idade da criança
- etnia: Etnia da criança
- data_desaparecimento: Data do desaparecimento (AAAA-MM-DD)
- hora_desaparecimento: Hora do desaparecimento (HH:MM)
- descricao: Descrição física da criança
- imagem: Link para uma imagem da criança
- local_desaparecimento: Local onde a criança desapareceu
- informacoes_adicionais: Informações adicionais relevantes
- contato_policia: Contato da polícia responsável pelo caso
- contato_familia: Contato da família da criança

### Utilização:

Execute o script Python. Navegue pelas opções do menu principal para gerenciar as informações das crianças desaparecidas.

### Observações:

- O script utiliza a biblioteca Google Gemini Pro para gerar o aviso de alerta. Certifique-se de ter a biblioteca instalada e configurada.
- O caminho para o arquivo JSON é definido no código. Ajuste o caminho para corresponder ao local do seu arquivo.
- Este script é um exemplo básico e pode ser expandido para incluir funcionalidades adicionais, como pesquisa por outros critérios, geração de relatórios, integração com APIs de mapas etc.
```
