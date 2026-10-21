# 🌱 EcoODS - Plataforma Comunitária de Gestão e Coleta Seletiva

> **Disciplina:** Projeto de Software — Experiência Prática IV  
> **Instituição:** Cruzeiro do Sul Virtual  
> **Estudante:** Diego Antunes da Costa  
> **RA:** 49720198  
> **Curso / Semestre:** Análise e Desenvolvimento de Sistemas — 2º Semestre  

---

## 📌 1. Visão Geral do Projeto

O **EcoODS** é uma solução de software desenvolvida para solucionar uma dor operacional crítica identificada na comunidade: o descarte incorreto de resíduos recicláveis por pequenos comerciantes e munícipes, agravado pela falta de canais diretos de comunicação e roteirização com cooperativas e catadores locais.

Alinhada diretamente ao **Objetivo de Desenvolvimento Sustentável (ODS) 12 da ONU — Consumo e Produção Responsáveis** (em especial às metas 12.5 de redução de resíduos por reciclagem e 12.8 de conscientização cidadã), a plataforma conecta os geradores de recicláveis às cooperativas de triagem, substituindo anotações manuais e gerando renda e dignidade para a comunidade atendida.

---

## 🚀 2. Funcionalidades do MVP (Produto Mínimo Viável)

- **Painel de Indicadores de Impacto em Tempo Real:**
  - Total de quilos de recicláveis recolhidos e triados.
  - Total de atendimentos e coletas realizadas.
  - Cálculo automático de emissões de $CO_2$ equivalente evitadas.
  - Quantidade de famílias/catadores beneficiados.
- **Módulo de Solicitação e Agendamento de Coletas:**
  - Formulário simplificado e responsivo com campos de material predominante (papelão, plástico, vidro, metal, eletrônicos), peso estimado, endereço e data de preferência.
- **Mapeamento de Pontos de Entrega Voluntária (PEVs):**
  - Catálogo de ecopontos com filtros por categoria de resíduo, endereços e horários de funcionamento.
- **Painel Operacional da Cooperativa (Triagem):**
  - Tabela dinâmica de triagem com atualização de status (*Pendente* ➔ *Em Trânsito* ➔ *Concluída*).
- **Módulo de Telemetria e Monitoramento Pós-Lançamento:**
  - Verificação de *Health Check*, medição contínua de latência (ms), integridade de armazenamento e console de logs de eventos em tempo real.

---

## 🛠️ 3. Tecnologias Utilizadas

- **Frontend:** HTML5 Semântico, Vanilla CSS3 (Design System com variáveis CSS, responsividade mobile-first e glassmorphism), JavaScript Moderno (ES6+).
- **Persistência de Dados:** *Web Storage API (LocalStorage)* para persistência local e garantia de funcionamento offline/demonstrativo sem quedas de infraestrutura.
- **Versionamento & Deploy:** Git, GitHub, e hospedagem pública via GitHub Pages / Vercel.
- **Monitoramento & Telemetria:** *Health Check* com captura de exceções `window.onerror`, simulação de heartbeat e compatibilidade com UptimeRobot.

---

## 🌐 4. Como Executar Localmente

1. Clone este repositório:
   ```bash
   git clone https://github.com/diego-antunes/projeto-ods.git
   cd projeto-ods
   ```

2. Abra o arquivo `index.html` diretamente em seu navegador web (Google Chrome, Firefox, Edge) ou utilize a extensão **Live Server** no VS Code.

---

## ☁️ 5. Publicação (Deploy) e Monitoramento

- **URL de Produção:** `https://diego-antunes.github.io/projeto-ods/` *(ou link Vercel)*
- **Monitoramento de Disponibilidade:**
  - Configurado via **UptimeRobot** monitorando a rota principal a cada 60 segundos com alerta para taxa de erro > 0%.
  - Console interno de telemetria acessível diretamente no painel inferior da aplicação.

---

## ⚖️ 6. Responsabilidade Ética e LGPD

O sistema foi concebido respeitando as diretrizes da **Lei Geral de Proteção de Dados (LGPD - Lei nº 13.709/2018)**:
- Coleta estrita dos dados necessários para a logística da coleta (nome de contato, telefone e endereço).
- Armazenamento em conformidade, sem comercialização ou compartilhamento indevido de dados com terceiros.
- Interface inclusiva com alto contraste e tipografia acessível.

---

## 📄 7. Licença

Este projeto é desenvolvido para fins acadêmicos e comunitários sob a licença [MIT](LICENSE).
