# Projecto Recomeço — versão 0.3 (GitHub Pages)

Esta pasta está preparada para publicação como site estático no GitHub Pages e instalação no Android como PWA.

## Publicar usando apenas o telemóvel
1. No Chrome, abre https://github.com e entra na tua conta (ou cria uma conta).
2. Cria um repositório novo, por exemplo `projecto-recomeco`. Se aparecer a opção de repositório público/privado, escolhe **Public** para facilitar a publicação gratuita pelo GitHub Pages.
3. Dentro do repositório, usa **Add file → Upload files** e envia os seis ficheiros desta pasta: `index.html`, `manifest.json`, `service-worker.js`, `icon-192.png`, `icon-512.png` e `README.md`.
4. Carrega em **Commit changes**.
5. No repositório, abre **Settings → Pages**.
6. Em **Build and deployment**, escolhe **Deploy from a branch**; branch `main`; pasta `/(root)`; carrega em **Save**.
7. Aguarda a publicação. O endereço será parecido com `https://TEU-NOME.github.io/projecto-recomeco/` (substitui pelo teu nome e repositório reais). Usa o endereço que o próprio GitHub Pages mostrar.
8. No Samsung Galaxy A05, abre esse endereço no Chrome. Menu ⋮ → **Adicionar ao ecrã inicial** ou **Instalar aplicação**, se aparecer.
9. Abre a aplicação pelo ícone criado. Exporta regularmente os dados em JSON e guarda o ficheiro num local seguro.

## Importante
- Não partilhes a pasta/repositório se adicionares dados pessoais. Esta aplicação não envia os registos para o GitHub; os registos ficam no armazenamento local do navegador/dispositivo.
- Os dados do navegador original não passam automaticamente para a versão alojada. Usa a exportação JSON da versão antiga como cópia de segurança; a importação automática ainda não está implementada.
- A aplicação já tem service worker para cache/offline depois da primeira visita. Isto não transforma os lembretes actuais em notificações garantidas quando a aplicação está fechada. Os lembretes por horário ainda dependem de a página estar activa. Para notificações verdadeiras em segundo plano seria necessária uma implementação adicional (push/servidor ou Android nativo).
- Não guardes senhas, dados bancários nem outras informações altamente sensíveis no diário.
