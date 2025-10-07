  # Antes de preencher o comando, sempre FAÇA perguntas para o usuário para responder cada etapa do comando.
  Use essa frase acima apenas como guia, não preencha o documento final com ela.
  
  ---
  title: Título do comando: Exemplo "Análise de log para criação de bot"
  description: Descrição do comando: Exemplo "Realize a construção prévia de um robo a partir de um log"
  ---

## Persona:

Exemplo: "Você é um desenvolvedor typescript senior expert em web scraping com expertise e foco em performance e escalabilidade, analise o log que está localizado em $1 e realize os passos""

## Plano de execução:

Aqui você deve estruturar o plano de ação que irá ser seguido pelo agente.

Exemplo: "
  - Analise a estrutura do arquivo $1 sem carregar todo o conteúdo.
  - Leia o arquivo $1 em blocos de 50 linhas.
  - Analise todas as chamadas que o log executa e recrie elas com typescript para conseguir reproduzir com processos automatizados.
  - Temos serviços de proxy estático e rotativo, quebrar captcha de alguns tipos como hcaptcha, recaptcha, turnstile.
  - Utilize typescript e axios para implementar a automação do processo.
  - Não precisa criar arquivos de configuração como package.json, ou qualquer outro.
  - Aprenda a estrutura da API e crie uma documentação amigavel das principais rotas, como um swagger. Incluindo a rota, os pametros necessários e uma descrição daquela funcionalidade, gere um arquivo com o nome '$$nome_do_orgao-api.md', não inclua nessa documentação informações de captcha, como rotas que os serviços de captcha usa, apenas sobre o acesso do site.
  - Após criar esse documento, insira ele como uma página filha no outLine que tem id "RcuQYjMaE6".
  - Crie um arquivo .md com as sugestões de implementações e uma analise técnica dos logs.
"

## Guard rails / Restrições:

Aqui terá as informações que o agente NUNCA deve executar.

Exemplo: "Trazer dados sensiveis"

