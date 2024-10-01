<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Informa Esportes</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/fotos-premium/campo-de-futebol-de-fundo-de-grama-verde_41969-7902.jpg');
            background-size: cover;
            color: #000000;
            margin: 0;
            padding: 0;
            position: relative;
        }
        header {
            background-color: rgba(255, 255, 255, 0.9);
            color: #006400;
            padding: 20px;
            text-align: center;
            position: relative;
        }
        h1 {
            font-size: 48px;
            margin: 0;
            color: #006400;
        }
        h2 {
            font-size: 24px;
            margin: 5px 0 20px 0;
            font-weight: normal;
            color: #006400;
        }
        nav ul {
            list-style-type: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin-right: 10px;
        }
        nav ul li a {
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
            border: 2px solid #006400;
            border-radius: 4px;
            background-color: #333;
        }
        nav ul li a:hover {
            background-color: #555;
        }
        .auth-buttons {
            position: absolute;
            top: 20px;
            right: 20px;
        }
        .btn-auth {
            margin-left: 10px;
            padding: 10px 20px;
            background-color: #006400;
            color: #fff;
            border: none;
            border-radius: 5px;
            font-size: 16px;
            cursor: pointer;
            text-decoration: none;
        }
        .btn-auth:hover {
            background-color: #004b23;
        }
        .container {
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            max-width: 800px;
            margin: 0 auto;
            border-radius: 8px;
        }
        .news-list {
            margin-top: 20px;
        }
        .news-list .news-item {
            margin-bottom: 20px;
            padding: 10px;
            border-left: 5px solid #006400;
            background-color: #f9f9f9;
            border-radius: 5px;
        }
        .news-item h3 {
            margin: 0;
            color: #006400;
        }
        .news-item p {
            margin: 5px 0;
            color: #333;
        }
        .news-item .btn-ver-mais {
            display: inline-block;
            margin-top: 10px;
            padding: 8px 12px;
            background-color: #006400;
            color: white;
            border: none;
            border-radius: 4px;
            text-decoration: none;
        }
        .news-item .btn-ver-mais:hover {
            background-color: #004b23;
        }
        .news-item .fonte-link {
            display: inline-block;
            margin-top: 10px;
            padding: 5px 10px;
            color: #ffffff;
            background-color: #006400;
            text-decoration: none;
            border-radius: 4px;
            font-size: 14px;
        }
        .news-item .fonte-link:hover {
            background-color: #004b23;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #333;
            color: #fff;
            margin-top: 20px;
        }

        /* Adaptações para dispositivos móveis */
        @media (max-width: 768px) {
            h1 {
                font-size: 32px;
            }
            h2 {
                font-size: 18px;
            }
            .auth-buttons {
                position: relative;
                text-align: center;
                margin-top: 10px;
            }
            .btn-auth {
                display: block;
                margin: 5px auto;
                width: 80%;
            }
            nav ul {
                text-align: center;
            }
            nav ul li {
                display: block;
                margin-bottom: 10px;
            }
            nav ul li a {
                display: block;
                width: 80%;
                margin: 0 auto;
            }
            .container {
                padding: 10px;
                max-width: 90%;
            }
            .news-item {
                padding: 10px;
            }
            .news-item h3 {
                font-size: 18px;
            }
            .news-item p {
                font-size: 14px;
            }
            .news-item .btn-ver-mais, .news-item .fonte-link {
                padding: 6px 10px;
                font-size: 12px;
            }
        }

        /* Estilos para telas maiores que 1024px */
        @media (min-width: 1024px) {
            h1 {
                font-size: 56px;
            }
            h2 {
                font-size: 28px;
            }
            .container {
                max-width: 1000px;
            }
            .news-item h3 {
                font-size: 24px;
            }
            .news-item p {
                font-size: 16px;
            }
            .news-item .btn-ver-mais, .news-item .fonte-link {
                font-size: 16px;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Informa Esportes</h1>
        <h2>As últimas notícias sobre esportes</h2>
        
        <div class="auth-buttons">
            <button class="btn-auth" onclick="window.location.href='login.html'">Login</button>
            <button class="btn-auth" onclick="window.location.href='registro.html'">Registrar-se</button>
        </div>

        <nav>
            <ul>
                <li><a href="#">Principais notícias</a></li>
                <li><a href="noticias.html">Adicionar Notícia</a></li> <!-- Atualizado para a nova página -->
            </ul>
        </nav>
    </header>
    
    <div class="container">
        <section id="home">
            <h2>Bem-vindo ao Informa Esportes!</h2>
            <p>Fique por dentro das últimas notícias.</p>
        </section>
        
        <section id="news" class="news-list">
            <h2>Notícias Recentes</h2>
            <div id="noticiasContainer">
                <div class="news-item">
                    <h3>Vini Jr. e o racismo no futebol</h3>
                    <p>À CNN, Vini Jr. revela que o Real Madrid cogita deixar o campo em caso de racismo...</p>
                    <a href="https://www.cnnbrasil.com.br/esportes/futebol/futebol-internacional/futebol-espanhol/a-cnn-vini-jr-revela-que-real-madrid-cogita-deixar-campo-em-caso-de-racismo/#:~:text=Porque%2C%20se%20as%20coisas%20n%C3%A3o,o%20atacante%20do%20Real%20Madrid." target="_blank" class="fonte-link">Ver Fonte</a>
                    <a href="#" class="btn-ver-mais">Ver mais</a>
                </div>
                <div class="news-item">
                    <h3>Desafio testado na Copa do Mundo Feminina Sub-20</h3>
                    <p>Alternativa econômica ao VAR, “desafio” é testado na Copa do Mundo Feminina Sub-20...</p>
                    <a href="https://www.cnnbrasil.com.br/esportes/futebol/futebol-internacional/alternativa-economica-ao-var-desafio-e-testado-na-copa-do-mundo-feminina-sub-20/#:~:text=eSports-,Alternativa%20econ%C3%B4mica%20ao%20VAR%2C%20%E2%80%9Cdesafio%E2%80%9D%20%C3%A9%20testado%20na%20Copa,do%20Mundo%20Feminina%20Sub%2D20&text=O%20Football%20Video%20Support%20Assistant,(V%2DA)%20na%20Copa%20do%20Mundo." target="_blank" class="fonte-link">Ver Fonte</a>
                    <a href="#" class="btn-ver-mais">Ver mais</a>
                </div>
            </div>
        </section>
    </div>

    <footer>
        <p>&copy; 2024 Informa Esportes. Todos os direitos reservados.</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const noticias = JSON.parse(localStorage.getItem('noticias')) || [];
            const noticiasContainer = document.getElementById('noticiasContainer');

            noticias.forEach(noticia => {
                const noticiaDiv = document.createElement('div');
                noticiaDiv.classList.add('news-item');
                noticiaDiv.innerHTML = `
                    <h3>${noticia.titulo}</h3>
                    <p>${noticia.conteudo}</p>
                    <a href="#" class="btn-ver-mais">Ver mais</a>
                `;
                noticiasContainer.appendChild(noticiaDiv);
            });
        });
    </script>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adicionar Notícia - Informa Esportes</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/fotos-premium/campo-de-futebol-de-fundo-de-grama-verde_41969-7902.jpg');
            background-size: cover;
            color: #000000;
            margin: 0;
            padding: 0;
            position: relative;
        }
        header {
            background-color: rgba(255, 255, 255, 0.9);
            color: #006400;
            padding: 20px;
            text-align: center;
        }
        h1 {
            font-size: 48px;
            margin: 0;
            color: #006400;
        }
        h2 {
            font-size: 24px;
            margin: 5px 0 20px 0;
            font-weight: normal;
            color: #006400;
        }
        nav ul {
            list-style-type: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin-right: 10px;
        }
        nav ul li a {
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
            border: 2px solid #006400;
            border-radius: 4px;
            background-color: #333;
        }
        nav ul li a:hover {
            background-color: #555;
        }
        .container {
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            max-width: 800px;
            margin: 0 auto;
            border-radius: 8px;
            margin-top: 20px;
        }
        form {
            margin-top: 30px;
        }
        form label {
            display: block;
            margin-bottom: 5px;
            font-size: 18px;
            color: #006400;
        }
        form input, form textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
        }
        form input[type="submit"] {
            background-color: #006400;
            color: #fff;
            cursor: pointer;
            border: none;
            border-radius: 4px;
            padding: 10px 20px;
            font-size: 18px;
        }
        form input[type="submit"]:hover {
            background-color: #004b23;
        }
        .error {
            color: red;
            margin-top: 10px;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #333;
            color: #fff;
            margin-top: 20px;
        }
        /* Estilo do botão de voltar */
        .btn-voltar {
            display: inline-block;
            margin-top: 20px;
            padding: 10px 20px;
            background-color: #006400;
            color: #fff;
            border-radius: 5px;
            text-decoration: none;
            font-size: 16px;
            border: none;
        }
        .btn-voltar:hover {
            background-color: #004b23;
        }
    </style>
