## ESTRUTURA OBRIGATÓRIA DO FPSD

  

### 1. CABEÇALHO PADRÃO

```

# Functional Poc Start Up Document (FPSD)

## [Nome do Produto]

  

**Documento:** Especificação Funcional

**Proprietário:** [Nome] - [Cargo]

**Versão:** 1.0

**Data:** [Data atual]

**Status:** Em Desenvolvimento

```

  

### 2. SEÇÕES OBRIGATÓRIAS

  

#### 2.1 Visão Geral do Sistema

- Propósito técnico detalhado

- Escopo funcional específico

- Atores e suas interações

  

#### 2.3 Especificações Funcionais Detalhadas

Para cada requisito funcional (RF###):

- **Dados obrigatórios/opcionais**

- **Regras de negócio específicas**

- **Validações técnicas**

- **Integrações necessárias**

  

#### 2.5 Regras de Negócio Críticas

Numeradas (RN###) com:

- Condições específicas

- Ações resultantes

- Exceções e tratamentos

  

#### 2.6 Integrações Externas

- APIs de terceiros

- Webhooks necessários

- Formatos de dados


#### 2.7 Fluxos de Dados

- Diagramas em formato textual

- Estados dos dados

- Transformações necessárias

  

#### 2.8 Critérios de Aceite MVP

- Lista verificável

- Métricas quantificáveis

- Condições de sucesso

  

#### 2.9 Casos de Uso Detalhados

Format UC### com:

- Pré-condições

- Fluxo principal (passos numerados)

- Fluxos alternativos

- Pós-condições
  

## DIRETRIZES TÉCNICAS OBRIGATÓRIAS

### NÍVEL DE DETALHAMENTO

- **Dados**: Especificar tipos, tamanhos, validações

- **APIs**: Definir endpoints, métodos, payloads

- **Estados**: Mapear todos os status possíveis

- **Integrações**: Detalhar formatos e protocolos
  

### LINGUAGEM TÉCNICA

- Use terminologia precisa de engenharia de software

- Especifique algoritmos quando necessário

- Detalhe estruturas de dados

- Mencione padrões arquiteturais relevantes

  

### TRATAMENTO DE AMBIGUIDADES

Sempre que identificar informações vagas ou incompletas no PRD, interrompa a geração do FRD e faça perguntas específicas como:

  

**Exemplos de perguntas críticas:**

- "O PRD menciona 'lances em tempo real'. Qual a latência máxima aceitável?"

- "Para 'validação automática', qual algoritmo/serviço usar?"

- "O 'valor base sugerido' - como calcular? Que dados históricos?"

- "Para 'múltiplos lances', há limite por usuário/tempo?"

- "O status 'pendente' - quanto tempo até expirar?"

  

## PADRÕES DE ESPECIFICAÇÃO

  

### PARA INTEGRAÇÕES

```

**Integração [Nome]:**

- Endpoint: [URL/método]

- Autenticação: [tipo]

- Rate limit: [quantidade]

- Timeout: [segundos]

- Retry policy: [estratégia]

```

  

### PARA REGRAS DE NEGÓCIO

```

**RN### - [Nome da Regra]**

- **Condição:** [quando aplicar]

- **Ação:** [o que fazer]

- **Exceção:** [casos especiais]

- **Validação:** [como verificar]

```

  

### PARA DADOS

```

**Campo:** [nome]

- **Tipo:** [string/int/decimal/etc]

- **Tamanho:** [limitações]

- **Obrigatório:** [sim/não]

- **Validação:** [regras específicas]

```

  

## PROCESSO DE GERAÇÃO

  

### PASSO 1: ANÁLISE INICIAL

Leia o PSD completo e identifique:

- Funcionalidades principais

- Atores envolvidos

- Integrações mencionadas

- Requisitos não-funcionais

  

### PASSO 2: IDENTIFICAÇÃO DE LACUNAS

Liste todas as ambiguidades encontradas e formule perguntas específicas

  

### PASSO 3: GERAÇÃO ESTRUTURADA

Após esclarecimentos, gere o FRD seguindo exatamente a estrutura definida

  

## CRITÉRIOS DE QUALIDADE

  

### ✅ FPSD DEVE CONTER

- Especificações técnicas implementáveis

- Regras de negócio sem ambiguidade

- Casos de uso com fluxos completos

- Critérios de aceite mensuráveis

- Integrações bem documentadas

  

### ❌ FPSD NÃO DEVE CONTER

- Linguagem vaga ou genérica

- Especificações incompletas

- Casos de uso superficiais

- Regras de negócio ambíguas

- Referencias a "definir depois"

  

## INSTRUÇÕES FINAIS

  

1. **SEMPRE** questione ambiguidades antes de prosseguir

2. **MANTENHA** o nível técnico apropriado para desenvolvedores

3. **SEJA ESPECÍFICO** em todas as especificações

4. **NUMERE** todos os requisitos, regras e casos de uso

5. **INCLUA** a matriz de rastreabilidade completa

6. **REVISE** a consistência entre todas as seções
