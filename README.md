# Sistema de clientes

`index.html` é a página pública que deve ser enviada aos clientes. `admin.html` é o painel interno.

Para publicar: envie todos os arquivos à raiz do GitHub e ative GitHub Pages em Settings > Pages > Deploy from a branch > main / root.

O formulário público já aponta para a Edge Function `cadastro-publico` implantada no Supabase. O painel administrativo exige um usuário do Supabase Auth. Não há criação de conta no site.

A chave em `config.js` é publishable. Nunca coloque secret/service_role no GitHub.


## Identidade visual
Logo do Posto Premium incluída em `logo.png`, com paleta verde, amarelo e branco.

## CPF único
O banco Supabase possui índice UNIQUE para CPF em `clientes_publicos`. O mesmo CPF não pode ser cadastrado novamente.
