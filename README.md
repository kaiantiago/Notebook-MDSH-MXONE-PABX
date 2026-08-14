# Notebook-MDSH-MXONE-PABX

Este repositório contém o material de referência utilizado para o **NotebookLM** sobre os comandos do **MDSH (Management and Device Service Handler)** do **Mitel MX-ONE PABX**.

O objetivo deste material é servir como uma base de consulta para administração, operação, diagnóstico e troubleshooting da infraestrutura de telefonia baseada em **Mitel MX-ONE**, utilizada no ambiente corporativo da empresa.

## Conteúdo

O NotebookLM foi desenvolvido a partir de documentações e materiais relacionados aos comandos MDSH, incluindo informações sobre:

* Comandos de administração do MX-ONE;
* Configuração e gerenciamento de ramais;
* Usuários e códigos de autenticação;
* Telefones e dispositivos;
* SIP e recursos relacionados à telefonia IP;
* Configurações do PABX;
* Consulta de status e informações do sistema;
* Diagnóstico e troubleshooting;
* Outros comandos disponíveis no ambiente MDSH.

## Objetivo

Este material tem como finalidade facilitar a consulta rápida aos comandos utilizados no dia a dia da administração e suporte da infraestrutura de telefonia.

O NotebookLM pode ser utilizado para pesquisar comandos, entender sua finalidade, consultar sintaxes e auxiliar na interpretação das informações retornadas pelo sistema.

> **Importante:** os comandos e procedimentos devem ser utilizados com cautela. Alterações realizadas diretamente no MX-ONE podem afetar o funcionamento da infraestrutura de telefonia. Antes de executar comandos que alterem configurações, recomenda-se verificar a documentação correspondente e avaliar o impacto da alteração.

## Ambiente

**Plataforma:** Mitel MX-ONE
**Interface:** MDSH
**Função:** Administração e gerenciamento da infraestrutura de telefonia/PABX corporativo

Este material é destinado principalmente ao uso técnico e à consulta durante atividades de suporte e administração do ambiente de telefonia.

## Observação

O conteúdo do NotebookLM é uma ferramenta de apoio e não substitui a documentação oficial da Mitel nem os procedimentos internos de mudança, segurança e administração da infraestrutura.

## Curadoria de Fontes

Informação extraída de alguns vídeos do youtube e de documentos de texto gerados a partir do comando Help no próprio terminal MDSH da ferramenta. Esses documentos podem ser encontrados neste mesmo repositório.

https://www.youtube.com/watch?v=KviuXiNr_7w
https://www.youtube.com/watch?v=pCGGzGaOChk
https://www.youtube.com/watch?v=ursAwMH1ow0
https://www.youtube.com/watch?v=HrJq7_yUDeU
https://www.youtube.com/watch?v=piPZjBQZGY8

## Engenharia de Prompts

Para obter melhores resultados no NotebookLM, foram elaborados prompts com foco em aprendizagem ativa, análise técnica, troubleshooting e validação das informações.

A estratégia utilizada não foi apenas solicitar respostas diretamente à IA, mas criar uma sequência de perguntas que permitisse explorar a documentação, identificar informações relevantes, comparar comandos e validar possíveis interpretações.

## Estratégia utilizada

A engenharia de prompts foi dividida em quatro etapas:

Exploração: entender os conceitos e funcionalidades disponíveis na documentação.
Aprofundamento: investigar comandos específicos, parâmetros e exemplos de utilização.
Troubleshooting: utilizar a IA para interpretar erros e resultados obtidos no ambiente real.
Validação: solicitar que a IA identifique limitações, ambiguidades e possíveis inconsistências nas respostas.
1. Prompt de exploração inicial

O primeiro objetivo foi fazer com que o NotebookLM apresentasse uma visão geral do conteúdo disponível nas fontes.

Prompt:
"Com base exclusivamente nas fontes deste notebook, apresente uma visão geral do MDSH no ambiente Mitel MX-ONE. Explique qual é sua finalidade, quais tipos de tarefas administrativas podem ser realizadas e quais são os principais grupos de comandos disponíveis."

Objetivo:
Obter uma visão geral antes de estudar comandos individuais e identificar os principais assuntos que deveriam ser aprofundados.

2. Identificação dos comandos relevantes
Depois da visão geral, o objetivo foi identificar comandos úteis para atividades reais de administração e suporte.

Prompt:
"Liste os principais comandos MDSH relacionados à administração e troubleshooting do MX-ONE encontrados nas fontes. Para cada comando, informe sua finalidade, sintaxe básica, parâmetros relevantes e um exemplo de utilização, quando disponível na documentação."

Objetivo:
Transformar a documentação em uma espécie de referência rápida para consulta durante atividades de suporte.

3. Investigação de um comando específico
Para aprofundar o conhecimento sobre comandos individuais, foi utilizada uma abordagem mais estruturada.

Prompt:
"Explique detalhadamente o comando [COMANDO]. Utilize exclusivamente as fontes disponíveis neste notebook. Apresente: finalidade, sintaxe, parâmetros, exemplos encontrados na documentação, possíveis resultados retornados e cuidados antes de executar o comando."

