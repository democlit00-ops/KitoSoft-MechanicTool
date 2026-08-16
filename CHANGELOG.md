# Changelog

Todas as mudanças relevantes do Mechanic Tool — by KitoSoft serão registradas neste arquivo.

## 1.0.2 - 2026-08-16

### Corrigido
- Corrigido o comportamento dos campos **Banco final do turno** e **Dinheiro final do turno** durante um turno aberto.
- O usuário agora pode alterar os valores finais várias vezes sem o campo restaurar o número anterior de forma intermitente.
- O **Lucro previsto** passa a ser recalculado imediatamente quando apenas um dos campos finais é informado e o outro permanece em zero.
- Os valores finais em edição permanecem disponíveis enquanto o turno continua aberto.

### Adicionado
- Verificação de novas versões pelo GitHub em segundo plano, sem bloquear o uso do aplicativo.
- Botão **Verificar atualizações** na tela **Sobre / Apoie**.
- Fluxo assistido de atualização: o usuário escolhe quando atualizar.
- Download do Installer oficial da Release mais recente.
- Validação do Installer por **SHA-256** antes da execução.
- Abertura automática do instalador após o download e a validação bem-sucedida.
- Tela de novidades/changelog exibida uma única vez após a atualização.
- Botão **Histórico de versões** para consultar as versões publicadas no GitHub.

### Atualização
- A v1.0.2 é a primeira versão com verificação de atualização integrada. Usuários da v1.0.1 precisam instalar a v1.0.2 manualmente; as versões seguintes poderão ser detectadas pelo próprio aplicativo.

## 1.0.1 - 2026-08-15

### Corrigido
- Correção da edição de atalhos globais: combinações válidas já utilizadas anteriormente, como `Shift + 7`, agora podem ser capturadas e configuradas novamente.
- Durante a captura de um novo atalho, os atalhos globais do próprio Mechanic Tool são suspensos temporariamente para evitar interferência.
- Mantidos como reservados apenas os atalhos críticos do aplicativo: `Shift + 0` para zerar a calculadora e `Ctrl + Shift + O` para mostrar ou ocultar o overlay.
- Melhorada a notificação ao minimizar para a bandeja.
- A notificação da bandeja agora identifica o aplicativo como **Mechanic Tool**, em vez de exibir apenas **KitoSoft**.
- O aviso de minimização é exibido somente uma vez por execução, evitando notificações repetitivas.

## 1.0.0 - 2026-08-15

### Adicionado
- Calculadora com até 9 itens/serviços configuráveis.
- Atalhos globais editáveis para +1 e +5.
- Suporte a teclas do NumPad.
- Overlay com total do orçamento e tempo trabalhado.
- Posição e opacidade configuráveis do overlay.
- Controle de início e fim de turno.
- Histórico de lucro por sessão e por hora.
- Análises de hoje, 7 dias, 30 dias, melhor data e melhor dia da semana.
- Ranking estimado de desempenho por faixa horária.
- Exportação CSV do histórico.
- Backup e restauração manual.
- Minimização para bandeja.
- Tela Sobre / Apoie com PIX fixo do projeto.
- Persistência local com arquivo de recuperação.

### Regras estatísticas
- Sessões curtas continuam no histórico e nos totais.
- Sessões menores que 15 minutos não entram na média/hora nem no ranking de horários.
- Turnos que atravessam a meia-noite têm lucro distribuído proporcionalmente entre os dias e faixas horárias.
