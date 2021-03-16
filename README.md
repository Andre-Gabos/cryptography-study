# cryptography-study
Estudo de níveis de criptografia a partir de um site com as ferramentas de registro de conta e login.

A intenção é de aplicar diferentes ferramentas para desenvolver a criptografia e segurança do site, desde o uso de uma string como chave até formas mais complexas.

### Versões
#### v1.
Criptografia construída a partir do uso de uma string chave (usando mongoose-encryption) e environment variables (usando dotenv), para criptografar a senha do usuário
e esconder a chave de criptografia, respectivamente. [Commit f8150f9](https://github.com/Andre-Gabos/cryptography-study/commit/f8150f961c6c6a3f625fc9154b04bfc8d01b26ce)

#### v2.
Troca do método de chave + variáveis para criptografia por hashing e identificação por comparação do hash, utilizando a extensão no node.js, md5. [Commit 89b96ae](https://github.com/Andre-Gabos/cryptography-study/commit/89b96ae464cf3eea02aa04daf7cfd6e87520a7f1)

#### v3.
Nesta versão foi aplicado o método de salting + hashing. O modulo utilizado para o hashing foi trocado, do md5 para o BCrypt, com o objetivo de complexificar o hash e com isso aumentar a segurança. O BCrypt também inclui a função de salting, que foi aplicada em 10 rodadas para esse teste. [Commit 0bcd5bd](https://github.com/Andre-Gabos/cryptography-study/commit/0bcd5bd6d495b0c6cc7f06c72447cf74887406e8)

### v4.
Essa versão inclui a aplicação dos métodos anteriores em conjunto e a adição de cookies, com a utilização do Passport e Express-session. String chave, salting e hashing são executados por esse módulos, e a integração à database (MongoDB), para criptografar as senhas guardadas e autenticação, é feita a partir do módulo Passport-local-mongoose. Nessa aplicação, com a introdução dos cookies, é possível manter o login autenticado e a página /secrets acessível até que o navegador seja fechado. [Commit 080c3d5](https://github.com/Andre-Gabos/cryptography-study/commit/080c3d544482528de987a79cc15f72f801a846e4)
