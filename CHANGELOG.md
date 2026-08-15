# Changelog

Todas as mudanças relevantes do Mechanic Tool — by KitoSoft serão registradas neste arquivo.

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
