# NOÛS 1.0 — protótipo web instalável

## Conteúdo
- `index.html`: interface e funcionalidades locais.
- `manifest.json`: metadados para instalação como PWA.
- `sw.js`: cache básico para uso offline após a primeira visita por HTTPS.

## Teste local
Abra `index.html` no navegador. Algumas funcionalidades de voz dependem do navegador e podem não funcionar em arquivo local.

## Publicar no GitHub Pages (HTTPS)
1. Entre em https://github.com e crie um repositório chamado `nous`.
2. Envie os três arquivos (`index.html`, `manifest.json`, `sw.js`) para a raiz do repositório. Pode enviar o README também.
3. Abra Settings → Pages.
4. Em Build and deployment, escolha Deploy from a branch; selecione `main` e `/ (root)`; salve.
5. Aguarde a publicação. O endereço geralmente será `https://SEU-USUARIO.github.io/nous/`.
6. Abra o endereço no Chrome do Android. Menu ⋮ → Adicionar à tela inicial (ou Instalar app, se aparecer).

## Limitações importantes
- Protótipo sem backend e sem modelo de IA remoto: as respostas são baseadas em comandos simples, não conversa inteligente geral.
- Voz: reconhecimento de fala depende do suporte do navegador; síntese de voz usa recursos do dispositivo.
- Notas e treinos ficam no armazenamento local do navegador, sem sincronização ou cópia de segurança automática.
- Não armazene informações identificáveis de pacientes nem use este protótipo como prontuário clínico.
- A ligação direta a XOSS, Google Agenda, WhatsApp e outros serviços não está implementada.
- Para integração com IA remota, nunca coloque uma chave de API diretamente no HTML; será necessário um backend seguro.
