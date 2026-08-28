# warera-painel-web

Este repositório **não tem código**. Só serve o painel WarEra ao GitHub Pages,
no ramo `gh-pages`:

- `index.html` — o painel (desenho e lógica de apresentação)
- `dados.enc` — o relatório, **cifrado**

O relatório vai cifrado com AES-256-CTR, chave derivada de uma frase-passe por
PBKDF2-SHA256 e autenticado com HMAC-SHA256; abre no browser com WebCrypto e a
frase nunca sai de lá. Sem a frase, `dados.enc` são bytes.

O código que produz o relatório vive noutro repositório, privado.

Existe separado porque o GitHub Pages não serve repositórios privados no plano
gratuito — em vez de tornar o código público, publica-se só o resultado.

https://noelferreira12.github.io/warera-painel-web/
