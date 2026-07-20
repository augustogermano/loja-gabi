# Loja Gabi — Guia para colocar o site no ar

Este pacote já vem pronto com:
- `index.html` — o site
- `content/products.json` — os produtos (é isso que o painel de admin edita)
- `admin/` — o painel de login onde sua cunhada sobe fotos e preços
- `images/` — pasta das fotos (tem uma imagem de exemplo lá)

## Passo 1 — Criar conta no GitHub (grátis)
1. Acesse github.com e crie uma conta (se ainda não tiver).
2. Crie um repositório novo, por exemplo `loja-gabi`.
3. Suba todos os arquivos desta pasta para esse repositório (pode arrastar os arquivos direto pela interface do GitHub, em "Add file" > "Upload files").

## Passo 2 — Publicar no Netlify (grátis)
1. Acesse app.netlify.com e crie uma conta (pode entrar direto com o GitHub).
2. Clique em "Add new site" > "Import an existing project".
3. Escolha o repositório `loja-gabi` que você criou.
4. Não precisa mudar nada nas configurações de build — clique em "Deploy".
5. Em poucos segundos o Netlify te dá um link tipo `nome-aleatorio.netlify.app`. O site já está no ar.

## Passo 3 — Ativar o painel de admin (Identity + Git Gateway)
Isso é o que permite ela fazer login e editar.
1. No painel do Netlify, vá em **Site configuration > Identity** e clique em "Enable Identity".
2. Em "Registration preferences", marque **Invite only** (assim só quem você convidar consegue entrar).
3. Ainda em Identity, vá em **Services > Git Gateway** e clique em "Enable Git Gateway".
4. Volte para a aba **Identity > Invite users**, digite o e-mail da sua cunhada e envie o convite.
5. Ela vai receber um e-mail, clicar no link, criar uma senha.
6. A partir daí, ela acessa `seusite.netlify.app/admin` para editar fotos e preços — sem mexer em nenhum código.

## Passo 4 — Comprar o domínio próprio
1. Compre o domínio (ex: `lojagabi.com.br`) em um registrador como registro.br (domínios .com.br) ou godaddy.com (~R$40-60/ano).
2. No Netlify, vá em **Domain management > Add a domain** e digite o domínio comprado.
3. O Netlify vai te mostrar os registros de DNS que você precisa colocar no site do registrador (geralmente 1-2 registros tipo "A" ou "CNAME"). É só copiar e colar lá.
4. Pode levar de alguns minutos até 24h para o domínio próprio começar a funcionar.

## Depois disso
- Ela edita fotos e preços em `seusite.com/admin`, faz login e usa um formulário simples (nada de código).
- Cada alteração que ela salvar atualiza o site sozinho, automaticamente, em 1-2 minutos.
- Você continua dono do "código" do site (repositório no GitHub) caso precise mudar o design no futuro.
