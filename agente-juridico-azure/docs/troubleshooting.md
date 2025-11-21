# 🔧 Troubleshooting - Solução de Problemas

## Problemas Comuns e Soluções

---

## 🚨 Problema 1: Agente não lê o PDF / Usa informações antigas

### Sintomas:
- O agente menciona dados de um documento anterior
- Mistura informações de processos diferentes
- Ignora o novo arquivo anexado

### ✅ Solução:

**Método 1 - Limpar Contexto (Recomendado):**
1. Clique em **"New Chat"** ou **"Nova Conversa"**
2. Anexe o documento novamente
3. Solicite a análise

**Método 2 - Comando Explícito:**
Escreva:
```
NOVO DOCUMENTO - IGNORE TODOS OS ANTERIORES
Analise APENAS este arquivo: [nome_do_arquivo.pdf]
```

**Método 3 - Atualizar Página:**
1. Pressione `F5` ou `Ctrl + R`
2. Inicie nova conversa
3. Anexe o documento

---
## 📨 Problema 2: Telegrama não é preenchido

### Sintomas:
- Agente diz que não encontrou o modelo
- Campos { } não são preenchidos
- Mensagem: "Template não encontrado"

### ✅ Solução:

**Passo 1 - Verificar Knowledge Base:**
1. Vá em **"Agent Settings"** → **"Knowledge"**
2. Confirme que a pasta **"Telegramas"** está lá
3. Verifique se os arquivos foram indexados (status: "Completed")

**Passo 2 - Reindexar Templates:**
1. Delete a Knowledge Base atual
2. Faça upload dos templates novamente
3. Aguarde a indexação completar

**Passo 3 - Comando Correto:**
Use o nome EXATO do template:
```
Correto: "Preencha o telegrama padrão"
Errado:  "Faça o telegrama da liminar"
```

**Passo 4 - Verificar Arquivos:**
- Os templates devem estar em formato `.txt`
- Devem conter campos entre chaves `{campo}`
- Exemplo: `{numero_processo}`, `{tribunal}`, `{prazo}`

---

## ⚠️ Problema 3: "Não identificado" em vários campos

### Sintomas:
- Muitos campos aparecem como "não identificado"
- Informações importantes estão faltando

### ✅ Solução:

**Causas Possíveis:**

1. **Documento Incompleto:**
   - Verifique se o PDF contém todas as páginas
   - Confirme se não está cortado

2. **Formatação Estranha:**
   - Alguns documentos têm formatação não padronizada
   - O agente pode ter dificuldade em identificar

3. **Informação Realmente Não Existe:**
   - Nem todas decisões têm todos os campos
   - "não identificado" pode ser correto

**Como melhorar:**
- Envie o documento completo (todas as páginas)
- Se possível, use PDFs oficiais (de sistemas judiciais)
- Forneça contexto adicional se souber informações

---

## 🔍 Problema 4: Análise muito lenta

### Sintomas:
- Agente demora muito para responder
- Timeout ou erro de conexão

### ✅ Solução:

**Passo 1 - Verificar Tamanho do Arquivo:**
- PDFs muito grandes (>10 MB) demoram mais
- Comprima o PDF se possível

**Passo 2 - Conexão com Internet:**
- Verifique sua conexão
- Tente novamente em alguns minutos

**Passo 3 - Reiniciar:**
1. Atualize a página (F5)
2. Faça login novamente
3. Tente em uma nova conversa

---

## 📋 Problema 5: Campos { } não são substituídos

### Sintomas:
- Telegrama retorna com `{numero_processo}` não preenchido
- Chaves permanecem no texto

### ✅ Solução:

**Verificar Template:**
1. Abra o arquivo do template
2. Confirme que os nomes dos campos estão corretos
3. Use nomes consistentes:
   - ✅ `{numero_processo}`
   - ❌ `{nº processo}` (com espaço)
   - ❌ `{NUMERO_PROCESSO}` (maiúsculas)

**Verificar Extração:**
- Peça primeiro só a análise
- Veja se o agente identificou as informações
- Se ele não encontrou, não consegue preencher

---

## 🤖 Problema 6: Erro "Rate Limit" ou "Too Many Requests"

### Sintomas:
- Mensagem de limite de requisições
- Agente para de responder

### ✅ Solução:

**Aguarde alguns minutos:**
- Azure tem limite de requisições por minuto
- Espere 5-10 minutos
- Tente novamente

**Dica:** Não faça múltiplos uploads simultâneos

---

## 🔐 Problema 7: Não consigo acessar o Azure AI Foundry

### Sintomas:
- Erro de login
- Página não carrega

### ✅ Solução:

**Passo 1 - Verificar Conta:**
- Use conta Microsoft válida
- Confirme que tem acesso ao Azure

**Passo 2 - Limpar Cache:**
1. Pressione `Ctrl + Shift + Del`
2. Limpe cache do navegador
3. Tente novamente

**Passo 3 - Tentar Outro Navegador:**
- Chrome, Edge, Firefox
- Use modo anônimo para testar

---

## ❓ Problema 8: Não encontrei solução aqui

### ✅ O que fazer:

**1. Documentação Oficial:**
- https://learn.microsoft.com/azure/ai-studio/

**2. Suporte Azure:**
- Portal Azure → "Help + Support"

---

## 📊 Checklist de Diagnóstico

Antes de reportar um problema, verifique:

- [ ] Estou em uma **nova conversa**?
- [ ] O arquivo foi **anexado corretamente**?
- [ ] O PDF está **legível** (texto selecionável)?
- [ ] A **Knowledge Base** está configurada?
- [ ] Usei o **comando correto**?
- [ ] Aguardei tempo suficiente para resposta?
- [ ] Minha **conexão com internet** está OK?
- [ ] Já tentei **atualizar a página**?

---

## 🎯 Dicas de Prevenção

### Para Evitar Problemas:

✅ **Dê preferência a usar "New Chat" para novos documentos**
✅ **Verifique o PDF antes de anexar** (legibilidade)
✅ **Mantenha templates atualizados** na Knowledge Base
✅ **Use comandos claros e diretos**
✅ **Não anexe múltiplos arquivos simultaneamente**
✅ **Aguarde a resposta completa** antes de novo comando

---

</div>