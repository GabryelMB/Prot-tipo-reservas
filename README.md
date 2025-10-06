# 📱 Plataforma de Reserva de Dispositivos

## 🧩 Descrição Geral

A **Plataforma de Reserva de Dispositivos** é um sistema desenvolvido para o controle, gestão e coleta de dados sobre o uso de iPads e Chromebooks por professores.

O objetivo é organizar as reservas, monitorar o uso dos dispositivos, e gerar relatórios de apoio à gestão pedagógica e tecnológica da instituição.

---

## 🎯 Objetivo Geral

Desenvolver uma plataforma que permita:

- A reserva e controle de dispositivos (iPads, Chromebooks);
- O gerenciamento do uso e disponibilidade dos equipamentos;
- A coleta de dados de utilização, incluindo justificativas e finalidades;
- A segmentação por grupos educacionais, como EFAI, EFAF e Infantil.

---

## ⚙️ Requisitos Funcionais

### 🗓️ Reserva de Dispositivos

Cada professor pode realizar suas próprias reservas.

**A reserva inclui:**
- Tipo de dispositivo: iPad, Chromebook ou ambos.
- Segmento/Ano/Turma (ex.: Year 1 A/D, Year 6 B).
- Sala/local de uso (ex.: Creative Lab, Sala de Música).
- Horário de início e término da reserva.
- Quantidade de dispositivos.
- Aplicativo ou uso pretendido (Google Classroom, Kahoot, YouTube, etc.).
- Campo opcional para observações.

### 💻 Controle de Equipamentos

- Inventário de dispositivos organizado por carrinhos e segmentos.
- Registro de onde cada dispositivo está alocado.
- Histórico de alocações e reservas.

### 🧠 Justificativa de Uso

- Cada reserva deve incluir o aplicativo ou finalidade de uso.
- O sistema armazena essas informações para análise posterior.

### 🏫 Gerenciamento de Segmentos

Organização dos dispositivos por segmento educacional:

- **EFAI**: Ensino Fundamental Anos Iniciais
- **EFAF**: Ensino Fundamental Anos Finais
- **Infantil**: Educação Infantil

Cada segmento possui carrinhos próprios de dispositivos.

### 📊 Relatórios e Análises

- Interface para geração de relatórios com filtros personalizados.
- Visualização em gráficos e tabelas.
- Exportação para formatos como PDF e Excel.
- Relatórios baseados no histórico de reservas e justificativas de uso.

---

## 🧱 Requisitos Não Funcionais

- Interface amigável e intuitiva para os professores.
- Garantia de integridade dos dados e segurança no acesso.
- Estrutura escalável para permitir a adição de novos dispositivos e carrinhos.
- Acesso restrito apenas a usuários autorizados.

---

## 👥 Atores do Sistema

| Ator | Descrição |
|------|-----------|
| **Professor** | Realiza reservas e informa justificativas de uso. |
| **Administrador** | Gerencia dispositivos, carrinhos, segmentos e relatórios. |
| **Sistema de Notificações** | Envia alertas sobre reservas, aprovações e possíveis problemas. |

---

## 🧾 Casos de Uso Principais

| Código | Caso de Uso | Ator | Descrição |
|--------|-------------|------|-----------|
| **UC1** | Fazer Reserva | Professor | Realiza a reserva informando dispositivo, segmento, sala, horário e finalidade. |
| **UC2** | Gerenciar Inventário | Administrador | Atualiza o cadastro de dispositivos, carrinhos e segmentos. |
| **UC3** | Visualizar Histórico | Administrador | Consulta reservas anteriores por professor, segmento ou carrinho. |
| **UC4** | Coletar Dados de Uso | Sistema | Registra justificativas de uso para análise posterior. |
| **UC5** | Gerar Relatórios | Administrador | Gera relatórios filtrados por período, segmento, dispositivo e uso. |

---

## 🧩 Entidades Principais (Modelo de Dados)

| Entidade | Atributos Principais |
|----------|---------------------|
| **Professor** | id, nome, e-mail, segmento |
| **Dispositivo** | id, tipo (iPad/Chromebook), estado, carrinho |
| **Carrinho** | id, segmento, quantidade_total, quantidade_disponível |
| **Reserva** | id, professor, dispositivo(s), data_inicio, data_fim, quantidade, aplicativo_uso, observações |
| **Segmento** | id, nome (EFAI, EFAF, Infantil) |
| **AplicativoUso** | id, nome |
| **Relatório** | id, tipo, parâmetros_filtro, data_geracao, conteúdo |

---

## 🚀 Tecnologias Sugeridas

- **Frontend**: HTML, CSS, JavaScript ou React
- **Backend**: Node.js (Express) ou Python (Flask/Django)
- **Banco de Dados**: MySQL / SQLite / Firebase
- **Relatórios**: Power BI, Chart.js, ou Google Charts
- **Controle de Versão**: Git & GitHub

---

## 🧠 Futuras Melhorias

- Sistema de autenticação e login para professores e administradores.
- Notificações automáticas por e-mail ou painel do sistema.
- Dashboard com indicadores de uso e manutenção.
- Integração direta com Power BI para análises avançadas.
- Módulo de manutenção preventiva e controle de status de dispositivos.

---

## 👨‍💻 Autor

**Gabryel Guimarães**  
Estudante de BICT - UFMA | Estagiário na área de inovação e tecnologia.

> *"Gerenciar dispositivos é garantir que a tecnologia esteja sempre pronta para o aprendizado."*

---


