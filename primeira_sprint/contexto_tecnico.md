O que são infraestruturas de recarga compartilhada e quais são os principais desafios operacionais enfrentados por gestores de condomínios, 
edifícios corporativos ou campus universitários;

**1. Infraestruturas de Recarga Compartilhada**

**1.1 Conceito**

Uma infraestrutura compartilhada de recarga consiste em um ou mais carregadores elétricos utilizados por múltiplos usuários.

Exemplos:

- Condomínios residenciais;
- Edifícios corporativos;
- Universidades;
- Hospitais;
- Centros logísticos;
- Estacionamentos comerciais.

Ao contrário de um carregador residencial dedicado, a infraestrutura compartilhada exige mecanismos de controle de acesso, medição individual e cobrança.

**1.2 Principais Desafios Operacionais**

**Identificação do usuário**

O carregador precisa saber quem está utilizando a infraestrutura.

Métodos comuns:

- RFID;
- Aplicativo móvel;
- QR Code;
- Login corporativo.

**Rateio de energia**

Sem medição individualizada, o custo acaba sendo distribuído entre todos os usuários, gerando distorções.

Exemplo:

- Usuário A carregou 400 kWh no mês;
- Usuário B carregou 20 kWh.

Sem controle adequado ambos podem pagar valores semelhantes.

**Controle de disponibilidade**

Problemas comuns:

- Veículos permanecem conectados após a carga;
- Filas de utilização;
- Reserva indevida de vagas.

**Gestão da demanda elétrica**

Múltiplos carregadores operando simultaneamente podem:

- ultrapassar limites contratados;
- provocar penalidades tarifárias;
- exigir gerenciamento dinâmico de carga.

**Transparência**

Moradores e usuários desejam visualizar:

- consumo;
- histórico;
- custos;
- relatórios.

____

Como funciona uma sessão de recarga do ponto de vista técnico: o que acontece entre o momento em que o veículo é conectado e o encerramento da sessão, 
quais dados são gerados e como podem ser capturados;

**2. Funcionamento Técnico de uma Sessão de Recarga**

**2.1 Início da Sessão**

Fluxo simplificado:

- Usuário conecta o veículo.
- Carregador detecta o cabo.
- Autenticação ocorre (RFID, aplicativo ou sistema externo).
- Sessão é autorizada.

**2.2 Negociação Elétrica**

O carregador e o veículo realizam comunicação conforme normas IEC 61851.

São definidos:

- corrente máxima;
- potência disponível;
- condições de segurança.

**2.3 Transferência de Energia**

Durante a sessão são coletados:

| Dado                 | Descrição   |
| -------------------- | ----------- |
| Timestamp            | Horário     |
| Potência instantânea | kW          |
| Corrente             | A           |
| Tensão               | V           |
| Energia acumulada    | kWh         |
| Estado do carregador | Operacional |
| Estado do veículo    | Carregando  |

**2.4 Encerramento**

A sessão termina quando:

- veículo desconecta;
- usuário encerra;
- limite é atingido;
- falha ocorre.

**2.5 Dados Gerados**

Cada sessão produz:

```json
{
  "session_id": "S0001",
  "user_id": "U015",
  "charger_id": "HCA-G2-01",
  "start_time": "2026-06-15T18:00:00",
  "end_time": "2026-06-15T20:15:00",
  "energy_kwh": 18.7,
  "duration_minutes": 135,
  "max_power_kw": 7.2
}
```
____

Quais modelos de negócio existem para recarga compartilhada no Brasil e no mundo: recarga gratuita, cobrança por kWh, cobrança por tempo, 
assinatura mensal ou rateio condominial.

**3. Modelos de Negócio para Recarga Compartilhada**

**3.1 Recarga Gratuita**

Utilizada em:

- empresas;
- hotéis;
- universidades.

Vantagem:

- benefício ao usuário.

Limitação:

- custo absorvido pelo operador.

**3.2 Cobrança por kWh**

Modelo mais justo.

Fórmula: Valor = kWh consumido × tarifa

**3.3 Cobrança por Tempo**

Utilizada quando legislação restringe comercialização de energia.

Exemplo:

- R$ 4,00/hora

**3.4 Assinatura Mensal**

Exemplo:

- Plano Básico = 100 kWh/mês

Benefícios:

- previsibilidade;
- receita recorrente.

**3.5 Rateio Condominial**

Muito comum no Brasil.

O consumo total é distribuído conforme regras definidas pelo condomínio.
____


Opção A — Análise de mercado: mapeie ao menos 3 soluções existentes que resolvem problemas similares ao EV ChargeOps. 
Para cada uma, destaque: o problema que resolve, as funcionalidades principais, o modelo de negócio e as limitações conhecidas. 
Referências: Zaptec, Wallbox Pulsar Plus, ChargePoint, Neocharge e Copel Telecom EV;

**4. Análise de Mercado**

**4.1 Zaptec**

[How our patented charging technology works](https://youtu.be/MWSXqysn7Eg?list=PLWSDRCFn68EiZUajzGZl0i09gHJgnz4Rr)

Problema Resolvido

Gestão de recarga residencial coletiva.

Funcionalidades
- balanceamento dinâmico;
- autenticação RFID;
- monitoramento remoto;
- cobrança individual.

Modelo

Hardware + SaaS.

Limitações
- foco europeu;
- integração limitada com sistemas locais.

**4.2 ChargePoint**

[How EV Charging with ChargePoint Works](https://youtu.be/bU5AuQFSpkY)

Problema Resolvido

Operação de redes públicas e privadas.

Funcionalidades
- faturamento;
- relatórios;
- gerenciamento remoto;
- API.

Modelo

Assinatura + hardware.

Limitações
- alto custo;
- foco em grandes operações.

**4.3 NeoCharge**

[Installation & How It Works](https://youtu.be/uvVJxRreawg)

Problema Resolvido

Compartilhamento de infraestrutura residencial.

Funcionalidades

- divisão inteligente de potência;
- controle de carga.

Modelo

Venda de equipamento.

Limitações
- pouca capacidade analítica;
- ausência de faturamento avançado.

**4.4 Wallbox Pulsar Plus**

[Pulsar Plus US](https://youtu.be/Cm2dF3ux73g)

Problema Resolvido

Recarga residencial inteligente.

Funcionalidades
- Wi-Fi;
- Bluetooth;
- aplicativo móvel.

Limitações
- não projetado para faturamento multiusuário.

**4.5 Copel Telecom EV**

Problema Resolvido

Gestão regional de infraestrutura pública.

Funcionalidades
- monitoramento;
- autenticação;
- gestão remota.

Limitações
- foco regional;
- menor flexibilidade para customização.