# 📊 Exemplos de Configuração para Grafana

Este repositório contém exemplos de configurações para o **Grafana**, incluindo dashboards, datasources, alertas e configurações YAML para provisionamento automático.

## 📂 Estrutura do Repositório

```
/
├── dashboards/           # Exemplos de dashboards (JSON)
│   ├── exemplo-dashboard.json
│   ├── logs-dashboard.json
│   ├── alerts-dashboard.json
│
├── datasources/          # Configurações de datasources (YAML)
│   ├── prometheus.yaml
│   ├── loki.yaml
│
├── alerts/               # Configurações de alertas (JSON/YAML)
│   ├── alerta-latencia.json
│   ├── alerta-cpu.yaml
│
├── provisioning/         # Provisionamento automático (YAML)
│   ├── dashboards.yaml
│   ├── datasources.yaml
│
├── README.md             # Este arquivo
```

## 🖥️ Como Usar

### 📌 Importar um Dashboard
1. Acesse o Grafana e clique em **Dashboards** → **Import**.
2. Faça upload de um arquivo JSON da pasta `dashboards/`.
3. Configure o datasource e finalize a importação.

### ⚙️ Provisionamento Automático
1. Copie os arquivos YAML da pasta `provisioning/` para o diretório de provisionamento do Grafana (`/etc/grafana/provisioning/` ou `/var/lib/grafana/provisioning/`).
2. Reinicie o Grafana para aplicar as configurações:
   ```sh
   systemctl restart grafana-server
   ```

### 🔔 Configurar Alertas
- Os alertas estão na pasta `alerts/`. Eles podem ser importados diretamente no painel de alertas do Grafana.

## 📜 Licença
Este repositório está sob a licença **MIT**. Sinta-se à vontade para usar e contribuir!

---

💡 **Sugestões e melhorias são bem-vindas!**

