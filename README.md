# DESGOVERNO v1.8 — ESTADO DE BARZI

Simulador fictício de gestão política da República Democrótica de Barzi. Esta versão parte da v0.9.4 e preserva seus sistemas anteriores, adicionando uma camada de instabilidade social, institucional, econômica e urbana.

## Novidades da v1.8
- Confirmação para reiniciar a campanha exibida em uma janela temática dentro do próprio jogo, sem o diálogo nativo do navegador.
- Identidade visual do Estado de Barzi reforçada no cabeçalho, com brasão, nome em destaque e identificação da capital Nova Aurora.
- Alertas, cutscenes e eventos continuam usando o painel modal interno do jogo.

## Como executar no VS Code
1. Extraia `Desgoverno_v1.0_VSCode.zip`.
2. Abra a pasta `desgoverno_v10` no VS Code.
3. Abra `index.html` no navegador ou use a extensão **Live Server**.
4. Clique em **SOM: ON** para liberar música e efeitos (o navegador exige interação do jogador).

Não é necessário instalar dependências nem executar servidor Node.

Após cada decisão, o resultado do D20 permanece visível no evento seguinte e só muda quando outra opção é escolhida. Alertas e cenas aguardam a interação do jogador antes de avançar.

## Objetivo e eleições
- Para vencer, reduza a zero os quatro pilares: agronegócio, economia, segurança e saúde.
- As eleições acontecem a cada 30 turnos. Sobreviva à votação para continuar a campanha; a eleição não substitui o objetivo dos quatro pilares.

## Novidades da v1.0

### Ministros com personalidade
- Cada ministro apresenta temperamento, agenda política e lealdade.
- O botão **OUVIR** abre espaço para negociação e pode recuperar lealdade ou apoio institucional.
- Demissões continuam possíveis, com risco de vazamentos e retaliação política.

### Protestos e revoltas
- Tensão nas ruas, adesão aos protestos e risco de revolta evoluem a cada turno.
- Diálogo com manifestantes reduz a temperatura social.
- A contenção pode aliviar a situação no curto prazo, mas aumentar a revolta e o desgaste institucional.
- Cutscene própria quando os protestos se tornam uma crise nacional.

### Forças armadas e risco de golpe
- Lealdade institucional, insatisfação militar e risco de golpe são indicadores independentes.
- Reuniões com o alto comando e reformas transparentes reduzem a tensão.
- Crises simultâneas podem levar a uma ruptura institucional e a um final específico.

### Mercado paralelo
- O câmbio paralelo acompanha dólar, inflação, escassez e capacidade de fiscalização.
- Fiscalizações podem aumentar o controle estatal, mas agravar temporariamente a escassez.
- Abastecimento emergencial reduz a escassez e ajuda a recuperar apoio popular.
- Cutscene de colapso do abastecimento e mercado paralelo.

### Mapa vivo das cidades
- Sete distritos têm indicadores próprios de tensão e qualidade dos serviços.
- O mapa muda a cada turno conforme inflação, protestos, serviços e situação dos pilares.
- Os sete distritos são exibidos em uma grade alinhada e responsiva.
- Selecione um distrito para ver sua situação e a região correspondente.

### Cutscenes de crises e finais
- Novas cenas animadas para protestos nacionais, ruptura institucional e colapso do abastecimento.
- Finais específicos para revolta popular e golpe de Estado.
- Cutscenes anteriores, cenas dos quatro pilares e finais existentes foram preservados.

## Sistemas preservados da v0.9.4
- Quatro pilares, D20, eventos e decisões com consequências.
- Ministros, noticiário dinâmico, inflação, preços e painel macroeconômico.
- Investigações lentas, níveis de investigação e até dois arquivamentos por campanha; a terceira tentativa convoca votação de impeachment.
- CPI, vazamentos, eleições, fake news, articulação política e pressão judicial.
- Desastres naturais, exploração de cinco regiões, aprovação regional e operações de segurança.
- Música e efeitos sonoros com ativação manual.
- Cutscenes animadas existentes e salvamento automático.

