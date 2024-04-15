# Lista de Vulnerabilidades Comuns em Segurança de Sistemas

## 1. Injeção de SQL (SQL Injection)

- **Descrição**: Inserção de código SQL malicioso em entradas de dados que são processadas por um interpretador SQL.
- **Exemplo**: Um formulário de login onde um atacante insere `' OR '1'='1` no campo de usuário, causando autenticação sem a necessidade de senha correta.

## 2. Cross-Site Scripting (XSS)

- **Descrição**: Injeção de scripts maliciosos em websites que são posteriormente executados por outros usuários.
- **Exemplo**: Inserção de `<script>alert('Hacked!')</script>` em um campo de comentários em um blog, que é renderizado diretamente no navegador de outros usuários.

## 3. Cross-Site Request Forgery (CSRF)

- **Descrição**: Enganar um usuário autenticado para executar ações indesejadas em uma aplicação web.
- **Exemplo**: Enviar um email para um usuário com um link que, quando clicado, automaticamente envia dinheiro de sua conta bancária online para a conta do atacante.

## 4. Roubo de Sessão

- **Descrição**: Captura ou manipulação de um cookie de sessão para sequestrar uma sessão de usuário válida.
- **Exemplo**: Capturar cookies de sessão através de um ataque Man-in-the-Middle em uma rede WiFi pública.

## 5. Buffer Overflow

- **Descrição**: Escrever dados além do buffer alocado, potencialmente sobrescrevendo a memória adjacente.
- **Exemplo**: Enviar dados excessivamente longos para um programa que não verifica adequadamente o tamanho do input.

## 6. Falhas de Configuração

- **Descrição**: Configurações inadequadas ou inseguras que deixam o sistema vulnerável.
- **Exemplo**: Deixar o diretório de administração de um site acessível sem autenticação adequada.

## 7. Injeção de Comandos

- **Descrição**: Execução de comandos do sistema operacional através de uma vulnerabilidade em uma aplicação.
- **Exemplo**: Um aplicativo web que toma um caminho de arquivo via input do usuário e permite executar `rm -rf /` como parte desse caminho.

## 8. Deserialização Insegura

- **Descrição**: Deserializar dados de fontes não confiáveis que podem conter lógica maliciosa.
- **Exemplo**: Aceitar e deserializar um objeto serializado que contém uma classe maliciosa que executa código arbitrário quando deserializado.

## 9. Uso de Componentes com Vulnerabilidades Conhecidas

- **Descrição**: Inclusão de bibliotecas ou frameworks que contêm vulnerabilidades conhecidas.
- **Exemplo**: Uso de uma versão antiga de uma biblioteca de terceiros que permite a execução remota de código.

## 10. Exposição de Dados Sensíveis

- **Descrição**: Inadequada proteção de dados sensíveis, permitindo acesso não autorizado.
- **Exemplo**: Armazenamento de senhas em texto claro em um banco de dados que pode ser acessado por um ataque SQL Injection.

