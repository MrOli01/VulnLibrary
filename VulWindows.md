# Técnicas em Windows

### 🛠️ Técnica 1: Invoke-WebRequest

**Descrição:**

O cmdlet `Invoke-WebRequest` do PowerShell é utilizado para enviar solicitações HTTP e HTTPS a páginas da web ou serviços. Ele pode ser explorado por agentes mal-intencionados para baixar scripts ou arquivos maliciosos diretamente da internet, facilitando a execução de código remoto sem a necessidade de ferramentas externas. [Microsoft Learn+1Microsoft Learn+1](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-7.5&utm_source=chatgpt.com)

**Recomendações de Mitigação:**

1. **Monitoramento de Comandos PowerShell:**
    - Configure o EDR para registrar e alertar sobre o uso de `Invoke-WebRequest`, especialmente quando utilizado para baixar arquivos executáveis ou scripts.
2. **Políticas de Execução Restritivas:**
    - Implemente políticas de execução do PowerShell que restrinjam a execução de scripts não assinados ou provenientes de fontes não confiáveis.
3. **Regras de Redução da Superfície de Ataque (ASR):**
    - Utilize regras de ASR para bloquear a execução de comandos que possam ser utilizados para baixar e executar conteúdo malicioso.

**Referências:**

- [Invoke-WebRequest - Microsoft Docs](https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/invoke-webrequest?view=powershell-7.5)
- [Regras de Redução da Superfície de Ataque (ASR) - Microsoft Docs](https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-reference)


