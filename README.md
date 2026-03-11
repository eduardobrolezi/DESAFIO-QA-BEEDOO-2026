# DESAFIO-QA-BEEDOO-2026
 Desafio de analise e teste de módulo de cadastro e listagem de cursos

 
•	Qual você acredita ser o objetivo da aplicação?

Acredito que o objetivo da aplicação seja gerenciar e centralizar cadastro e registro de cursos presenciais e online cadastrados na aplicação.

•	Quais são os principais fluxos disponíveis?

Fluxo de navegação inicial:  Na tela inicial temos como segui para listar os cursos e cadastrar curso.

Fluxo de listagem de cursos: Ao ir para esse fluxo ainda tela inicial a aplicação lista todos os cursos cadastrados.

Fluxo de cadastro de curso:  Ao ir para esse fluxo a aplicação vai para outra página onde é possível criar um cadastro de um curso, com os campos para preencher com informações (Nome do curso, descrição do curso, instrutor, url da imagem de capa, datas de início e fim, números de vagas, tipo do curso online ou presencial, endereço ou link para as aulas).

• Quais pontos do sistema você considera mais críticos para teste?

1. Salvar os dados e aparecer na lista
O principal é garantir que, quando eu clicar em "Cadastrar", os dados cheguem de verdade no banco. Não adianta nada o usuário preencher tudo e, depois do refresh, o curso sumir ou aparecer com o instrutor errado. O que foi digitado tem que ser exatamente o que aparece na listagem da aplicação.

2. Cuidado com as datas
A aplicação não pode deixar o usuário fazer bobeira, tipo colocar que o curso termina antes de começar. Se a data de fim for menor que a de início, o registro fica todo errado e vai dar erro na lógica lá na frente.

3. Validação do campo de vagas
No campo de vagas, a gente tem que travar para aceitar só números positivos. Se alguém digitar uma letra ou colocar "-10" vagas, a aplicação vai se perder nos cálculos de inscrição e pode dar erro no banco.

4. Segurança e botões
A gente precisa cuidar para ninguém tentar injetar scripts maliciosos nos campos de texto (tipo Nome ou URL) para não comprometer a aplicação. Outra coisa importante é travar o botão de "Cadastrar" logo no primeiro clique; se o usuário clicar duas vezes rápido, não pode criar dois cursos iguais.

5. Link da imagem da capa
Como a página mostra as fotos dos cursos, o link da URL tem que funcionar direitinho. Se a imagem quebrar, o layout da aplicação fica todo bagunçado e passa uma impressão ruim para o usuário.

## 📊 Integração com Google Sheets

Para validar que os dados da aplicação estão sendo enviados corretamente para a planilha, acesse as evidências de integração abaixo:

🔗 [Pasta de Evidências (Tabela google Sheets)](https://docs.google.com/spreadsheets/d/1itTaTENAVghTsJvCjuOv46BMFlYPM1ye4lOPS7ljEvA/edit?usp=sharing)


## 📁 Evidências de Teste

Para conferir o funcionamento da aplicação (prints de tela, testes realizados), acesse o link abaixo:

🔗 [Pasta de Evidências - Google Drive](https://drive.google.com/drive/folders/1TxwNAL8U1XbldYjemoWMjtY7xwjG3UEN?usp=sharing)
