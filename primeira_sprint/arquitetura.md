Quais são as camadas da plataforma EV ChargeOps: física (carregador), conectividade (rede e protocolos), 
aplicação (back-end, regras de negócio e IA) e apresentação (interfaces do gestor e do usuário);


**8. Arquitetura da Plataforma EV ChargeOps**

**Camada Física**

Equipamentos:

- GoodWe HCA G2;
- medidores;
- infraestrutura elétrica.

**Camada de Conectividade**

Protocolos:

- Modbus;
- TCP/IP;
- HTTPS;
- MQTT;
- APIs REST.

**Camada de Aplicação**

Componentes:

- motor de faturamento;
- regras de negócio;
- IA;
- banco de dados;
- integração ERP.

**Camada de Apresentação**

Interfaces:

**Gestor**
- dashboard;
- relatórios;
- faturamento.

**Usuário**
- histórico;
- sessões;
- pagamentos.
___
Como os dados fluem da sessão de recarga até a fatura do usuário: qual é o caminho completo, 
quais transformações ocorrem e onde a IA entra nesse fluxo;

**9. Fluxo Completo dos Dados**

Etapa 1: Usuário autentica.


Etapa 2: Carregador inicia sessão.


Etapa 3: Telemetria é enviada.


Etapa 4: Back-end registra dados.


Etapa 5: IA analisa comportamento.


Etapa 6: Motor de faturamento processa consumo.


Etapa 7: Fatura individual é gerada.


Etapa 8

Usuário visualiza cobrança.

**10. Papel da Inteligência Artificial**

A IA atua em:

**Detecção de Anomalias**

Exemplos:

- sessões muito longas;
- consumo incompatível;
- falhas recorrentes.
- Previsão de Demanda

Permite:

- planejamento energético;
- expansão da infraestrutura.

**Previsão de Demanda**

Permite:

- planejamento energético;
- expansão da infraestrutura.

**Classificação de Usuários**

Perfis:

- residencial;
- corporativo;
- visitante.

**Otimização de Rateio**

- Validação automática das cobranças.
___

Qual é o modelo de rateio que a equipe propõe: quais variáveis serão usadas, 
como a fatura individual será calculada e como o modelo lida com casos excepcionais (sessão interrompida, 
usuário que não carregou no mês ou dois veículos da mesma unidade)

**11. Modelo de Rateio Proposto**

Variáveis

**Consumo**

kWh consumidos

**Taxa Operacional**

Manutenção

**Taxa Administrativa**

Custos da plataforma

Fatura =
(kWh × tarifa)
+
taxa operacional
+
taxa administrativa

**Casos Excepcionais**

**Sessão interrompida**

Cobrança proporcional.

**Usuário sem recarga**

Valor zero.

**Dois veículos mesma unidade:**

Consumo total =
Veículo A + Veículo B

ou

Cobrança individual por veículo.

___
Opção C — Esquema da base de dados: defina e documente o esquema de dados da plataforma, como entidades (usuário, unidade, sessão e fatura), atributos, relacionamentos e exemplos de registros simulados que serão usados na sprint 02.

[Esquema Base de Dados](/primeira_sprint/design/schema.md)