</head>
<body>
    <header>
        <h1>Informa Esportes</h1>
        <h2>Adicionar Notícia</h2>
    </header>

    <div class="container">
        <!-- Botão para voltar para a página principal -->
        <a href="trabalho1.html" class="btn-voltar">Voltar para a Página Principal</a>

        <form id="formNoticia">
            <h2>Envie uma nova notícia</h2>
            <label for="titulo">*Título da Notícia:</label>
            <input type="text" id="titulo" name="titulo" placeholder="Digite o título da notícia" required>

            <label for="conteudo">*Conteúdo da Notícia:</label>
            <textarea id="conteudo" name="conteudo" placeholder="Escreva o conteúdo da notícia aqui" required></textarea>

            <label for="fonte">*Link da Fonte:</label>
            <input type="url" id="fonte" name="fonte" placeholder="Digite o link da fonte da notícia" required>

            <label for="categoria">Categoria (Opcional):</label>
            <input type="text" id="categoria" name="categoria" placeholder="Ex: Futebol, Basquete">

            <input type="submit" value="Enviar Notícia">
            <p id="feedback" class="error"></p>
        </form>
<section id="news" class="news-list">
    <h2>Notícias Recentes</h2>
    <div id="noticiasContainer">
        <!-- As notícias serão carregadas aqui -->
    </div>
