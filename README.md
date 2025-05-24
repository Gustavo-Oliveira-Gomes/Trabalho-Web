# Comparação entre XmlHttpRequest, fetch, Promises e async/await

## 🔍 Introdução

Esta pesquisa tem como objetivo comparar quatro abordagens para realizar requisições AJAX no JavaScript: XmlHttpRequest, fetch, Promises e async/await. Para isso, foram desenvolvidas três implementações de um exemplo chamado ajax3.html, cada uma utilizando uma das abordagens modernas.

---

## 🧪 Comparativo das Tecnologias

| Tecnologia       | Ano de Introdução | Sintaxe Simples | Suporte Nativo | Controle de Fluxo | Suporte a Promises |
|------------------|------------------|------------------|-----------------|-------------------|---------------------|
| XmlHttpRequest   | ~2000            | ❌ Verboso       | ✅ Amplo         | ❌ Complexo         | ❌ Não               |
| fetch            | 2015             | ✅ Moderna        | ✅ Amplo         | ⚠️ Encadeamento     | ✅ Sim               |
| Promises         | 2015             | ✅ Moderna        | ✅ Amplo         | ⚠️ Encadeamento     | ✅ Sim               |
| async/await      | 2017             | ✅ Muito clara    | ✅ Amplo         | ✅ Simples          | ✅ Sim               |

---

## 📊 Comparação de Desempenho

Em um teste simples de carregamento de um arquivo de texto (dados.txt), o tempo de execução entre os métodos fetch, Promises e async/await foi praticamente o mesmo. A diferença principal reside na *legibilidade* e *facilidade de manutenção* do código.

| Método           | Facilidade de Uso | Legibilidade | Tempo Médio de Execução |
|------------------|-------------------|--------------|--------------------------|
| fetch            | ✅ Boa             | ✅ Boa       | ~20ms                   |
| Promises         | ⚠️ Moderada        | ⚠️ Média     | ~21ms                   |
| async/await      | ✅ Excelente       | ✅ Excelente | ~20ms                   |

---

## 📁 Estrutura do Repositório

- fetch-ajax3.html – Implementação usando fetch
- promise-ajax3.html – Implementação usando Promises
- async-await-ajax3.html – Implementação usando async/await
- dados.txt – Arquivo de dados carregado pelas páginas
- README.md – Documento com a pesquisa comparativa

---

## 📌 Conclusão

O async/await provou ser a abordagem mais intuitiva e limpa para código assíncrono, principalmente quando há múltiplas operações em sequência. A API fetch é moderna e fácil de usar, enquanto Promises ainda exigem um pouco mais de atenção em encadeamentos. XmlHttpRequest, apesar de funcional, está obsoleto para a maioria dos casos modernos.