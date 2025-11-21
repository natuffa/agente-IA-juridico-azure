# ⚡ Guia Rápido de Uso

## 🎯 Como Usar o Agente em 4 Passos

### Passo 1️⃣: Acessar o Agente

1. Entre no **Azure AI Foundry**: https://ai.azure.com
2. Faça login com sua conta Microsoft
3. Vá em **"Agents"** no menu lateral
4. Clique no agente **"Assistente Jurídico Operacional"**

---

### Passo 2️⃣: Anexar o Documento

1. Clique no ícone de **anexo 📎** (ao lado da caixa de texto)
2. Selecione o **PDF da decisão judicial**
3. Aguarde o upload completar (aparece o nome do arquivo)

---

### Passo 3️⃣: Solicitar a Análise

Digite na caixa de texto:

```
Analise este documento
```

**Pressione Enter** e aguarde a resposta

---

### Passo 4️⃣: Obter o Telegrama (Opcional)

Após receber a análise, digite:

```
Preencha o telegrama de liminar deferida
```

Ou escolha outro modelo conforme sua necessidade.

---

## 📋 Tipos de Telegrama Disponíveis

Digite exatamente assim:

- **"Preencha o telegrama padrão"**
- **"Preencha o telegrama indicação"**
- **"Preencha o telegrama reembolso"**

---

## ✅ Resultado Esperado

### O agente vai retornar:

**1. Resumo Simples** (4-6 frases em linguagem clara)

**2. Informações Estruturadas:**
- Número do processo
- Tribunal/Comarca
- Partes (autor e réu)
- Tipo de decisão
- Contexto da ação
- Deferimento literal
- Prazos

**3. Telegrama Preenchido** (se solicitado)

---

## ⚠️ Dicas Importantes

### ✅ FAÇA:
- Use documentos judiciais **legíveis** (PDF com texto, não imagem)
- Anexe **um documento por vez**
- Inicie **nova conversa** para cada novo documento
- Verifique se o arquivo foi carregado antes de solicitar análise

### ❌ NÃO FAÇA:
- Não envie múltiplos PDFs na mesma mensagem
- Não reutilize a mesma conversa para documentos diferentes
- Não envie documentos que não sejam decisões judiciais
- Não espere que o agente "lembre" de documentos anteriores

---

## 🔄 Como Analisar Outro Documento

**Sempre que for analisar um novo documento:**

1. Clique em **"New Chat"** (Nova Conversa)
2. Anexe o novo PDF
3. Solicite a análise novamente

---

## 💡 Atalhos Úteis

### Comandos Rápidos:

| Digite | O agente vai |
|--------|-------------|
| "Analise este documento" | Extrair todas as informações |
| "Resuma este processo" | Dar um resumo objetivo |
| "Quais são os prazos?" | Listar prazos identificados |
| "Preencha o telegrama" | Preencher o template adequado |

---

## 🎯 Exemplo Completo

### Fluxo Típico:

```
1. Você: [anexa liminar_ficticia.pdf]
2. Você: "Analise este documento"
3. Agente: [retorna análise completa]
4. Você: "Preencha o telegrama padrão"
5. Agente: [retorna telegrama preenchido]
6. Você: ✅ Copia e usa o telegrama
```

---

## ⏱️ Tempo Estimado

- **Upload do documento:** 5-10 segundos
- **Análise completa:** 15-30 segundos
- **Preenchimento de telegrama:** 10-15 segundos

**Total:** Aproximadamente **1 minuto por documento** ⚡

---

## 📞 Precisa de Ajuda?

Se algo não funcionar como esperado:

1. Consulte o **[Troubleshooting](troubleshooting.md)**
2. Verifique se o documento está legível
3. Tente em uma nova conversa

---

## 🎉 Pronto!

Agora você já sabe usar o agente! 