</section>

<script>
    document.addEventListener('DOMContentLoaded', function() {
        const noticias = JSON.parse(localStorage.getItem('noticias')) || [];
        const noticiasContainer = document.getElementById('noticiasContainer');

        noticias.forEach(noticia => {
            const noticiaDiv = document.createElement('div');
            noticiaDiv.classList.add('news-item');
            noticiaDiv.innerHTML = `
                <h3>${noticia.titulo}</h3>
                <p>${noticia.conteudo}</p>
                <a href="#" class="btn-ver-mais">Ver mais</a>
            `;
            noticiasContainer.appendChild(noticiaDiv);
        });
    });
</script>

        <script>
            document.getElementById('formNoticia').addEventListener('submit', function(event) {
                event.preventDefault();

                var titulo = document.getElementById('titulo').value.trim();
                var conteudo = document.getElementById('conteudo').value.trim();
                var fonte = document.getElementById('fonte').value.trim();
                var categoria = document.getElementById('categoria').value.trim();
                var feedback = document.getElementById('feedback');

                if (!titulo || !conteudo || !fonte) {
                    feedback.textContent = "O título, o conteúdo e o link da fonte são obrigatórios.";
                } else {
                    feedback.textContent = "";
                    // Adiciona a notícia a um contêiner de notícias (pode ser customizado conforme o sistema)
                    console.log("Notícia adicionada:", {titulo, conteudo, fonte, categoria});
                    document.getElementById('formNoticia').reset();
                }
            });
        </script>
    </div>

    <footer>
        &copy; 2024 Informa Esportes
    </footer>
