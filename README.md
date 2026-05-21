# **🧪 EasyPark \- Quality Assurance (QA) & Testing**

Bem-vindo ao repositório oficial de Quality Assurance do projeto **EasyPark**. 
Este repositório contém a documentação, os roteiros e as evidências das validações de qualidade de software (Testes Manuais e Automatizados) aplicadas ao nosso ecossistema Mobile e Backend.

---

## **📌 Entregáveis da Sprint (Links Oficiais)**

| Recurso | Plataforma | Link de Acesso |
| :--- | :--- | :--- |
| **Testes Manuais** | Azure Boards | [https://dev.azure.com/kgb-easypark/Easypark/_testPlans/define?planId=56&suiteId=57] |
| **Testes Automatizados** | YouTube | [https://youtu.be/JkzRpz71zGM] |

---

## **📋 Parte A: Plano de Testes Manuais (Nível de Sistema)**

Para garantir a qualidade da Interface do Usuário (UI) e a usabilidade do motorista, elaboramos **4 Casos de Teste (Test Cases)** diretamente integrados ao nosso Backlog no **Azure Boards**, garantindo 100% de rastreabilidade com as *User Stories* entregues.

Os testes foram executados com **dados controlados** (inputs predefinidos) e cobrem as funcionalidades críticas do aplicativo:
1. **[CT01]** Busca de Vagas por Destino em Raio Definido (TanStack Query / Azure API).
2. **[CT02]** Seleção de Vaga e Interatividade do Bottom-Sheet no Mapa.
3. **[CT03]** Fluxo de Checkout e Confirmação de Pagamento com Timer Regressivo.
4. **[CT04]** Acesso e Consulta ao Histórico de Reservas Paginado.

---

## **🤖 Parte B: Testes Automatizados (API / Backend)**

Para garantir a integridade da base da nossa pirâmide de testes, utilizamos o **Postman** para automatizar a validação do nosso endpoint RESTful principal hospedado na Microsoft Azure (`/estacionamentos`).

Foram desenvolvidos **4 scripts de automação (JavaScript)** acionados via Post-response no Postman, que validam instantaneamente:
* **CT01 (Disponibilidade):** Validação de Status Code HTTP 200 (Success).
* **CT02 (Performance):** Validação de latência e tempo de resposta inferior a 1500ms.
* **CT03 (Contrato/Estrutura):** Validação da presença do array principal (`content`) no JSON de resposta.
* **CT04 (Regra de Negócio):** Validação da existência de campos críticos e obrigatórios para o mapa do App Mobile (Nome, Latitude e Longitude).

Uma demonstração em vídeo da configuração, execução e aprovação (PASS) desses scripts no Postman foi gravada e anexada na tabela de links acima.

---

## **✨ Criadores**

* [@gabrielCZz](https://github.com/orgs/kgb-fiap/people/gabrielCZz) - Gabriel Cruz | RM 569613
* [@k-auaferreira](https://github.com/orgs/kgb-fiap/people/k-auaferreira) - Kauã Ferreira | 560992
* [@Vi-debu](https://github.com/orgs/kgb-fiap/people/Vi-debu) - Vinicius Bitú | RM 560227