Objetivo:
Evitar respostas genéricas e concentrar a análise em informações efetivamente presentes nas fontes selecionadas.

4. Prompt para troubleshooting
Uma das aplicações mais importantes do NotebookLM foi utilizar a IA como apoio na interpretação de problemas encontrados durante a administração do ambiente.

Prompt:
"Estou executando o comando [COMANDO] no ambiente MX-ONE e obtive o seguinte retorno: [RETORNO]. Com base exclusivamente nas fontes deste notebook, explique o que esse retorno pode indicar. Identifique as possíveis causas, quais comandos ou informações adicionais podem ser consultados e quais verificações devem ser realizadas antes de alterar qualquer configuração."

Objetivo:
Utilizar a IA como ferramenta de investigação, evitando executar alterações no PABX sem compreender previamente o impacto.

5. Prompt para análise de erro
Também foi utilizado um formato específico para diferenciar erros de sintaxe, permissões, configuração e problemas do sistema.

Prompt:
"Analise o seguinte erro do MDSH: [ERRO]. Classifique o problema, se possível, entre erro de sintaxe, permissão/autorização, configuração, estado do sistema ou outra categoria. Explique quais evidências presentes nas fontes sustentam sua interpretação e indique quais informações adicionais seriam necessárias para confirmar o diagnóstico."

Objetivo:
Estimular uma análise baseada em evidências em vez de simplesmente solicitar uma solução.

6. Prompt de comparação entre comandos
Prompt:
"Compare os comandos [COMANDO A] e [COMANDO B] utilizando exclusivamente as informações disponíveis nas fontes. Explique as diferenças de finalidade, sintaxe, parâmetros, impacto no sistema e situações em que cada um deve ser utilizado."

Objetivo:
Facilitar a compreensão de comandos semelhantes e evitar a utilização de um comando inadequado para determinada situação.

7. Prompt para validação da resposta
Uma etapa importante da engenharia de prompts foi solicitar que o próprio NotebookLM apresentasse as limitações da resposta.

Prompt:
"Revise sua resposta anterior. Identifique quais informações estão diretamente sustentadas pelas fontes e quais conclusões podem ser apenas interpretações. Caso exista alguma informação que não possa ser confirmada pelas fontes disponíveis, indique explicitamente essa limitação."

Objetivo:
Reduzir o risco de aceitar como fato uma informação que não esteja presente na documentação utilizada pelo NotebookLM.

##Cicatrizes e dificuldades encontradas

Durante os testes, algumas dificuldades foram identificadas na utilização da IA para consultas técnicas sobre o MX-ONE.
Respostas excessivamente genéricas
Perguntas muito abertas, como:
"Como administrar um MX-ONE?"
produziram respostas amplas demais para uma necessidade operacional.
Ajuste realizado: as perguntas passaram a especificar o comando, o contexto e o resultado esperado.
Falta de contexto operacional
Perguntar apenas pelo significado de um comando não necessariamente fornece informações suficientes para resolver um problema real.
Por isso, os prompts passaram a incluir:

comando executado;
retorno apresentado pelo sistema;
objetivo da operação;
versão do MX-ONE;
informações adicionais relevantes;
solicitação de validação nas fontes.
Risco de interpretações não sustentadas

Em determinados casos, uma resposta pode parecer tecnicamente plausível, mas não estar explicitamente documentada nas fontes.
Para contornar esse problema, foi adicionada uma instrução recorrente:
"Utilize exclusivamente as fontes disponíveis neste notebook."
Também passou a ser solicitado que a IA diferenciasse informações documentadas de interpretações ou inferências.
Necessidade de perguntas de aprofundamento
Outra estratégia utilizada foi solicitar que a IA não respondesse imediatamente quando faltassem informações importantes.

Prompt:
"Antes de apresentar uma solução, verifique se existem informações insuficientes para realizar o diagnóstico. Caso existam, faça perguntas objetivas para obter os dados necessários."
Essa abordagem transforma o NotebookLM de um simples mecanismo de perguntas e respostas em uma ferramenta de investigação técnica.

## Resultado da engenharia de prompts

A utilização de prompts progressivos permitiu transformar o NotebookLM em uma ferramenta de apoio ao estudo e à consulta técnica do Mitel MX-ONE PABX.
O processo passou de perguntas genéricas para uma metodologia baseada em:
Pergunta → Contexto → Investigação → Evidências → Validação → Conclusão
Essa abordagem também permite reutilizar os mesmos princípios em outros ambientes de infraestrutura, documentação técnica e troubleshooting.

## Exemplo de solicitação executada no notebook requisitando uma explicação detalhada do comando extension

Prompt: 
"Explique detalhadamente o comando extension. Utilize exclusivamente as fontes disponíveis neste notebook. Apresente: finalidade, sintaxe, parâmetros, exemplos encontrados na documentação, possíveis resultados retornados e cuidados antes de executar o comando."