</body>
</html>
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registro - Informa Esportes</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/fotos-premium/campo-de-futebol-de-fundo-de-grama-verde_41969-7902.jpg');
            background-size: cover;
            color: #000000;
            margin: 0;
            padding: 0;
            position: relative;
        }
        header {
            background-color: rgba(255, 255, 255, 0.9);
            color: #006400;
            padding: 20px;
            text-align: center;
        }
        h1 {
            font-size: 48px;
            margin: 0;
            color: #006400;
        }
        h2 {
            font-size: 24px;
            margin: 5px 0 20px 0;
            font-weight: normal;
            color: #006400;
        }
        .container {
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            max-width: 800px;
            margin: 0 auto;
            border-radius: 8px;
        }
        form {
            margin-top: 30px;
        }
        form label {
            display: block;
            margin-bottom: 5px;
        }
        form input {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        form input[type="submit"] {
            background-color: #333;
            color: #fff;
            cursor: pointer;
            border: none;
            border: 2px solid #006400;
        }
        form input[type="submit"]:hover {
            background-color: #555;
        }
        .error {
            color: red;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #333;
            color: #fff;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Informa Esportes</h1>
        <h2>Registro de Usuário</h2>
    </header>
    
    <div class="container">
        <form id="formRegistro">
            <h1>Criar Conta</h1>
            <p>Preencha os campos abaixo para se registrar no Informa Esportes.</p>
            
            <label for="nome">*Nome Completo:</label>
            <input type="text" id="nome" name="nome" placeholder="Digite seu nome completo" required>
            
            <label for="email">*E-mail:</label>
            <input type="email" id="email" name="email" placeholder="Digite seu e-mail" required>
            
            <label for="senha">*Senha:</label>
            <input type="password" id="senha" name="senha" placeholder="Digite uma senha" required>
            
            <label for="confirmarSenha">*Confirmar Senha:</label>
            <input type="password" id="confirmarSenha" name="confirmarSenha" placeholder="Confirme sua senha" required>
            
            <input type="submit" value="Registrar">
            <p id="feedback" class="error"></p>
        </form>

        <script>
            document.getElementById('formRegistro').addEventListener('submit', function(event) {
                event.preventDefault(); // Impede o envio padrão do formulário

                var nome = document.getElementById('nome').value.trim();
                var email = document.getElementById('email').value.trim();
                var senha = document.getElementById('senha').value.trim();
                var confirmarSenha = document.getElementById('confirmarSenha').value.trim();
                var feedback = document.getElementById('feedback');

                // Validação básica do formulário
                if (!nome || !email || !senha || !confirmarSenha) {
                    feedback.textContent = "Todos os campos marcados com * são obrigatórios.";
                } else if (senha !== confirmarSenha) {
                    feedback.textContent = "As senhas não coincidem.";
                } else {
                    feedback.textContent = "";

                    // Exemplo de como tratar os dados (aqui seria a parte de integração com o backend)
                    alert('Usuário registrado com sucesso!');

                    // Redireciona para a página inicial
                    window.location.href = 'trabalho1.html'; // Altere para o nome correto do arquivo da sua página inicial
                    
                    // Limpa os campos do formulário
                    document.getElementById('formRegistro').reset();
                }
            });
        </script>
    </div>
    
    <footer>
        &copy; 2024 Informa Esportes
    </footer>
</body>
</html>

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login - Informa Esportes</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-image: url('https://img.freepik.com/fotos-premium/campo-de-futebol-de-fundo-de-grama-verde_41969-7902.jpg');
            background-size: cover;
            color: #000000;
            margin: 0;
            padding: 0;
            position: relative;
        }
        header {
            background-color: rgba(255, 255, 255, 0.9);
            color: #006400;
            padding: 20px;
            text-align: center;
        }
        h1 {
            font-size: 48px;
            margin: 0;
            color: #006400;
        }
        h2 {
            font-size: 24px;
            margin: 5px 0 20px 0;
            font-weight: normal;
            color: #006400;
        }
        .container {
            padding: 20px;
            background-color: rgba(255, 255, 255, 0.8);
            max-width: 800px;
            margin: 0 auto;
            border-radius: 8px;
        }
        form {
            margin-top: 30px;
        }
        form label {
            display: block;
            margin-bottom: 5px;
        }
        form input {
            width: 100%;
            padding: 8px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        form input[type="submit"] {
            background-color: #333;
            color: #fff;
            cursor: pointer;
            border: none;
            border: 2px solid #006400;
        }
        form input[type="submit"]:hover {
            background-color: #555;
        }
        .error {
            color: red;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #333;
            color: #fff;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Informa Esportes</h1>
        <h2>Login de Usuário</h2>
    </header>
    
    <div class="container">
        <form id="loginForm">
            <h1>Acessar Conta</h1>
            <p>Preencha os campos abaixo para fazer login.</p>
            
            <label for="email">*E-mail:</label>
            <input type="email" id="email" name="email" placeholder="Digite seu e-mail" required>
            
            <label for="password">*Senha:</label>
            <input type="password" id="password" name="password" placeholder="Digite sua senha" required>
            
            <input type="submit" value="Entrar">
            <p id="feedback" class="error"></p>
        </form>
    </div>

    <footer>
        &copy; 2024 Informa Esportes
    </footer>

    <script>
        // Função para redirecionar o usuário após o login correto
        function redirecionarAposLogin() {
            window.location.href = 'index.html'; // Redireciona para a página inicial
        }

        // Evento de submit do formulário de login
        document.getElementById('loginForm').addEventListener('submit', function(event) {
            event.preventDefault(); // Impede o envio padrão do formulário

            const email = document.getElementById('email').value.trim();
            const password = document.getElementById('password').value.trim();

            // Simulação de verificação de login
            if (email === 'usuario@example.com' && password === 'senha') { // Substitua pela sua lógica de autenticação
                redirecionarAposLogin(); // Chama a função para redirecionar
            } else {
                alert("Email ou senha incorretos."); // Mensagem de erro
            }
        });
    </script>
</body>
</html>
