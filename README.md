# Magazord.
Teste técnico

# 1º Cenário:

Plano de Testes para Integração com Marketplaces

**1. Documentação e Materiais de Apoio**
   
Identificação da Documentação:

- Documentos Oficiais: Primeiro, eu reuniria toda a documentação oficial dos marketplaces – os guias de integração, os manuais de API, os termos de uso, enfim, tudo que eles disponibilizam.
- Especificações Técnicas: Também vou usar as especificações técnicas da integração que o time de desenvolvimento passou. Essas especificações vêm com diagramas, fluxos e requisitos bem detalhados.
- Requisitos do Projeto: Não posso esquecer dos requisitos do projeto que a gente discutiu nas reuniões e que estão registrados, por exemplo, no JIRA. Esses documentos ajudam a entender o que o sistema precisa fazer.
  
Análise da Documentação:

- Vou fazer uma leitura cuidadosa de todos esses materiais pra identificar os fluxos críticos – como, entender exatamente como a atualização do estoque acontece em tempo real e quais são os pontos que podem dar ruim.
- Durante a leitura, anoto dúvidas e pontos de risco que podem ser discutidos com a equipe. Assim, consigo pensar em testes que realmente impactam o negócio.
  
Mapeamento dos Requisitos:

- Cada requisito do sistema vai ser ligado a um ou mais casos de teste. Por exemplo, se o requisito é que o estoque seja atualizado imediatamente após uma venda, eu crio testes para simular essa situação e ver se o estoque muda direitinho.
- Pra manter tudo organizado, uso uma ferramenta de gerenciamento de requisitos (pode ser uma planilha mesmo ou algo como o JIRA) para mapear os requisitos pros testes correspondentes.
  
Ferramentas de Apoio:

- Utilizarei o JIRA para rastrear os requisitos e os casos de teste.
- Também posso recorrer a ferramentas de análise de texto pra identificar pontos chave na documentação e garantir que nenhum detalhe importante seja esquecido.

**2. Abrangência dos Testes**

Funcionalidades a Serem Testadas:

- Estoque: Vou testar se o estoque atualiza corretamente depois de cada venda ou reposição.
- Anúncios: Confirmar que os anúncios são criados, atualizados e removidos como esperado.
- Faturamento: Verificar se a emissão de faturas e a integração com o sistema financeiro acontecem sem nenhum erro.
- Pedidos: Checar se os pedidos são gerados, atualizados, cancelados e rastreados de forma correta.
- Preço: Garantir que qualquer alteração de preço no e-commerce seja refletida direitinho nos marketplaces.
  
Casos de Uso:

- Cenários de Sucesso: Por exemplo, simular um fluxo completo onde um pedido é feito com sucesso, o estoque é atualizado, o anúncio é publicado e a fatura é gerada.
- Cenários de Falha: Testar o que acontece se rolar algum erro na comunicação com a API do marketplace ou se os dados enviados estiverem errados.
- Cenários de Carga: Simular uma situação de alta demanda, com muitos pedidos e atualizações acontecendo ao mesmo tempo, pra ver se o sistema aguentaa.
- Cenários com Dados Inválidos: Inserir dados errados pra confirmar se o sistema valida as informações e mostra mensagens de erro adequadas.
  
Priorização dos Testes:

- Vou priorizar primeiro as funcionalidades que têm maior impacto no negócio, como pedidos e faturamento, porque erros nessas áreas podem causar grandes problemas.
- Também dou atenção especial aos pontos onde a comunicação com os marketplaces é mais crítica, já que esses são os lugares com maior risco de falhas.
- Claro, sempre converso com a equipe pra alinhar e esclarecer dúvidas sobre quais pontos merecem mais atenção.
  
**3. Execução dos Testes**

Ambiente de Teste:

- Utilizarei um ambiente de homologação que simule bem o ambiente de produção, pra que os testes não afetem dados reais mas ainda sejam representativos.
  
Dados de Teste:

- Vou criar cenários com dados fictícios – como produtos, pedidos e clientes – pra simular várias situações.
- Se precisar, posso usar ferramentas para gerar esses dados e cobrir tanto os casos esperados quanto os imprevistos.

Ferramentas de Automação:

- Para testar as APIs, ferramentas como o Postman são essenciais.
- Além disso, para os testes end-to-end, posso usar o Cypress, que permite automatizar os testes e executá-los repetidamente.
  
Registro de Resultados:

- Documentarei tudo em uma ferramenta de gerenciamento de testes, que pode ser a que a equipe já usa.
- Cada teste terá evidências – prints, logs, resultados – e se algum bug for encontrado, vou registrar com detalhes pra facilitar a análise e correção pela equipe de desenvolvimento.

# 2º Cenário:

Plano de Testes para Integração com o Bling
- Básicamente farei quase tudo igual ao Cenário 1.