## Compatibilidade de saves
Ao iniciar ou continuar, os campos novos são adicionados automaticamente. Saves v0.9.x são mantidos e migrados; a campanha também grava uma cópia no novo espaço `desgoverno_v10_save`.

## Observações
- O jogo é fictício e funciona localmente no navegador.
- Para começar do zero, use **Reiniciar Campanha**.


## v1.7 — Remoção da mecânica de dissolução dos estados
- Removida a opção de dissolver ou extinguir estados e o painel correspondente.
- Removido o aumento automático de revoltas estaduais a cada escolha. Os indicadores gerais de protestos e tensão social continuam no jogo.
- As escolhas avançam o turno automaticamente depois que alertas e cenas forem fechados.
- Removido o limite fixo de quatro turnos; a campanha continua até um dos finais causados pelas condições do jogo.

## v1.2 — Alertas de movimentação
- Os painéis **Rua em Chamas**, **Alto Comando** e **Mercado Paralelo** abrem alertas pop-up quando um dos indicadores relacionados varia pelo menos 8 pontos percentuais (o câmbio paralelo usa variação relativa de 8%).
- O alerta apresenta os indicadores que mudaram e oferece ações rápidas relacionadas ao tema.
- Os alertas são verificados após decisões, ações dos painéis e atualização de turno.


## v1.3 — Gabinete limitado
- O gabinete passa a ter exatamente cinco ministérios ativos por campanha.
- Saves anteriores são ajustados automaticamente: ministros excedentes são removidos e vagas são preenchidas com os ministérios disponíveis.
- Demitir um ministro substitui o cargo, sem aumentar o total acima de cinco.
- O painel mostra a contagem atual de ministérios (ex.: 5/5).
- Os botões **OUVIR** e **DEM.** ficam agrupados na mesma linha; a troca de ministro mantém o gabinete em cinco cargos.


## v1.4 — Trilha sonora original
- Música ambiente original gerada em tempo real pela Web Audio API, sem arquivos externos ou músicas protegidas por direitos autorais.
- Trilha eletrônica cinematográfica em tom menor, com baixo pulsante, bateria sintetizada, acordes atmosféricos e melodia em loop.
- O botão `SOM: ON/OFF` controla a música; por padrão ela só começa após o jogador ativar o som, respeitando as restrições de reprodução automática dos navegadores.


## v1.5 — Legibilidade e correções políticas
- Painéis **Rua em Chamas** e **Articulação Política** ganharam destaque visual, melhor contraste e tipografia maior.
- No desktop, esses dois painéis ocupam mais largura; os indicadores e botões ficam mais fáceis de localizar.
- A cutscene de protestos nacionais foi corrigida: o desenho da multidão e das cenas de crise não depende mais de variáveis inexistentes.
- Alertas de movimentação que coincidirem com outra cutscene ficam aguardando o fechamento do evento, em vez de desaparecer. O jogador pode avançar o turno manualmente depois de fechar o alerta.
- Ações de rua e articulação política indicam quando o Tesouro não tem saldo suficiente; botões sem recursos ficam desabilitados.
- Ações políticas exibem uma mensagem de confirmação após a execução.


## v1.6 — botão de demissão do gabinete
- O controle abreviado “DEM.” agora recebe um ícone de lixeira, cor de alerta e dica acessível para identificar claramente a ação de demitir um ministro.
- O botão mantém a mesma função de demissão e substituição, respeitando o limite de cinco ministérios.


## v1.9 — correções de mapa, articulação e ministérios
- Mapa urbano reorganizado em formato espacial de distritos, com seleção persistente, status, tensão e nível de serviços por bairro.
- Painéis laterais agora podem ser percorridos sem cortar o mapa ou as ações políticas em telas desktop.
- Articulação política apresenta feedback específico por medida e mantém bloqueio de ações sem saldo suficiente.
- Gabinete normaliza saves antigos para até cinco ministérios, evita cargos duplicados e repõe o ministro demitido em uma pasta disponível.
- Corrigido contador visual de turnos para não exibir limite fixo de quatro turnos.
