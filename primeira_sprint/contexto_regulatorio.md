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

**Mapeamento Regulatório – Carregadores Compartilhados no Estado de São Paulo**

A análise regulatória indica que o EV ChargeOps está alinhado com a legislação atual, mas existem requisitos importantes que devem ser considerados na arquitetura e operação da plataforma.

**1. Nível Federal – ANEEL Resolução Normativa ANEEL nº 1.000/2021**

Continua sendo a principal norma do setor.

Os pontos mais relevantes para o EV ChargeOps são:

**Exploração comercial permitida**

A ANEEL permite que qualquer agente ofereça serviços de recarga, inclusive mediante cobrança. A atividade não é considerada distribuição de energia elétrica, mas prestação de serviço de recarga.

**Protocolos abertos**

Equipamentos de uso compartilhado devem permitir supervisão e controle remoto por protocolos abertos, evitando dependência tecnológica de um único fabricante.

**Comunicação com a distribuidora**

Dependendo da potência instalada e dos impactos na rede, a distribuidora local poderá exigir análise de carga e adequações técnicas.

**2. Estado de São Paulo Lei Estadual nº 18.403/2026**

A principal novidade regulatória recente.

A lei garante aos condôminos o direito de instalar carregadores em vagas privativas de condomínios residenciais e comerciais. O condomínio não pode proibir a instalação sem justificativa técnica formal.

**Requisitos obrigatórios**

A instalação deve observar:

- compatibilidade com a capacidade elétrica da edificação;
- normas da distribuidora;
- normas ABNT;
- execução por profissional habilitado;
- emissão de ART ou RRT;
- comunicação prévia à administração condominial.


A lei cria demanda direta por:

- identificação individual de usuários;
- medição individualizada;
- cobrança individual;
- gestão de múltiplos carregadores.

Esses são exatamente os problemas que o EV ChargeOps resolve.

**3. Município de São Paulo Lei Municipal nº 17.336/2020**

Aplica-se aos novos empreendimentos aprovados no Município de São Paulo.

Ela determina que projetos residenciais e comerciais prevejam infraestrutura para recarga de veículos elétricos.

Um aspecto particularmente relevante para o EV ChargeOps é que a legislação menciona a necessidade de:

- medição individualizada;
- cobrança individual do consumo associado à recarga.

A lei praticamente cria uma necessidade operacional para plataformas de gestão e faturamento.

**4. Normas Técnicas ABNT**

Embora não sejam leis, são obrigatórias na prática porque são referenciadas por:

- distribuidoras;
- Corpo de Bombeiros;
- projetos elétricos;
- ARTs e RRTs.

As mais relevantes incluem:

**ABNT NBR 17019**

Infraestrutura para recarga de veículos elétricos.

Define requisitos para:

- instalação;
- segurança;
- dimensionamento;
- proteção elétrica.

**IEC 61851 (adotada no Brasil)**

Define a comunicação entre:

- veículo;
- carregador.

**IEC 62196**

Define conectores e interfaces.

**5. Corpo de Bombeiros de São Paulo**

O Estado de São Paulo vem discutindo requisitos específicos para garagens com recarga de veículos elétricos.

Entre as exigências técnicas discutidas e parcialmente incorporadas em atualizações normativas estão:

- detecção de fumaça;
- detecção térmica;
- ventilação adequada;
- sistemas de combate a incêndio;
- sprinklers em novos empreendimentos.

Embora muitas dessas regras ainda dependam de regulamentações complementares e instruções técnicas específicas, a tendência regulatória é clara: aumentar os requisitos de segurança para instalações coletivas de recarga.

**6. Distribuidoras de Energia (Enel SP, EDP SP, CPFL)**

Além da ANEEL, cada distribuidora possui normas técnicas próprias.

Em projetos coletivos geralmente são exigidos:

- estudo de demanda;
- memorial de carga;
- adequação de transformadores;
- análise de impacto na rede interna.

A Lei Estadual 18.403/2026 reforça a necessidade de conformidade com as regras da distribuidora local.

___

Agência Nacional de Energia Elétrica (ANEEL)

ANEEL.
Resolução Normativa nº 1.000, de 7 de dezembro de 2021. Estabelece as Regras de Prestação do Serviço Público de Distribuição de Energia Elétrica.
Brasília: Agência Nacional de Energia Elétrica, 2021.

[ANEEL – Resolução Normativa nº 1.000/2021](https://www2.aneel.gov.br/cedoc/ren20211000.pdf?utm_source=chatgpt.com)

Agência Nacional de Energia Elétrica (Mobilidade Elétrica)

ANEEL.
Veículos Elétricos – Perguntas Frequentes e Regulamentação.
Brasília: Agência Nacional de Energia Elétrica.

[Portal ANEEL – Veículos Elétricos](https://www.gov.br/aneel/pt-br/assuntos/veiculos-eletricos?utm_source=chatgpt.com)

Estado de São Paulo

SÃO PAULO (Estado).
Lei nº 18.403, de 2026. Dispõe sobre a instalação de infraestrutura de recarga para veículos elétricos em condomínios residenciais e comerciais.

[Governo do Estado de São Paulo – Lei sobre carregadores em condomínios](https://www.agenciasp.sp.gov.br/governo-de-sp-sanciona-lei-que-permite-instalacao-de-carregadores-de-carros-eletricos-em-condominios/?utm_source=chatgpt.com)

Município de São Paulo

SÃO PAULO (Município).
Lei nº 17.336, de 30 de março de 2020. Dispõe sobre a instalação de infraestrutura para abastecimento de veículos movidos a energia elétrica em edificações.

[Lei Municipal nº 17.336/2020](https://legislacao.prefeitura.sp.gov.br/lei-17336-de-30-de-marco-de-2020)

Associação Brasileira de Normas Técnicas (ABNT)

ABNT.
ABNT NBR 17019: Infraestrutura para carregamento condutivo de veículos elétricos.
Rio de Janeiro: Associação Brasileira de Normas Técnicas.

Observação: norma técnica adquirida mediante licenciamento junto à ABNT.

[ABNT Oficial](https://abnt.org.br/?utm_source=chatgpt.com)

Comissão Eletrotécnica Internacional (IEC)

INTERNATIONAL ELECTROTECHNICAL COMMISSION (IEC).
IEC 61851 – Electric Vehicle Conductive Charging System.

Genebra: IEC.

[IEC 61851 Overview](https://webstore.iec.ch/en/publication/32973)

INTERNATIONAL ELECTROTECHNICAL COMMISSION (IEC).
IEC 62196 – Plugs, Socket-Outlets, Vehicle Connectors and Vehicle Inlets for Electric Vehicles.

[IEC Official Website](https://webstore.iec.ch/en/publication/110638)
