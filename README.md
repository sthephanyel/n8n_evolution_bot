# n8n_evolution_bot

## 📦 Ambiente Completo com Evolution API, N8N, Postgres e Redis

### Docker Compose para automação, integrações e comunicação via WhatsApp

Este repositório fornece uma stack completa baseada em Docker Compose, reunindo:

Evolution API – Integração de WhatsApp com múltiplas instâncias. <br/>
N8N – Automação de fluxos, bots, pipelines e integrações. <br/>
PostgreSQL – Banco de dados robusto para armazenamento das informações. <br/>
Redis – Cache de alta performance para filas e otimizações internas. <br/>

Tudo configurado para funcionar de forma integrada, simples e totalmente automatizada.
<br/>
<br/>

## 🔒 Observações importantes

- A imagem do Postgres foi fixada na versão 17, devido à mudança na estrutura de diretórios nas versões mais recentes. <br/>
- É recomendado configurar o .env para guardar tokens e chaves sensíveis. <br/>
- A Evolution API requer configuração adicional dentro do painel para iniciar instâncias de WhatsApp. <br/>

## 🚀 Comandos Importantes
### 1️⃣ Subir todos os serviços
> docker compose up -d

### 2️⃣ Ver logs
> docker logs -f n8n <br/>
> docker logs -f evolution_api

### 3️⃣ Parar tudo
> docker compose down

### 4️⃣ Subir novamente recriando contêineres
> docker compose up -d --force-recreate
