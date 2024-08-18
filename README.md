# Monitoramento com Prometheus e Grafana

Este repositório contém uma configuração Docker Compose para implementar Prometheus e Grafana com o objetivo de monitorar o sistema e os containers Docker.

O setup foi criado para facilitar a visualização e análise das métricas do servidor e dos containers em execução, utilizando Prometheus para a coleta de dados e Grafana para a criação de dashboards interativos.

#### Atenção
Quando o Prometheus é configurado para exigir autenticação básica, ele compara a senha fornecida pelo usuário com o hash armazenado no web.yml. Se eles corresponderem, o acesso é concedido.
Isso impede que usuários não autorizados acessem o Prometheus e visualizem ou manipulem dados sensíveis.


- Acesse o Gerador de Hash Bcrypt e coloque sua senha
- Adicione sua hash no arquivo [web.yml](web.yml)
- Adicione a senha normal no arquivo [prometheus.yml](prometheus.yml)
