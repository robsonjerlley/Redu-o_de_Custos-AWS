# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS
Data: 21/08/2025
Empresa: Abstract Int LTDA.
Responsável: Robson Jerlley Dos Santos Ferreira

## 📝Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa Abstrac Int LTDA,
realizado por Robson Jerlley Dos Santos Ferreira. O objetivo do projetp foi elencar três serviços AWS,
com a finalidade de diminuição de custos de forma imediata.

## 📑 Descrição

O projeto de implemantação de ferramentas foi dividido em três estapas, cada uma focada em um serviço
AWS específicos. A seguir detalharemos objetivos, atividades e resultados esperados de cada fase do prjeto:

## 🚀 Stack Utilizada
| Serviço AWS           | Propósito                            | Economia Estimada |
|-----------------------|--------------------------------------|-------------------|
| Cost Explorer         | Gerar relatórios de custo e uso      |  –                |
| Compute Optimizer     | Rightsizing de instâncias e EBS      | 20% a 30%         |
| Lambda + EventBridge  | Desligamento automático de dev       | Até 40%           |


#Etapas de Implementação:

📌 Etapa 1: Diagnóstico de Custos com AWS Cost Explorer

## 🎯 Objetivo
  * Identificar padrões de consumo e principais fontes de gastos na conta AWS.

## 🛠️ Atividades

  * Habilitar AWS Cost Explorer na conta e configurar permissões mínimas.
  
  * Gerar relatórios mensais de custo e uso em CSV.
  
  * Analisar top 5 serviços com maior despesa e horários de pico de consumo.

## 📈 Resultados Esperados
  * Relatórios armazenados em bucket S3 que apontem imediatamente onde há desperdício.
 
📌 Etapa 2: Rightsizing com AWS Compute Optimizer

## 🎯 Objetivo
  * Ajustar capacidade de recursos sobredimensionados para reduzir custos sem impactar a performance.

## 🛠️ Atividades

  * Ativar AWS Compute Optimizer na região principal.
  
  * Coletar recomendações de redimensionamento para instâncias EC2, volumes EBS e funções Lambda.
  
  * Aplicar downsizing conforme orientação e validar testes de carga.
  
## 📈 Resultados Esperados
  * Economia de 20% a 30% na fatura de computação e armazenamento sem alteração perceptível de serviço.

📌 Etapa 3: Automação de Desligamento de Recursos com AWS Lambda

## 🎯 Objetivo
  * Desligar automaticamente recursos de desenvolvimento e homologação fora do horário de expediente.
    
## 🛠️ Atividades

  * Desenvolver função Lambda em Java para stop/start de instâncias EC2.
  
  * Configurar regra agendada no EventBridge para invocar a Lambda nos horários pré-definidos.
  
  * Monitorar execuções e logs no CloudWatch, ajustando janelas conforme necessidade.

## 📈 Resultados Esperados
  * Redução de até 40% no custo de execução de instâncias não críticas, com total visibilidade dos desligamentos.

## 🏁 Conclusão

A adoção dos três serviços AWS proporcionará:

* Visibilidade imediata dos gastos e oportunidades de otimização.

* Recomendações automatizadas de rightsizing aplicadas com segurança.

* Desligamento programado de recursos ociosos, garantindo economia contínua.

* Estima-se uma redução combinada de até 50% na fatura mensal de infraestrutura.

