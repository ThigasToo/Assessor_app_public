# Daniel.AI

## 📌 Visão Geral

Este projeto nasce de um problema real:

> Pessoas comuns não têm acesso a aconselhamento financeiro de qualidade, em tempo real e sem conflitos de interesse.

Na prática:

* Familiares e amigos sem conta em corretoras ou assessores
* Falta de tempo para estudar investimentos
* Assessores com viés comercial (produtos que geram mais comissão)

## O Problema

O investidor comum enfrenta três grandes barreiras:

1. **Acesso limitado a informação qualificada**
2. **Falta de tempo para análise profunda**
3. **Conflito de interesse em assessorias tradicionais**

Isso resulta em decisões financeiras subótimas, baseadas em:

* Achismos
* Conteúdo superficial
* Recomendações enviesadas

---

## A Solução

Um **Consultor Financeiro Autônomo baseado em IA**, que atua de forma:

* 📊 **Data-driven**
* ⚡ **Em tempo real**
* 🧠 **Sem viés comercial**
* 🎯 **Personalizado por perfil de risco**

---

## Arquitetura do Sistema

O sistema foi projetado com uma abordagem moderna baseada em **microsserviços**, garantindo escalabilidade, performance e modularidade.

### Backend (Core API)

* **Framework:** FastAPI
* **Arquitetura:** REST API
* **Banco de Dados:** Supabase (PostgreSQL)

Responsável por:

* Orquestração de dados
* Persistência
* Integração com IA
* Exposição dos endpoints

---

### Pipeline de Ingestão de Dados

Rotinas automatizadas (Cron Jobs) responsáveis por alimentar o sistema com dados atualizados:

* Web scraping com Python (`requests`, `BeautifulSoup`)

* Coleta de dados públicos:

  * Taxa Selic
  * IPCA
  * CDI
  * Indicadores macroeconômicos

* Integração com APIs de Open Finance:

  * Tesouro Direto
  * CDBs
  * Fundos de investimento
  * Ações
  * Criptomoedas

> Atualização contínua para manter o sistema sempre alinhado com o mercado

---

### Motor de Inteligência (IA)

Diferencial central do projeto.

Ao invés de usar RAG tradicional, o sistema utiliza:

#### 📸 Contexto Curado Dinâmico

* Injeção diária de um **"Snapshot do Mercado"**, contendo:

  * Notícias relevantes
  * Taxas reais atualizadas
  * Dados de ativos financeiros

#### 🎯 Benefícios:

* Redução de alucinações da IA
* Respostas com dados reais e atuais
* Recomendações precisas

---

### Memória Persistente

Gerenciamento inteligente do usuário:

* Histórico de conversas
* Perfil de investidor:

  * Conservador
  * Moderado
  * Agressivo

📌 Armazenado no Supabase para continuidade entre sessões

---

### Interface de Voz

Pipeline de áudio com baixa latência:

* Integração com ElevenLabs
* Conversão para Base64
* Streaming eficiente para frontend (Flutter)

Resultado:

> Interação natural, como conversar com um assessor humano

---

## Resultado Final

Um sistema capaz de:

* Processar milhares de dados financeiros em segundos
* Reduzir horas de pesquisa para milissegundos
* Fornecer recomendações com:

  * Ativos reais
  * Instituições financeiras específicas
  * Taxas atualizadas

💡 Experiência do usuário:

> Um **"Bloomberg simplificado"**, acessível via conversa para qualquer pessoa

---

## Diferenciais

* ⚖️ **Sem conflito de interesse**
* 🧠 **IA com contexto atualizado diariamente**
* 🔄 **Dados em tempo real**
* 🗣️ **Interface conversacional com voz**
* 🎯 **Personalização por perfil de risco**

---

## Status do Projeto

Este repositório é uma **versão pública demonstrativa**.

O código completo do projeto é privado, mas esta documentação apresenta:

* Arquitetura
* Conceitos técnicos
* Abordagem de engenharia

---

## ⚠️ Disclaimer

Este sistema tem caráter informativo e educacional.
Não constitui recomendação formal de investimento.

---

## 🧠 Filosofia

> "Um sistema que elimina vieses humanos e transforma dados em decisões melhores."

---

## 📄 Licença

Este repositório é apenas demonstrativo.
Direitos reservados.
