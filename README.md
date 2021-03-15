# cryptography-study
Estudo de níveis de criptografia a partir de um site com as ferramentas de registro de conta e login.

A intenção é de aplicar diferentes ferramentas para desenvolver a criptografia e segurança do site, desde o uso de uma string como chave até formas mais complexas.

### Versões
#### v1.
Criptografia construída a partir do uso de uma string chave (usando mongoose-encryption) e environment variables (usando dotenv), para criptografar a senha do usuário
e esconder a chave de criptografia, respectivamente. [Commit f8150f9](https://github.com/Andre-Gabos/cryptography-study/commit/f8150f961c6c6a3f625fc9154b04bfc8d01b26ce)

#### v2.
Troca do método de chave + variáveis para criptografia por hashing e identificação por comparação do hash, utilizando a extensão no node.js, md5. [Commit 89b96ae](https://github.com/Andre-Gabos/cryptography-study/commit/89b96ae464cf3eea02aa04daf7cfd6e87520a7f1)
