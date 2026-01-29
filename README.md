# Projeto: Análise de Evasão – Telecom X

Este repositório contém uma análise exploratória de dados (EDA) detalhada sobre o cancelamento de serviços (*churn*) na empresa fictícia Telecom X. O objetivo principal é identificar padrões comportamentais e financeiros que influenciam a decisão do cliente em deixar a empresa.

## Sobre o Projeto

A evasão de clientes é um dos maiores desafios do setor de telecomunicações. Reter um cliente atual é significativamente mais barato do que adquirir um novo. Este projeto utiliza técnicas de ciência de dados para extrair, tratar e visualizar informações estratégicas que auxiliam na retenção.

## Tecnologias e Ferramentas

O projeto foi desenvolvido em **Python** utilizando o ambiente Jupyter Notebook. As principais bibliotecas utilizadas foram:

- **Pandas & NumPy**: Manipulação e limpeza de dados.
- **Requests & JSON**: Extração e normalização de dados brutos de fontes externas.
- **Matplotlib & Seaborn**: Visualização de dados e análise estatística.

## Etapas da Análise

1.  **Extração de Dados**: Recuperação de dados estruturados em formato JSON via API.
2.  **Tratamento e Limpeza**:
    - Normalização de colunas aninhadas.
    - Imputação de valores nulos (utilizando a moda para a coluna alvo).
    - Conversão de tipos de dados (ex: `TotalCharges` para numérico).
3.  **Análise Exploratória (EDA)**:
    - Verificação da distribuição de churn.
    - Análise de correlação entre tipo de contrato e cancelamento.
    - Estudo do impacto das cobranças diárias e mensais.
4.  **Engenharia de Features**: Criação de métricas como o custo diário dos serviços para melhor comparação entre perfis.

## Principais Insights

- **Contratos Mensais**: Apresentam a maior taxa de churn, sugerindo que a falta de fidelização contratual facilita a saída.
- **Custos Diários**: Clientes que cancelam o serviço tendem a ter uma média de custo diário superior à dos clientes retidos.
- **Serviço de Fibra Óptica**: Identificado como um ponto de atenção devido ao alto custo percebido.

## Recomendações Estratégicas

- **Migração de Pagamento e Redução de Fricção:** O alto churn no "Cheque Eletrônico" sugere fricção mensal na decisão de pagamento. Devemos implementar uma estratégia "Digital-First", incentivando a migração para débito automático com benefícios exclusivos.
- **Investigação Técnica da Fibra Óptica:** Auditoria imediata na infraestrutura de fibra e na qualidade do suporte técnico. O cliente está pagando pelo serviço top-tier e não está vendo valor proporcional.
- **Incentivos de Conversão de Contrato:** Programas de benefícios para conversão de planos mensais para anuais nos primeiros 6 meses — o período de maior vulnerabilidade identificado.
- **Foco no Segmento Senior:** Desenvolver canais de atendimento e interfaces adaptadas para os 16% da base idosa, visando mitigar a correlação de 0,15 identificada entre este grupo e a evasão.