Retorno:
O comando extension é um utilitário UNIX disponível no terminal MDSH do sistema MiVoice MX-ONE
. A seguir, é apresentada a explicação detalhada de sua operação com base estrita na documentação técnica disponível.
1. Finalidade
O comando extension é utilizado para alterar (change), apagar (erase), iniciar (initiate/criar) e imprimir (print) dados individuais de usuário, correspondendo à configuração base de um ramal no PABX
. No MX-ONE, os dados configurados por esse comando são categorizados como dados de aplicação ou "dados de intercâmbio" (exchange data)
.
2. Sintaxe
O comando aceita diferentes estruturas de sintaxe dependendo da operação desejada
:
Alteração (Reconfiguração de ramal existente):
extension [-v] [-V] -c -d m [opções...]
Exclusão (Apagar ramal do banco de dados):
extension [-v] [-V] -e -d M
Iniciação (Criação de novo ramal vinculado a um domínio ou LIM):
Opção com domínio de rede:
extension [-v] [-V] -i -d m --domain-name x --csp x [opções...]
Opção vinculada a uma LIM física específica:
extension [-v] [-V] -i -d m -l x --csp x [opções...]
Impressão / Visualização (Consultar dados cadastrados):
Resumo geral:
extension [-v] [-V] -p [-l x] --summary
Detalhamento de ramal:
extension [-v] [-V] -p [-l x] [-d M] [--csp x] [±s [x]] [--customer x] [--type s] [--format x]
3. Parâmetros Principais
Os parâmetros aceitos pelo utilitário definem o comportamento e as facilidades do ramal
:
-i (implicitamente na sintaxe): Inicializa (cria) o ramal
.
-c / --change: Altera ou reconfigura um ramal já existente
.
-e: Apaga (erase) o ramal selecionado
.
-p: Imprime (print) as configurações ou o resumo na tela
.
-d <número>: Define o número de diretório (Directory Number) ou número do ramal
.
-l <número>: Especifica a LIM (Logical Interface Module) física onde o ramal será criado
.
--csp <perfil>: Associa o ramal a um Perfil de Serviço Comum (Common Service Profile), que dita as permissões do usuário
.
--amc <valor>: Configura a categoria para a funcionalidade do cliente móvel Mitel Mobile Client (MMC)
. Valores aceitos: '1', 't', 'true', 'y', 'yes', '0', 'f', 'false', 'n', 'no'
.
--domain-name <nome>: Nome de domínio associado ao ramal
.
--emergency <parâmetro>: Define os parâmetros de tratamento de emergência para o ramal
.
-v / -V: Opções de detalhamento (verbose) na execução do comando
.
Outros parâmetros de facilidades telefônicas: --backup-number, --hotline-number, --hotline-option, --csta-support, --customer, --free-on-second-line, --language-code, --max-call-cost, --secretary, --security-exception, --area-code, --blustar-client-model, --third-party-client, --video, --max-terminals, --edn, --virtual
.
4. Exemplos Encontrados na Documentação
Alterar o Perfil de Serviço Comum (CSP) de um ramal existente: Para alterar as permissões (CSP) do ramal de número 1767 para o perfil de serviço 142:
example% extension -c -d 1767 --csp 142
``` [3]

5. Possíveis Resultados Retornados e Impacto no Sistema
Embora as mensagens exatas de sucesso no prompt (stdout) dependam do ambiente, os impactos lógicos do comando no banco de dados Cassandra e na memória do sistema são definidos da seguinte forma:
Inclusão/Alteração de Dados de Intercâmbio: O comando grava as novas configurações nas bases de dados ativas (Cassandra) em formato CQL no servidor Linux (Service Node)
.
Remoção de Ramais: O comando deleta o ramal da tabela Cassandra ativa imediatamente após sua execução
.
Inconsistência após Restaurações (Cenário de Erro): Caso o sistema sofra uma pane de dados antes que um backup seja realizado, o início pós-restauração (Start After Data Restore) forçará a limpeza de todas as alterações. Nesse cenário, qualquer ramal que tenha sido adicionado ou modificado após o último backup válido do sistema será apagado ou revertido
.
6. Cuidados Antes de Executar o Comando
Necessidade de Backup Imediato: As modificações feitas pelo comando extension não são salvas automaticamente em arquivos de backup persistentes na hora
. O administrador deve executar um backup de dados manual (data_backup) logo após as alterações
.
Risco de Perda de Dados em Restores: Se ocorrer uma falha grave e o sistema precisar restaurar dados do banco Cassandra, as informações serão revertidas ao estado exato do último snapshot gerado
. Se o comando extension foi executado mas nenhum backup foi gerado posteriormente, todas as novas criações serão descartadas na inicialização regenerativa
.
Uso de Backups Agendados (crontab): Para mitigar o esquecimento de backups manuais pós-configuração de ramais, certifique-se de que a conta de administração (mxone_admin) possua rotinas de data_backup configuradas no agendador de tarefas do Linux (crontab -e)


