# KitoSoft Mechanic Tool

Ferramenta Windows leve para mecânicos em servidores **GTA RP / FiveM**.

O KitoSoft foi criado para reduzir Alt+Tab durante o atendimento: a calculadora pode ser controlada por atalhos globais, o total aparece em um overlay sobre o jogo e os turnos registram automaticamente tempo trabalhado e evolução de saldo.

## Recursos

- Calculadora rápida com até **9 itens/serviços** configuráveis.
- Atalhos globais editáveis para `+1` e `+5`, inclusive NumPad.
- Overlay sobre o jogo com total atual e tempo trabalhado.
- Posição e opacidade do overlay configuráveis.
- Controle de turno por saldo inicial e saldo final.
- Lucro por sessão e lucro por hora.
- Histórico de turnos editável e exportação CSV.
- Análises de hoje, últimos 7 dias e últimos 30 dias.
- Melhor data, melhor dia da semana e ranking estimado por faixa horária.
- Backup e restauração manual em ZIP.
- Minimização para a bandeja do Windows.
- Dados armazenados localmente no computador.
- Tela de apoio ao projeto via PIX.

## Download

As versões prontas para uso serão publicadas em **Releases** deste repositório.

Planejamento de distribuição:

- **Light** — menor, exige .NET 8 Desktop Runtime instalado.
- **Portable x64** — não exige instalação do .NET, porém o arquivo é maior.

## Como usar

1. Abra o KitoSoft.
2. Em **Configurações**, ajuste nomes, preços, itens ativos e atalhos.
3. Se desejar, ajuste posição e opacidade do overlay.
4. Em **Meu turno**, informe o dinheiro no banco e na mão ao iniciar.
5. Durante o jogo, use os atalhos da calculadora sem sair do FiveM.
6. Ao terminar, informe os valores finais do banco e da mão.
7. Consulte o lucro em **Histórico** e **Análises**.

### Atalhos reservados

- `Shift + 0` — zerar orçamento.
- `Ctrl + Shift + O` — mostrar/ocultar overlay.

Os atalhos dos itens são configuráveis pelo usuário.

## Como as análises funcionam

O lucro de cada sessão é calculado como:

```text
saldo final - saldo inicial
```

Sessões menores que 15 minutos continuam aparecendo no Histórico e contam nos totais de lucro, mas são ignoradas em métricas sensíveis à duração, como média por hora e ranking de horários.

O **ranking de horários é uma estimativa**. Como o programa não registra cada pagamento individual, o lucro de um turno é distribuído proporcionalmente pelo tempo trabalhado dentro de cada faixa horária.

## Privacidade e dados

O KitoSoft não exige conta, servidor ou banco de dados online.

Os dados ficam em:

```text
%LOCALAPPDATA%\KitoSoft\MechanicTool\data.json
```

O programa também mantém um arquivo local de recuperação.

## Desenvolvimento

Stack:

- .NET 8
- Windows Forms
- C#
- QRCoder para o QR Code PIX

### Executar pelo terminal

```powershell
dotnet restore
dotnet run --project src/CapitalValleyMechanicTool/CapitalValleyMechanicTool.csproj
```

### Build

```powershell
dotnet build src/CapitalValleyMechanicTool/CapitalValleyMechanicTool.csproj -c Release
```

## Apoie o projeto

O KitoSoft é gratuito. Se a ferramenta for útil, existe uma opção de apoio voluntário via PIX dentro do próprio aplicativo.

**Chave PIX:** `5ca81030-e0f6-4776-93be-ded515c14654`

O apoio não é obrigatório para usar o programa.

## Status

**Versão alvo da primeira release pública: 1.0.0**

A v1 está focada em estabilidade, cálculo rápido, turnos, histórico e análises. Novos recursos ficam para versões futuras depois de uso e feedback reais.