**1. Documentação e Materiais de Apoio**

Identificação da Documentação:

- Primeiro, eu pegaria a documentação oficial da Bling (como o guia de integração, manuais da API, termos de uso – tudo que eles oferecem).
- Também usaria as especificações técnicas da integração que a equipe de desenvolvimento passou pra gente, como diagramas, fluxos e os requisitos que definem o que deve acontecer.
- Além disso, vou me apoiar nos requisitos do projeto, aqueles que discutimos em reuniões e estão registrados no JIRA ou outra ferramenta.

Mapeamento dos Requisitos:

- Depois de juntar toda a documentação, eu faria uma leitura detalhada pra identificar os pontos críticos – por exemplo, como o estoque deve ser atualizado em tempo real ou como os pedidos são processados.
- Cada requisito vai ser relacionado a um ou mais casos de teste. Pra isso, uso planilhas ou outras ferramentas, onde eu mapeio cada requisito para os testes correspondentes.
- 
Utilização de Ferramentas:

- Pra organizar tudo, uso o JIRA pra centralizar os requisitos e anotações.
- Também posso usar ferramentas simples de análise de texto pra ajudar a identificar os pontos chave.

**2. Abrangência dos Testes**

Funcionalidades a Serem Testadas:

- Sincronização de Produtos: Vou verificar se os produtos do e-commerce estão sendo corretamente importados e atualizados no Bling.
- Atualização de Estoque: Testar se, depois de uma venda ou reposição, o estoque é atualizado em tempo real nos dois sistemas.
- Processamento de Pedidos: Verificar se os pedidos feitos no e-commerce estão sendo refletidos corretamente no Bling, com todas as informações (quantidade, preço, status, etc).
- Geração de Relatórios: Confirmar se os relatórios de movimentação do estoque e vendas estão sendo gerados conforme esperado.

Priorização dos Testes:

- Prioridade máxima para as funcionalidades que impactam diretamente o negócio, tipo atualização de estoque e processamento de pedidos.
- Também vou dar atenção especial aos pontos onde a comunicação com a API da Bling é crítica, pois qualquer falha aqui pode causar grandes problemas.
- E sempre conversar com a equipe pra alinhar e esclarecer dúvidas sobre quais pontos merecem mais atenção.

**3. Execução dos Testes**

Dados de Teste:

- Pra testar, eu vou criar cenários com dados fictícios que simulem situações reais: produtos com variações no estoque, pedidos de diferentes tamanhos e até situações com dados errados pra ver como o sistema reage.
- Posso usar geradores de dados ou mesmo inserir manualmente os dados, se necessário.

Ferramentas de Automação:

- Pra validar os endpoints e os fluxos de integração, eu usaria ferramentas como o Postman (ou o Insomnia, se preferir).
- Para os testes end-to-end, eu rodo frameworks como Robot Framework ou Cypress, que permitem automatizar os fluxos críticos e agilizar o processo.

Registro de Resultados:

- Toda a execução dos testes vai ser registrada em uma ferramenta de gerenciamento de testes, onde eu documente cada caso de teste, com prints, logs e observações.
- Se encontrar algum bug, eu registro com todos os detalhes pra facilitar a correção e a comunicação com os desenvolvedores.

  # 3º Cenário:

  Análise do Problema – Anúncios não Marcados como "Pausado (sem estoque)"


Revisar a Documentação Oficial do ML:

- Primeiramente, eu ia dar uma boa olhada na documentação do ML pra entender certinho qual informação deve ser enviada quando o estoque chega a zero. Por exemplo, ver se a API espera um campo com valor “0” ou se tem algum padrao específico pra acionar o status “Pausado (sem estoque)”.

Comparar com o Comportamento Manual:

- Quando a gente manda a atualização manual com estoque zero, o anúncio muda de status, certo? Então, a documentação provavelmente indica que é preciso enviar essa informação de forma explícita. Se não estiver chegando, pode ser que a integração automática esteja pulando esse passo.

 
Verificar os Logs:

- Segundo o que foi informado, os logs não mostram o envio do estoque “0” quando o item se esgota. Isso me leva a pensar que, automaticamente, o ERP (ou a integração) não está enviando essa info.

Mapeamento do Requisito:

- Se o requisito do projeto diz “quando estoque = 0, o anúncio deve ser marcado como ‘Pausado (sem estoque)’”, é preciso garantir que essa regra esteja sendo aplicada. Se não estiver, é provável que falte alguma condição na integração.

**Possíveis Erros**

Como não tenho acesso direto aos sistemas, aqui vão algumas hipóteses que eu levantaria:

Erro na Integração do ERP com o ML:

- Pode ser que o ERP Magazord não esteja enviando o valor “0” quando o estoque se esgota. Talvez o campo esteja vindo nulo ou com um valor diferente do esperado.

Problema na Comunicação com a API do ML:

