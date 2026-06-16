Resolução normativa ANEEL nº 1.000/2021: exploração comercial da recarga, comunicação prévia à distribuidora 
e exigência de protocolos abertos de comunicação para equipamentos não exclusivos de uso privado;

**5. Marco Regulatório Brasileiro**

**5.1 Resolução Normativa ANEEL nº 1.000/2021**

A resolução consolidou regras do setor elétrico.

Impactos:

- permite exploração comercial da recarga;
- exige comunicação prévia em determinados cenários;
- favorece interoperabilidade;
- incentiva uso de protocolos abertos.

Protocolos Abertos na Resolução Normativa ANEEL nº 1.000/2021

O ponto mais importante para o EV ChargeOps está no Artigo 552, que estabelece:

"Equipamentos de recarga que não sejam exclusivos para uso privado devem ser compatíveis com protocolos abertos de domínio público para comunicação e supervisão e controle remotos."

O operador não pode ficar preso a uma solução proprietária que impeça interoperabilidade.

Na prática, a estação de recarga deve ser capaz de ser integrada a sistemas externos de gerenciamento.

Isso evita cenários como:

- carregador funcionando apenas com aplicativo do fabricante;
- impossibilidade de troca de software de gestão;
- dependência exclusiva de um fornecedor;
- impossibilidade de auditoria dos dados de recarga.

**O que é considerado um protocolo aberto?**

| Característica        | Descrição                                        |
| --------------------- | ------------------------------------------------ |
| Especificação pública | Documentação disponível                          |
| Interoperabilidade    | Diferentes fabricantes podem implementar         |
| Não exclusivo         | Não depende de um único fornecedor               |
| Padronização          | Amplamente aceito pelo mercado                   |
| Integração externa    | Permite comunicação com plataformas de terceiros |

**Protocolos normalmente aceitos pelo mercado**

**OCPP (Open Charge Point Protocol)**
[OCPP Explained: The Easy Way to Improve EV Chargers](https://youtu.be/tMxew3AEnNQ)
[Protocolo OCPP para a gestão de recarga de veículos elétricos](https://youtu.be/gScckuf7sKU)
[What is OCPP? What is OCPP's relevance to Electric Vehicle Charging?](https://youtu.be/5G5DRQ6NtKU)

É o padrão dominante para carregadores inteligentes.

Permite:
- iniciar sessões;
- encerrar sessões;
- autenticar usuários;
- coletar medições;
- receber alarmes;
- atualizar firmware;
- controlar potência remotamente.

**Modbus**

[What is Modbus and How does it Work?](https://youtu.be/txi2p5_OjKU)

Muito utilizado em equipamentos industriais e energéticos.

Permite:

- leitura de registradores;
- potência;
- corrente;
- tensão;
- energia acumulada.

**MQTT**

[What Is MQTT and How It Works](https://youtu.be/EZAhu31jSUg)

Muito usado em IoT.

Permite:

telemetria em tempo real;
publicação de eventos;
integração com IA.

**REST API**

Protocolos HTTP modernos.

Permitem:

integração com aplicativos;
dashboards;
faturamento;
ERPs.

O GoodWe HCA G2 possui interface RS-485, o que normalmente está associado ao uso de Modbus RTU.

**5.2 Conformidade do EV ChargeOps**

A solução:

- Não comercializa energia diretamente.

- Realiza cobrança pelo serviço de recarga.

- Mantém rastreabilidade.

- Utiliza protocolos interoperáveis.

- Permite auditoria das sessões.

**5.3 Cenário Regulatório em São Paulo**

Aspectos relevantes:

- Código de Obras municipal pode exigir adequações elétricas.
- Normas do Corpo de Bombeiros influenciam instalações em garagens.
- ABNT NBR 17019 e normas correlatas orientam infraestrutura de recarga.
- Distribuidoras podem exigir estudos de carga em ampliações significativas.

O EV ChargeOps atua na camada de gestão, mantendo aderência ao marco regulatório vigente.

[NBR 17019 | A nova norma de CARROS ELÉTRICOS lançada em 2022 no Brasil](https://youtu.be/WUfbkcNtotY)
[Infraestrutura de pontos de recarga de veículos elétricos: normas, dimensionamento e estudo de caso.](https://youtu.be/gy3SadmBheQ)
___

Carregador GoodWe HCA G2: interfaces RS-485, LAN, Wi-Fi, Bluetooth e RFID — 
o que cada uma permite fazer e como podem ser utilizadas pela plataforma;

[GoodWe HCA G2 Series Unboxing and Installation](https://youtu.be/JR6R5bowyMQ)

**6. Carregador GoodWe HCA G2**
**6.1 Interfaces Disponíveis**
RS-485

Permite:

- Modbus RTU;
- integração industrial;
- telemetria local.

LAN

Permite:

- monitoramento IP;
- integração com servidores locais;
- comunicação contínua.

Wi-Fi

Permite:

- conectividade sem fio;
- atualização remota;
- envio de telemetria.

Bluetooth

Permite:

- configuração local;
- manutenção;
- provisionamento.

RFID

Permite:

- autenticação de usuários;
- rastreamento individual;
- associação de sessões.

___

API GoodWe (SEMS Portal): quais dados ela expõe sobre o carregador, como status, potência, energia entregue e eventos de sessão.
___

Opção A — Mapeamento regulatório completo: além da RN 1.000/2021, verifique se existem normas estaduais, municipais ou resoluções complementares da ANEEL que impactem a operação de carregadores compartilhados em São Paulo. Avalie se a solução proposta estaria em conformidade;

[Carregadores Elétricos em Condomínios.](https://youtu.be/UhLus4jtAVE)