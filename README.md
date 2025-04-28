# **Documentação do Projeto - Automação e Extração de Informações em Atendimento Inteligente**

## **Sumário**

- [1. Objetivo do Projeto](#1-objetivo-do-projeto)
- [2. Descrição da Problemática](#2-descrição-da-problemática)
- [3. Product Backlog](#3-product-backlog)
  - [3.1. User Stories](#31-user-stories)
- [4. Sprint Backlog - Primeira Sprint](#4-sprint-backlog---primeira-sprint)
     - [4.1. BurnDown da Sprint 1](#41-burndown-da-sprint-1)

- [5. Sprint Backlog - Segunda Sprint](#5-sprint-backlog---segunda-sprint)
     - [5.1. BurnDown da Sprint 1](#51-burndown-da-sprint-2)
- [7. Equipe do Projeto](#7-equipe-do-projeto)
- [8. Links dos Repositórios](#8-links-dos-repositórios)

## **1. Objetivo do Projeto**

O objetivo deste projeto é desenvolver uma solução capaz de **automatizar a extração de informações relevantes a partir de interações textuais** em sistemas de atendimento automatizado. O sistema utilizará técnicas de **Processamento de Linguagem Natural (PLN)** para **extrair, classificar e sumarizar** dados de grandes volumes de interações, permitindo a geração de insights estratégicos para otimização do atendimento ao cliente. Além disso, a aplicação fornecerá uma interface intuitiva para facilitar a navegação e a interpretação dos dados extraídos.

---

## **2. Descrição do Problema**

Empresas que utilizam sistemas de atendimento automatizado, como **chatbots, assistentes virtuais e CRMs**, geram **grandes volumes de dados textuais** a partir das interações entre clientes e sistemas de inteligência artificial. No entanto, transformar essa grande massa de informações em **insights estratégicos úteis** continua sendo um desafio.

Os principais problemas enfrentados são:

- **Dificuldade na extração de dados relevantes**: Muitas empresas possuem registros extensos de interações, mas não conseguem filtrar e extrair as informações realmente úteis.
- **Falta de uma sumarização eficiente**: A análise manual das interações demanda tempo e esforço, tornando difícil a identificação de padrões e tendências.
- **Classificação inconsistente de atendimentos**: Categorizar automaticamente as interações pode ajudar na priorização de chamados e na melhoria do atendimento.
- **Falta de uma interface intuitiva para análise de dados**: Ferramentas eficazes de visualização são fundamentais para que os insights possam ser interpretados rapidamente.

Com base nesses desafios, este projeto visa **criar uma plataforma inteligente que possibilite a extração automática dos principais pontos das conversas, classifique os atendimentos e gere insights diários**, melhorando a eficiência operacional das empresas.

---

## **3. Product Backlog**

O Product Backlog contém todas as funcionalidades organizadas por prioridade, de acordo com o retorno de valor ao negócio.

### **Épicos**

| Épico                                        | Prioridade | Sprint Relacionada             |
|----------------------------------------------|------------|--------------------------------|
| **Mecanismo de Extração de Informações**     | Alta       | Sprint 1, Sprint 2             |
| **Busca Semântica**                          | Alta       | Sprint 2, Sprint 3             |
| **Sumarização Automática de Interações**     | Média      | Sprint 2, Sprint 3             |
| **Classificação Automática de Atendimentos** | Média      | Sprint 3                       |
| **Geração de Insights e Dashboards**         | Alta       | Sprint 2, Sprint 3             |
| **Gestão de Usuários e Controle de Acesso**  | Alta       | Sprint 1, Sprint 2             |
| **Escalabilidade e Performance**             | Baixa      | Sprint 3                       |
| **Segurança e Conformidade com LGPD/GDPR**   | Média      | Sprint 3                       |
| **Integrações com APIs Externas**            | Alta       | Sprint 3                       |

---

### **3.1. User Stories**

Cada User Story foi elaborada seguindo o formato:  
**“Como <tipo de usuário>, quero <funcionalidade desejada> para <algum motivo que remeta valor para o negócio>.”**

#### **Mecanismo de Extração de Informações**

1. **Como Admin, quero que o sistema extraia automaticamente informações relevantes das interações para facilitar a análise de atendimento.**
   - Critérios de Aceitação:
     - A extração deve ser automática e baseada em regras de PLN.
     - O sistema deve permitir visualizar os dados extraídos de cada interação.
     - O sistema deve processar dados provenientes de arquivos CSV.

#### **Busca Semântica**

2. **Como Admin, quero configurar filtros na busca semântica para refinar os resultados exibidos.**
   - Critérios de Aceitação:
     - A busca deve permitir filtragem por palavras-chave e categorias.
     - Os resultados devem ser ordenados por relevância.
     - Deve haver integração com um banco de vetores (exemplo: Pinecone).

#### **Sumarização Automática de Interações**

3. **Como Admin, quero obter um resumo automático das interações para economizar tempo na análise dos atendimentos.**
   - Critérios de Aceitação:
     - A sumarização deve destacar os principais pontos da conversa.
     - O resultado deve ser acessível via API.
     - A solução deve utilizar modelos de PLN pré-treinados para otimização.

#### **Classificação Automática de Atendimentos**

4. **Como Admin, quero que o sistema classifique automaticamente os atendimentos para priorizar chamados e melhorar o atendimento.**
   - Critérios de Aceitação:
     - A classificação deve ser baseada em categorias predefinidas.
     - O sistema deve permitir ajustes nas categorias.

#### **Geração de Insights e Dashboards**

5. **Como Admin, quero visualizar insights e métricas em um dashboard para acompanhar a performance do atendimento.**
   - Critérios de Aceitação:
     - O dashboard deve exibir métricas como número de dúvidas, reclamações e outros tipos de interação.
     - Deve permitir filtros por data e categorias.

#### **Gestão de Usuários e Controle de Acesso**

6. **Como Admin, quero gerenciar usuários e definir permissões para garantir a segurança do sistema.**
   - Critérios de Aceitação:
     - O sistema deve permitir cadastro, edição e exclusão de usuários.
     - Deve haver controle de acesso baseado em papéis.

#### **Escalabilidade e Performance**

7. **Como Admin, quero que o sistema seja escalável e tenha boa performance para suportar grandes volumes de dados.**
   - Critérios de Aceitação:
     - O sistema deve ser capaz de processar grandes volumes de dados sem perda de performance.
     - Deve haver suporte para múltiplos usuários simultâneos.

---

## **4. Sprint Backlog - Primeira Sprint**

### **Objetivo da Sprint:**  
Criar um **protótipo navegável no Figma** e iniciar a implementação de funcionalidades básicas de PLN, com foco na extração de dados de um CSV e pré-processamento de texto

| Rank | Prioridade | User Story                                                                                                                 | Estimativa |
| ---- | ---------- | -------------------------------------------------------------------------------------------------------------------------- | ---------- |
| 1    | Alta       | Como Admin, quero acessar uma página de login para entrar no sistema. (Protótipo Navegável)                                | 3          |
| 2    | Alta       | Como Admin, quero cadastrar interações a partir de um arquivo CSV.                                                         | 5          |
| 3    | Média      | Como Admin, quero realizar buscas semânticas e visualizar os resultados extraídos.                                         | 8          |
| 4    | Média      | Como Admin, quero visualizar um dashboard com filtros de classificação e sumarização das interações. (Protótipo Navegável) | 5          |

### **4.1. BurnDown da Sprint 1**

![BurnDown da Sprint 1](/img/burndown_sprint1.png)

### **Telas e Funcionalidades da Primeira Sprint:**

1. **Página de Login**
   - Criar um **protótipo navegável no Figma** para a tela de login.
   - **Resultado esperado:** Interface interativa que simula o login de usuários.

2. **Cadastro de Interação**
   - Criar um **protótipo navegável no Figma** para a tela de envio de arquivos CSV contendo interações.
   - **Resultado esperado:** Interface interativa que simula o processo de carregamento de dados.

3. **Busca e Exibição Semântica**
   - Criar um **protótipo navegável no Figma** para a busca semântica e exibição de resultados.
   - **Resultado esperado:** Interface que mostra onde ficará disponível a busca semântica.

4. **Dashboard**
   - Criar um **protótipo navegável no Figma** para o dashboard de classificações e sumarização.
   - Exibir métricas como número de dúvidas, reclamações e outros tipos de interação.
   - **Resultado esperado:** Interface interativa apresentando estatísticas básicas.

5. **Extração de Dados de um CSV e Pré-processamento de Texto (PLN)**
   - Implementar a funcionalidade de leitura de arquivos CSV.
   - Aplicar técnicas básicas de **pré-processamento de texto**, como remoção de stopwords, normalização e tokenização.
   - **Resultado esperado:** CSV carregado e texto processado para futuras análises semânticas.

## **5. Sprint Backlog - Segunda Sprint**

### **Objetivo da Sprint:**  

Desenvolver funcionalidades adicionais no sistema, incluindo a implementação de mecanismos de busca semântica, sumarização automática de interações, e a criação de dashboards para visualização de dados.

| Rank | Prioridade | User Story                                                                                                                 | Estimativa |
| ---- | ---------- | -------------------------------------------------------------------------------------------------------------------------- | ---------- |
| 1    | Alta       | Como Admin, quero configurar filtros na busca semântica para refinar os resultados exibidos.                                | 8          |
| 2    | Alta       | Como Admin, quero obter um resumo automático das interações para economizar tempo na análise dos atendimentos.             | 8          |
| 3    | Alta       | Como Admin, quero visualizar insights e métricas em um dashboard para acompanhar a performance do atendimento.              | 13         |
| 4    | Média      | Como Admin, quero permitir a integração da busca semântica com um banco de vetores (ex. Pinecone) para otimizar a busca.    | 5          |
| 5    | Média      | Como Admin, quero integrar a sumarização automática ao sistema para gerar insights diários automaticamente.               | 10         |

### **5.1. BurnDown da Sprint 2**

![BurnDown da Sprint 2](/img/burndown_sprint2.png)

### **Telas e Funcionalidades da Segunda Sprint:**

1. **Busca Semântica**  
   - **Objetivo:** Permitir que o admin refine as buscas com semelhança semântica.  
   - **Resultado Esperado:** Funcionalidade para filtrar resultados de busca e integrá-los com o banco de vetores (ex. Pinecone).

2. **Sumarização Automática das Interações**  
   - **Objetivo:** Implementar a sumarização automática das interações para que o admin consiga identificar rapidamente os principais pontos de cada conversa.  
   - **Resultado Esperado:** A geração de resumos automáticos das conversas, acessíveis via API.

3. **Dashboard de Insights e Métricas**  
   - **Objetivo:** Criar um dashboard que mostre métricas.  
   - **Resultado Esperado:** Uma interface interativa com gráficos e métricas claras para análise de performance de atendimento.

4. **Integração da Sumarização Automática**  
   - **Objetivo:** Incorporar a sumarização automática de interações no sistema, gerando insights diários.  
   - **Resultado Esperado:** O sistema deve gerar relatórios diários automáticos que sumarizam as interações e apresentam informações úteis para a análise.

### **Critérios de Aceitação:**

- **Busca Semântica**: 
  - Filtros por palavra-chave e categoria funcionando corretamente.
  - Integração com o banco de vetores, com resultados relevantes e ordenados.
  
- **Sumarização Automática**: 
  - Resumos concisos e claros para cada interação.
  - A API deve ser capaz de acessar as sumarizações de forma eficiente.

- **Dashboard**: 
  - Métricas visíveis e filtráveis por diferentes parâmetros (data, tipo de interação).
  - Exibição de gráficos de fácil entendimento.

- **Integração da Busca Semântica e Sumarização**: 
  - Implementação de integração entre a busca semântica e a sumarização de interações, tornando a plataforma mais inteligente e dinâmica.



## **7. Equipe do Projeto**

|    Função     | Nome                           |                                                                                                                                                      LinkedIn & GitHub                                                                                                                                                      |
| :-----------: | :----------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   Dev Team     | Thiago Frederico da Silva Zani |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/thiago-zani-1b8503249/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/zani19)          |
| Dev Team  | Jean Lucas de Faria Silva      |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jeanlfs/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/jeejinf)          |
|   Dev Team    | Gabriel Brosig Briscese        |   [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/gabriel-brosig-briscese-344a5587/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Briscese)   |
|   Dev Team    | Jonas Rafael Siqueira Ribeiro      |                 [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jonasrsribeiro/) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/jonasrsribeiro)         |
|   Scrum Master  | Jonatas Mathias Dalló     |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/jonatas-mathias-147638206) [![GitHub Badge](https://img.shields.io/badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Jonatas-Dallo)          |
|   Product Owner   | Miguel Carvalho Soares     |         [![Linkedin Badge](https://img.shields.io/badge/Linkedin-blue?style=flat-square&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/miguel-carvalho-soares-722b161a3/) [![GitHub Badge](https://img.shields.io-badge/GitHub-111217?style=flat-square&logo=github&logoColor=white)](https://github.com/Miguel-C1)          |

## **8. Links dos Repositórios**

Aqui estão os links para os repositórios relacionados ao projeto:

- [Pré-processamento](https://github.com/AntedeguemonAPI/pre-processamento)
- [Banco de Dados](https://github.com/AntedeguemonAPI/banco-de-dados)
- [Processamento](https://github.com/AntedeguemonAPI/processamento)
- [Frontend](https://github.com/AntedeguemonAPI/frontend)
- [Controller de Usuários e Autenticação](https://github.com/AntedeguemonAPI/controller-usuarios-autenticao)