- Mesmo que o ERP envie o valor, pode estar ocorrendo alguma perda de informação na transmissão, ou algum delay que faz com que o ML não receba o dado no momento certo.

Falha na Lógica de Atualização Automática:

- Se os anúncios são atualizados corretamente quando a atualização é feita manualmente, pode ser que a rotina automática que deveria detectar o estoque zerado esteja com algum problema ou não esteja sendo acionada.

# 4º Cenário:

Validação de Dados Cadastrais no Sistema de Gerenciamento de Usuários

Casos de Teste:

**1. Nome Completo**
   
Caso 01 – Nome Válido:

Passos:
- Preencher o campo com "Gregory Schulze".
- Enviar o formulário.
- Resultado Esperado: Cadastro realizado com sucesso (sem mensagens de erro).
  
Caso 02 – Campo Vazio:

Passos:
- Deixar o campo vazio.
- Tentar enviar o formulário.
- Resultado Esperado: Exibir mensagem de erro: "Nome completo é obrigatório".
  
Caso 03 – Nome com Caracteres Inválidos:

Passos:
- Preencher o campo com "Gregory123" ou "Gregory@Schulze".
- Enviar o formulário.
- Resultado Esperado: Mensagem de erro informando que não são permitidos números ou caracteres especiais.
  
**2. E-mail**
   
Casos de Teste:

Caso 04 – E-mail Válido:

Passos:
- Preencher o campo com um e-mail válido.
- Enviar o formulário.
- Resultado Esperado: Cadastro realizado com sucesso.
  
Caso 05 – E-mail sem @ ou .com:

Passos:
- Preencher o campo com um formato inválido "gregoryschulze.com" ou "Gregory@Schulze".
- Enviar o formulário.
- Resultado Esperado: Exibir mensagem de erro: "Formato de e-mail inválido".
  
Caso 06 – Campo Vazio:

Passos:
- Deixar o campo em branco e enviar o formulário.
- Resultado Esperado: Mensagem de erro: "E-mail é obrigatório".
  
**3. Número de Telefone**
   
Casos de Teste:

Caso 07 – Número Válido:

Passos:
- Preencher o campo com um número válido.
- Enviar o formulário.
- Resultado Esperado: Cadastro realizado com sucesso.
  
Caso 08 – Número com letras:

Passos:
- Inserir o número com letras "47ABC968159".
- Enviar o formulário.
- Resultado Esperado: Mensagem de erro: "Número de telefone deve conter apenas dígitos".
  
Caso 09 – Campo Vazio:

Passos:
- Deixar o campo em branco e enviar.
- Resultado Esperado: Mensagem de erro: "Número de telefone é obrigatório".
  
**4. Data de Nascimento**
   
Casos de Teste:

Caso 10 – Data Válida (Formato Correto):

Passos:
- Preencher com uma data válida no formato dd/mm/aaaa.
- Enviar o formulário.
- Resultado Esperado: Cadastro realizado com sucesso.
  
Caso 11 – Data Inválida (Futura):

Passos:
- Inserir uma data futura.
- Enviar o formulário.
- Resultado Esperado: Mensagem de erro: "Data de nascimento não pode ser no futuro".
  
Caso 12 – Campo Vazio:

Passos:
- Deixar o campo vazio e enviar.
- Resultado Esperado: Mensagem de erro: "Data de nascimento é obrigatória".
  
**5. Endereço (Rua, Cidade, Estado, CEP)**
   
Casos de Teste para cada subcampo:

Rua:

Caso 13 – Rua Válida:
- Entrada: "Estr. da Madeira, 1875"
- Resultado Esperado: Cadastro com sucesso.

Caso 14 – Campo Vazio:
- Entrada: ""
- Resultado Esperado: Erro: "Rua é obrigatória".

Cidade:

Caso 15 – Cidade Válida:
- Entrada: "Rio do Sul"
- Resultado Esperado: Cadastro realizado.

Caso 16 – Campo Vazio ou com Números:
- Entrada: "" ou "Rio123"
- Resultado Esperado: Erro: "Cidade inválida" ou "Cidade é obrigatória".
  
Estado:

Caso 17 – Estado Válido:
- Entrada: "Santa Catarina"
- Resultado Esperado: Cadastro realizado

Caso 18 – Estado Vazio ou Não Selecionado:
- Entrada: ""
- Resultado Esperado: Erro: "Estado é obrigatório".
  
CEP:

Caso 18 – CEP Válido:
- Entrada: "89165-063"
- Resultado Esperado: Cadastro realizado com sucesso.
  
Caso 19 – CEP Inválido:
- Entrada: "1234" ou "ABCDE123"
- Resultado Esperado: Erro: "Formato de CEP inválido".

Caso 20 – Campo Vazio:
- Entrada: ""
- Resultado Esperado: Erro: "CEP é obrigatório".



