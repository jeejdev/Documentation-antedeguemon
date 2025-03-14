# **Documentação do Projeto - Automação e Extração de Informações em Atendimento Inteligente**

## **1. Objetivo do Projeto**

O objetivo deste projeto é desenvolver uma solução capaz de **automatizar a extração de informações relevantes a partir de interações textuais** em sistemas de atendimento automatizado. O sistema utilizará técnicas de **Processamento de Linguagem Natural (PLN)** para **extrair, classificar e sumarizar** dados de grandes volumes de interações, permitindo a geração de insights estratégicos para otimização do atendimento ao cliente. Além disso, a aplicação fornecerá uma interface intuitiva para facilitar a navegação e a interpretação dos dados extraídos.

---

## **2. Descrição da Problemática**

Empresas que utilizam sistemas de atendimento automatizado, como **chatbots, assistentes virtuais e CRMs**, geram **grandes volumes de dados textuais** a partir das interações entre clientes e sistemas de inteligência artificial. No entanto, transformar essa grande massa de informações em **insights estratégicos úteis** continua sendo um desafio. 

Os principais problemas enfrentados são:

- **Dificuldade na extração de dados relevantes**: Muitas empresas possuem registros extensos de interações, mas não conseguem filtrar e extrair as informações realmente úteis.
- **Falta de uma sumarização eficiente**: A análise manual das interações demanda tempo e esforço, tornando difícil a identificação de padrões e tendências.
- **Classificação inconsistente de atendimentos**: Categorizar automaticamente as interações pode ajudar na priorização de chamados e na melhoria do atendimento.
- **Falta de uma interface intuitiva para análise de dados**: Ferramentas eficazes de visualização são fundamentais para que os insights possam ser interpretados rapidamente.

Com base nesses desafios, este projeto visa **criar uma plataforma inteligente que possibilite a extração automática dos principais pontos das conversas, classifique os atendimentos e gere insights diários**, melhorando a eficiência operacional das empresas.

---

## **3. Equipe do Projeto**

A equipe responsável pelo desenvolvimento do projeto é composta pelos seguintes membros:

| Nome                                  | Função        |
|---------------------------------------|--------------|
| Miguel Carvalho Soares               | Product Owner (PO) |
| Thiago Frederico da Silva Zani       | Dev Team     |
| Jean Lucas de Faria Silva            | Dev Team     |
| Gabriel Brosig Briscese              | Dev Team     |
| Jonas Rafael Siqueira Ribeiro        | Dev Team     |
| Jonatas Mathias Dalló                | Scrum Master |

---

## **4. Product Backlog**

O Product Backlog contém todas as funcionalidades organizadas por prioridade, de acordo com o retorno de valor ao negócio.

### **Épicos**

1. **Mecanismo de Extração de Informações**
2. **Busca Semântica**
3. **Sumarização Automática de Interações**
4. **Classificação Automática de Atendimentos**
5. **Geração de Insights e Dashboards**
6. **Gestão de Usuários e Controle de Acesso**
7. **Escalabilidade e Performance**
8. **Segurança e Conformidade com LGPD/GDPR**
9. **Integrações com APIs Externas**

---

### **4.1. User Stories**

Cada User Story foi elaborada seguindo o formato:
**“Como <tipo de usuário>, quero <funcionalidade desejada> para <algum motivo que remeta valor para o negócio>.”**

#### **Mecanismo de Extração de Informações**
1. **Como Admin, quero que o sistema extraia automaticamente informações relevantes das interações para facilitar a análise de atendimento.**
   - Critérios de Aceitação:
     - A extração deve ser automática e baseada em regras de PLN.
     - O sistema deve permitir visualizar os dados extraídos de cada interação.
     - O sistema deve processar dados provenientes de arquivos CSV e API do Jira.

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

---

## **5. Sprint Backlog - Primeira Sprint**

### **Objetivo da Sprint:** Criar um **protótipo navegável no Figma** e iniciar a implementação de funcionalidades básicas de PLN, com foco na extração de dados de um CSV e pré-processamento de texto.

| Rank | Prioridade | User Story                                                                                                                 | Estimativa |
| ---- | ---------- | -------------------------------------------------------------------------------------------------------------------------- | ---------- |
| 1    | Alta       | Como Admin, quero acessar uma página de login para entrar no sistema. (Protótipo Navegável)                                | 3          |
| 2    | Alta       | Como Admin, quero cadastrar interações a partir de um arquivo CSV.                                                         | 5          |
| 3    | Média      | Como Admin, quero realizar buscas semânticas e visualizar os resultados extraídos.                                         | 8          |
| 4    | Média      | Como Admin, quero visualizar um dashboard com filtros de classificação e sumarização das interações. (Protótipo Navegável) | 5          |

### **Telas e Funcionalidades da Primeira Sprint:**

1. **Página de Login**
   - Criar um **protótipo navegável no Figma** para a tela de login.
   - **Resultado esperado:** Interface interativa que simula o login de usuários.

2. **Cadastro de Interação**
   - Criar um **protótipo navegável no Figma** para a tela de envio de arquivos CSV contendo interações.
   - **Resultado esperado:** Interface interativa que simula o processo de carregamento de dados.

3. **Busca e Exibição Semântica**
   - Criar um **protótipo navegável no Figma** para a busca semântica e exibição de resultados.
   - **Resultado esperado:** Interface interativa demonstrando a busca e a exibição de resultados relevantes.

4. **Dashboard**
   - Criar um **protótipo navegável no Figma** para o dashboard de classificações e sumarização.
   - Exibir métricas como número de dúvidas, reclamações e outros tipos de interação.
   - **Resultado esperado:** Interface interativa apresentando estatísticas básicas.

5. **Extração de Dados de um CSV e Pré-processamento de Texto (PLN)**
   - Implementar a funcionalidade de leitura de arquivos CSV.
   - Aplicar técnicas básicas de **pré-processamento de texto**, como remoção de stopwords, normalização e tokenização.
   - **Resultado esperado:** CSV carregado e texto processado para futuras análises semânticas.

Esta documentação foi elaborada para refletir os objetivos do projeto, os desafios enfrentados e as funcionalidades planejadas para as primeiras entregas. Se houver necessidade de ajustes ou mais detalhes, estamos à disposição!

