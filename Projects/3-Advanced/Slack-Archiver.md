# Arquivador do Slack

**Nível:** 3-Avançado

O Slack é uma ferramenta na qual muitas equipes confiam para colaboração não apenas entre desenvolvedores, mas também entre desenvolvedores e seus usuários. É especialmente atraente para equipes de Software de Código Aberto (OSS) já que suporta um nível gratuito altamente funcional.

Um problema é que o nível gratuito é limitado a um máximo de 10K mensagens. Quando este limite é atingido, mensagens mais antigas tornam-se indisponíveis, pois são expurgadas. Isso é muito impactante para equipes e comunidades ativas do Slack, já que mensagens mais antigas frequentemente contêm uma grande quantidade de "conhecimento institucional" que é perdido quando o limite de mensagens é atingido.

O Arquivador do Slack busca remediar esta situação extraindo o histórico de canais específicos para um banco de dados ou arquivo. Mensagens podem ser extraídas até o limite máximo permitido de 50 mensagens por minuto para o método API `channels.history`. Nesta taxa (nível 4) 86,4K mensagens poderiam ser teoricamente recuperadas por dia.

Implementadores são alertados que mais pesquisa será necessária para determinar o melhor método de extração a usar antes de tentar qualquer desenvolvimento desta aplicação.

## Histórias de Usuário

-   [ ] Permitir que o usuário especifique os canais a serem arquivados. Isso inclui adicionar e remover canais da lista
-   [ ] Apenas os proprietários da Equipe do Slack devem ser autorizados a arquivar mensagens
-   [ ] Para cada canal a ser arquivado, extrair periodicamente mensagens começando da última mensagem recuperada na última extração e gravá-las em um banco de dados
-   [ ] Permitir que o usuário copie um canal extraído para um arquivo
-   [ ] O arquivamento deve ser um processo automático. Ao contrário de um 'bot do Slack, nenhuma intervenção manual deve ser necessária para iniciar ou parar uma operação de arquivamento

## Funcionalidades Bônus

-   [ ] Implementar uma API que permita a uma aplicação extrair mensagens arquivadas do banco de dados de arquivamento

## Links e Recursos Úteis

Detalhes da API do Slack podem ser encontrados [aqui](https://api.slack.com/).

## Projetos de Exemplo

Para um exemplo de uma aplicação de arquivamento comercial para Slack veja [Chronicle](https://chingu-prework.slack.com/apps/A47KWM6Q4-chronicle)