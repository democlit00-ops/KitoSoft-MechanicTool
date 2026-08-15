# Mechanic Tool

**by KitoSoft**

Ferramenta leve para mecânicos em servidores **GTA RP / FiveM**, criada para reduzir Alt+Tab e facilitar cálculos, controle de turno, histórico e análise de ganhos.

## Download

Os arquivos oficiais são publicados somente em **Releases** deste repositório.

### Installer — recomendado

Baixe:

`MechanicTool-KitoSoft-Setup-v1.0.0.exe`

Instala o Mechanic Tool no Windows, cria os atalhos escolhidos durante a instalação e inclui o desinstalador.

### Portable

Baixe:

`MechanicTool-KitoSoft-Portable-v1.0.0.zip`

Extraia o ZIP para uma pasta e execute `Mechanic Tool.exe`. Não exige instalação.

> As duas versões são para Windows x64 e incluem o runtime necessário. Não é preciso instalar o .NET separadamente.

## Recursos

- Calculadora rápida com até **9 itens/serviços** configuráveis.
- Atalhos globais editáveis para adicionar `+1` ou `+5` sem sair do jogo.
- Suporte a combinações alternativas, inclusive teclas do NumPad.
- Overlay sobre o jogo com total do orçamento e tempo trabalhado.
- Posição do overlay ajustável por arrastar e soltar.
- Opacidade do overlay configurável.
- Controle de turno por saldo inicial e saldo final.
- Registro automático dos horários de início e término.
- Lucro por sessão e média por hora.
- Histórico de turnos com edição e exclusão.
- Exportação CSV.
- Análises de hoje, últimos 7 dias e últimos 30 dias.
- Melhor data, melhor dia da semana e ranking estimado por faixa horária.
- Backup e restauração manual.
- Minimização para a bandeja do Windows.
- Dados armazenados localmente no computador.

## Atalhos

Os atalhos dos itens podem ser alterados em **Configurações**.

Atalhos reservados:

- `Shift + 0` — zerar orçamento.
- `Ctrl + Shift + O` — mostrar/ocultar overlay.

## Controle de turno

Ao iniciar o turno, informe quanto possui no banco e em dinheiro na mão.

Ao finalizar, informe os valores finais.

O lucro da sessão é calculado como:

```text
saldo final - saldo inicial
```

Qualquer dinheiro que entrar ou sair durante o período naturalmente fará parte do resultado da sessão.

## Análises

Sessões menores que 15 minutos continuam aparecendo no Histórico e contam nos totais de lucro, mas ficam fora das métricas em que uma duração muito curta distorceria o resultado, como média por hora e ranking de horários.

O ranking de horários é **estimado**. Como o aplicativo não registra cada pagamento individual, o lucro de um turno é distribuído proporcionalmente pelo tempo trabalhado em cada faixa horária.

## Privacidade

O Mechanic Tool funciona localmente e não exige conta, login ou servidor próprio.

Os dados de uso ficam no computador do usuário. O programa não envia histórico de turnos para a KitoSoft.

## Windows SmartScreen

A versão 1.0.0 ainda não possui certificado comercial de assinatura de código. Por isso, em alguns computadores o Windows SmartScreen pode exibir um aviso de **editor desconhecido** ao abrir o instalador ou o executável pela primeira vez.

Baixe sempre os arquivos pela página oficial de Releases deste repositório.

## Apoie o projeto

O Mechanic Tool é gratuito. Se ele for útil no seu RP, você pode apoiar voluntariamente o desenvolvimento via PIX.

**PIX:** `5ca81030-e0f6-4776-93be-ded515c14654`

O aplicativo também possui a tela **Sobre / Apoie**, com QR Code e PIX Copia e Cola.

## Feedback e problemas

Encontrou um bug ou comportamento incorreto? Use a aba **Issues** deste repositório e descreva:

- o que aconteceu;
- o que você esperava que acontecesse;
- versão do Mechanic Tool;
- versão do Windows;
- passos para reproduzir o problema.

## Versão atual

**Mechanic Tool v1.0.0 — by KitoSoft**

Este repositório é usado para documentação, downloads oficiais e suporte. O código-fonte do aplicativo não é distribuído aqui.
