# Remember Me — versão para celular e lojas

## Uso em iPhone e Android

Publique esta pasta em uma hospedagem HTTPS. Depois, abra o endereço pelo celular:

- **iPhone (Safari):** Compartilhar → **Adicionar à Tela de Início**.
- **Android (Chrome):** menu ⋮ → **Instalar app** ou **Adicionar à tela inicial**.

O Remember Me será aberto como aplicativo e a tela principal continuará disponível mesmo sem internet após o primeiro acesso.

## Login e dados

Esta versão possui uma tela de cadastro e login para testar a experiência do usuário. As contas, senhas e registros ficam exclusivamente no armazenamento local do navegador; portanto, não é uma autenticação segura nem sincroniza dados entre aparelhos.

## Publicação futura nas lojas

Esta versão é uma PWA e já contém `manifest.webmanifest`, `service-worker.js` e o arquivo de configuração do Capacitor. Para gerar os aplicativos de loja, o próximo passo é instalar o Capacitor no projeto e adicionar os destinos Android e iOS. Ele cria os projetos nativos mantendo a mesma interface web.

Antes da publicação comercial, recomenda-se substituir `com.rememberme.app` por um identificador definitivo e criar as contas de desenvolvedor Apple e Google. Também será necessário integrar um provedor de autenticação seguro e um banco de dados em nuvem, para que contas e registros possam ser protegidos e usados em mais de um aparelho.
