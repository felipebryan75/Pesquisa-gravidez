<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pesquisa: Gravidez na Adolescência no Brasil</title>
    <style>
        :root {
            --primary: #e91e63;
            --primary-dark: #c2185b;
            --secondary: #fce4ec;
            --text: #333;
            --light-text: #777;
            --border: #e0e0e0;
            --shadow: rgba(0, 0, 0, 0.1);
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f8f9fa;
            color: var(--text);
            line-height: 1.6;
            padding: 20px;
            max-width: 1000px;
            margin: 0 auto;
        }
        
        .container {
            background: white;
            border-radius: 12px;
            box-shadow: 0 5px 25px var(--shadow);
            overflow: hidden;
            margin: 20px 0;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: white;
            padding: 30px;
            text-align: center;
        }
        
        header h1 {
            font-size: 2.2rem;
            margin-bottom: 10px;
        }
        
        header p {
            font-size: 1.1rem;
            max-width: 700px;
            margin: 0 auto;
            opacity: 0.9;
        }
        
        .intro {
            background-color: var(--secondary);
            padding: 20px;
            text-align: center;
            font-size: 1.05rem;
            border-bottom: 1px solid var(--border);
        }
        
        .form-container {
            padding: 30px;
        }
        
        .form-group {
            margin-bottom: 30px;
            padding-bottom: 25px;
            border-bottom: 1px solid var(--border);
        }
        
        .form-group:last-child {
            border-bottom: none;
        }
        
        label {
            display: block;
            margin-bottom: 12px;
            font-weight: 600;
            color: #555;
            font-size: 1.05rem;
        }
        
        .required::after {
            content: " *";
            color: var(--primary);
        }
        
        input[type="text"],
        input[type="number"],
        input[type="email"],
        select,
        textarea {
            width: 100%;
            padding: 14px;
            border: 1px solid var(--border);
            border-radius: 8px;
            font-size: 1rem;
            margin-top: 5px;
            transition: border-color 0.3s;
        }
        
        input:focus, textarea:focus, select:focus {
            outline: none;
            border-color: var(--primary);
            box-shadow: 0 0 0 2px rgba(233, 30, 99, 0.1);
        }
        
        textarea {
            min-height: 120px;
            resize: vertical;
        }
        
        .radio-group, .checkbox-group {
            display: flex;
            flex-direction: column;
            gap: 12px;
            margin-top: 8px;
        }
        
        .option {
            display: flex;
            align-items: flex-start;
        }
        
        .option label {
            margin: 0;
            font-weight: normal;
            cursor: pointer;
        }
        
        input[type="radio"],
        input[type="checkbox"] {
            margin-right: 12px;
            margin-top: 5px;
            cursor: pointer;
        }
        
        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
            margin: 25px 0;
            text-align: center;
        }
        
        .stat-item {
            background: var(--secondary);
            border-radius: 10px;
            padding: 15px;
            flex: 1;
            min-width: 200px;
        }
        
        .stat-number {
            font-size: 2.2rem;
            font-weight: bold;
            color: var(--primary);
            margin-bottom: 5px;
        }
        
        .stat-label {
            font-size: 0.95rem;
            color: var(--light-text);
        }
        
        button {
            background: var(--primary);
            color: white;
            border: none;
            padding: 16px 32px;
            font-size: 1.1rem;
            border-radius: 8px;
            cursor: pointer;
            display: block;
            margin: 40px auto 20px;
            transition: all 0.3s;
            width: 100%;
            max-width: 300px;
            font-weight: 600;
        }
        
        button:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(233, 30, 99, 0.3);
        }
        
        footer {
            text-align: center;
            padding: 25px;
            color: var(--light-text);
            font-size: 0.95rem;
            border-top: 1px solid var(--border);
            margin-top: 20px;
        }
        
        @media (max-width: 768px) {
            .form-container {
                padding: 20px;
            }
            
            header {
                padding: 20px 15px;
            }
            
            header h1 {
                font-size: 1.8rem;
            }
            
            .stat-item {
                min-width: 150px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Pesquisa sobre Gravidez na Adolescência no Brasil</h1>
            <p>Ajude-nos a entender as percepções sobre este importante tema de saúde pública</p>
        </header>
        
        <div class="intro">
            <p>Esta pesquisa busca compreender as percepções sobre gravidez na adolescência no contexto brasileiro. Suas respostas são confidenciais e contribuirão para o desenvolvimento de políticas públicas mais efetivas.</p>
        </div>
        
        <div class="stats">
            <div class="stat-item">
                <div class="stat-number">1 em cada 5</div>
                <div class="stat-label">bebês nasce de mães adolescentes no Brasil</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">400 mil</div>
                <div class="stat-label">casos por ano de gravidez na adolescência</div>
            </div>
            <div class="stat-item">
                <div class="stat-number">3x mais</div>
                <div class="stat-label">chance de mortalidade materna em adolescentes</div>
            </div>
        </div>
        
        <div class="form-container">
            <form id="pesquisaGravidez">
                <!-- Pergunta 1 -->
                <div class="form-group">
                    <label class="required">1. Qual sua idade?</label>
                    <input type="number" name="idade" min="12" max="24" required>
                </div>
                
                <!-- Pergunta 2 -->
                <div class="form-group">
                    <label class="required">2. Você já recebeu educação sexual na escola?</label>
                    <div class="radio-group">
                        <div class="option">
                            <input type="radio" id="educacao1" name="educacao" value="regularmente" required>
                            <label for="educacao1">Sim, regularmente</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="educacao2" name="educacao" value="uma_vez">
                            <label for="educacao2">Sim, mas apenas uma vez</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="educacao3" name="educacao" value="nunca">
                            <label for="educacao3">Não, nunca</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="educacao4" name="educacao" value="nao_sei">
                            <label for="educacao4">Não tenho certeza</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 3 -->
                <div class="form-group">
                    <label class="required">3. Na sua opinião, quais são as principais causas da gravidez na adolescência no Brasil? (Selecione até 3)</label>
                    <div class="checkbox-group">
                        <div class="option">
                            <input type="checkbox" id="causa1" name="causas" value="falta_info">
                            <label for="causa1">Falta de informação sobre métodos contraceptivos</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="causa2" name="causas" value="acesso_saude">
                            <label for="causa2">Dificuldade de acesso a serviços de saúde</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="causa3" name="causas" value="pressao_parceiro">
                            <label for="causa3">Pressão do parceiro(a)</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="causa4" name="causas" value="falta_perspectiva">
                            <label for="causa4">Falta de perspectiva de futuro</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="causa5" name="causas" value="midia">
                            <label for="causa5">Influência da mídia/redes sociais</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="causa6" name="causas" value="abuso">
                            <label for="causa6">Abuso sexual</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="causa7" name="causas" value="dialogo_familiar">
                            <label for="causa7">Falta de diálogo familiar</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 4 -->
                <div class="form-group">
                    <label class="required">4. Como você avalia o acesso a métodos contraceptivos para adolescentes no SUS?</label>
                    <div class="radio-group">
                        <div class="option">
                            <input type="radio" id="acesso1" name="acesso" value="facil" required>
                            <label for="acesso1">Fácil e gratuito</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="acesso2" name="acesso" value="barreiras">
                            <label for="acesso2">Disponível, mas com barreiras</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="acesso3" name="acesso" value="dificil">
                            <label for="acesso3">Difícil e limitado</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="acesso4" name="acesso" value="nao_sei">
                            <label for="acesso4">Não sei informar</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 5 -->
                <div class="form-group">
                    <label class="required">5. Na sua comunidade, adolescentes grávidas recebem:</label>
                    <div class="radio-group">
                        <div class="option">
                            <input type="radio" id="apoio1" name="apoio" value="apoio" required>
                            <label for="apoio1">Apoio familiar e social</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="apoio2" name="apoio" value="preconceito">
                            <label for="apoio2">Algum apoio, mas com preconceito</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="apoio3" name="apoio" value="julgamento">
                            <label for="apoio3">Pouco apoio e muito julgamento</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="apoio4" name="apoio" value="rejeicao">
                            <label for="apoio4">Rejeição familiar e social</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 6 -->
                <div class="form-group">
                    <label>6. Quais as principais consequências da gravidez precoce que você observa? (Selecione até 3)</label>
                    <div class="checkbox-group">
                        <div class="option">
                            <input type="checkbox" id="consequencia1" name="consequencias" value="abandono_escolar">
                            <label for="consequencia1">Abandono escolar</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="consequencia2" name="consequencias" value="dificuldades_financeiras">
                            <label for="consequencia2">Dificuldades financeiras</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="consequencia3" name="consequencias" value="problemas_saude">
                            <label for="consequencia3">Problemas de saúde</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="consequencia4" name="consequencias" value="conflitos_familiares">
                            <label for="consequencia4">Conflitos familiares</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="consequencia5" name="consequencias" value="limitacao_oportunidades">
                            <label for="consequencia5">Limitação de oportunidades</label>
                        </div>
                        <div class="option">
                            <input type="checkbox" id="consequencia6" name="consequencias" value="depressao">
                            <label for="consequencia6">Depressão/ansiedade</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 7 -->
                <div class="form-group">
                    <label class="required">7. Você conhece os direitos das adolescentes grávidas no Brasil (como permanência na escola, pré-natal, etc)?</label>
                    <div class="radio-group">
                        <div class="option">
                            <input type="radio" id="direitos1" name="direitos" value="bem" required>
                            <label for="direitos1">Sim, conheço bem</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="direitos2" name="direitos" value="alguns">
                            <label for="direitos2">Conheço alguns</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="direitos3" name="direitos" value="pouco">
                            <label for="direitos3">Conheço muito pouco</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="direitos4" name="direitos" value="nao">
                            <label for="direitos4">Não conheço</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 8 -->
                <div class="form-group">
                    <label>8. Qual a principal fonte de informação sobre sexualidade para os jovens na sua região?</label>
                    <div class="radio-group">
                        <div class="option">
                            <input type="radio" id="fonte1" name="fonte" value="escola">
                            <label for="fonte1">Escola</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="fonte2" name="fonte" value="familia">
                            <label for="fonte2">Família</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="fonte3" name="fonte" value="amigos">
                            <label for="fonte3">Amigos</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="fonte4" name="fonte" value="internet">
                            <label for="fonte4">Internet/redes sociais</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="fonte5" name="fonte" value="saude">
                            <label for="fonte5">Unidades de saúde</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="fonte6" name="fonte" value="nenhuma">
                            <label for="fonte6">Não há informação</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 9 -->
                <div class="form-group">
                    <label class="required">9. Você acredita que programas sociais como o Bolsa Família influenciam na gravidez adolescente?</label>
                    <div class="radio-group">
                        <div class="option">
                            <input type="radio" id="programas1" name="programas" value="incentivam" required>
                            <label for="programas1">Sim, incentivam</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="programas2" name="programas" value="nao_influenciam">
                            <label for="programas2">Não influenciam</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="programas3" name="programas" value="ajudam">
                            <label for="programas3">Podem ajudar na prevenção</label>
                        </div>
                        <div class="option">
                            <input type="radio" id="programas4" name="programas" value="nao_sei">
                            <label for="programas4">Não sei opinar</label>
                        </div>
                    </div>
                </div>
                
                <!-- Pergunta 10 -->
                <div class="form-group">
                    <label>10. Que medidas seriam mais eficazes para reduzir a gravidez na adolescência no Brasil?</label>
                    <textarea name="medidas" placeholder="Sugira ações e políticas..."></textarea>
                </div>
                
                <button type="submit">Enviar Respostas</button>
            </form>
        </div>
        
        <footer>
            <p>Pesquisa desenvolvida para fins educacionais - Dados do Brasil: 1 em cada 5 bebês nasce de mães adolescentes (Fonte: Ministério da Saúde)</p>
            <p>© 2023 - Todos os direitos reservados</p>
        </footer>
    </div>

    <script>
        document.getElementById('pesquisaGravidez').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Validação adicional
            let idade = document.querySelector('input[name="idade"]').value;
            if (idade < 12 || idade > 24) {
                alert('Por favor, informe uma idade entre 12 e 24 anos.');
                return;
            }
            
            // Simulação de envio
            alert('Obrigado por participar desta pesquisa importante! Suas respostas foram registradas.');
            
            // Aqui normalmente enviaria os dados para um servidor
            // this.reset(); // Limpa o formulário após envio
        });
    </script>
</body>
</html>
