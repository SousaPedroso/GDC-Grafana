# Projeto Final - Gerenciamento de Configurações @ UFMT/2025

- Tecnologia: [Grafana](https://grafana.com/)
- Tecnologias aplicadas: Windows home, grafana.
- Integrantes:
  - Gabriel de Sousa Gomes Pedroso
  - Paulo Cézar Menichini

## 1. Descrição da tecnologia

O Grafana é uma plataforma de observabilidade utilizada para visualizar e monitorar dados provenientes de diferentes fontes, como bancos de dados, logs e métricas de infraestrutura. Ele se destaca pela capacidade de criar dashboards interativos e personalizáveis, facilitando a análise de desempenho de sistemas e a tomada de decisões.

No monitoramento do Windows Server, o Grafana se integra a ferramentas como Prometheus, Telegraf, InfluxDB e Windows Exporter, permitindo a coleta e exibição de métricas essenciais, como uso de CPU, memória, disco, rede e eventos do sistema. Diferente das ferramentas nativas do Windows, como Performance Monitor (PerfMon) e Event Viewer, que exigem configurações complexas e não fornecem uma visão centralizada, o Grafana oferece uma abordagem unificada e em tempo real, além de suportar alertas automáticos para detecção proativa de falhas.

Com toda essa facilidade o Grafana auxilia equipes de DevOps e infraestrutura a otimizar o desempenho dos servidores Windows, reduzindo o tempo de resposta a incidentes e melhorando a previsibilidade da operação.

## 2. Descrição do problema

O monitoramento eficaz da infraestrutura é um dos desafios enfrentados por equipes de DevOps, especialmente em ambientes baseados em Windows Server. Embora o sistema operacional ofereça ferramentas nativas, como PerfMon, Event Viewer e Task Manager, essas soluções possuem limitações que dificultam a obtenção de uma visão abrangente do desempenho do servidor, impactando diretamente a capacidade de identificar e responder a incidentes de forma ágil.

Alguns dos principais desafios enfrentados incluem:
• Falta de centralização: As ferramentas nativas do Windows Server não oferecem uma visão consolidada dos dados, obrigando as equipes a acessar múltiplas interfaces para obter métricas de desempenho.
• Dificuldade na análise de tendências: PerfMon e Event Viewer registram eventos e métricas, mas não fornecem uma forma intuitiva de identificar padrões ao longo do tempo.
• Ausência de alertas eficientes: As soluções nativas não permitem configurar alertas dinâmicos e personalizados para notificações em tempo real sobre possíveis falhas.
• Escalabilidade limitada: Em ambientes distribuídos, monitorar múltiplos servidores Windows exige configurações adicionais, tornando o processo trabalhoso e propenso a erros.

## 3. Solução

Utilização do grafana para acompanhamento de indicadores da máquina. Aqui para simulação, estamos utilizando uma licença gratuita do windows server. Para isso, configuramos os exportadores definidos na página [all in one do grafana](https://grafana.com/grafana/dashboards/21674-all-in-one/); em especíifico o windows exporter do prometheus, e o currency exporter; repositório do github que acompanha várias trocas de moeda; isso para simular o monitoramento dos indicadores da máquina e uma aplicação (visualmente seu funcionamento).

Após as configurações, importamos a configuração do grafana que agrupa as visualizações de estado necessárias. Nas imagens abaixo seguem~exemplos de funcionamento inicial e gradativo da monitoração.

![image](https://github.com/user-attachments/assets/9b49abf2-cc6d-48d5-990e-372bd2ad4430)


## 4. Referências

- [Laboratório grafana](https://grafana.com/grafana/dashboards/21674-all-in-one/)
- [Principais Ferramentas de Monitoramento do Windows Server para 2024](https://rds-tools.com/pt/top-windows-server-monitoring-tools/)
- [Solucionar problema de monitoramento](https://learn.microsoft.com/pt-br/windows-server-essentials/support/troubleshoot-computer-monitoring-in-windows-server-essentials)
