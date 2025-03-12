<nav class="container d-flex justify-content-between align-items-center">
    <img src="img/logo.png" class="nav-img" loading="lazy">
    <ul class="nav mt-5">
        <li class="nav-item"><a class="nav-link" href="#inicio">Início</a></li>
        <li class="nav-item"><a class="nav-link" href="#galeria">Galeria</a></li>
        <li class="nav-item"><a class="nav-link" href="#contato">Contato</a></li>
    </ul>
    <div id="acessibilidade" class="menu-acessibilidade">
        <button id="botao-acessibilidade" class="btn btn-primary fw-bold rotacao-botao" aria-expanded="false">
            Acessibilidade
        </button>
        <div id="opcoes-acessibilidade">
            <button id="aumentar-fonte" class="btn btn-primary fw-bold">A+</button>
            <button id="diminuir-fonte" class="btn btn-primary fw-bold">A-</button>
        </div>
    </div>
</nav>
document.addEventListener('DOMContentLoaded', function() {
    const aumentaFonteBotao = document.getElementById('aumentar-fonte');
    const diminuirFonteBotao = document.getElementById('diminuir-fonte');
    
    let tamanhoAtualFonte = 1;

    aumentaFonteBotao.addEventListener('click', function() {
        tamanhoAtualFonte += 0.1;
        document.body.style.fontSize = `${tamanhoAtualFonte}rem`;
    });

    diminuirFonteBotao.addEventListener('click', function() {
        tamanhoAtualFonte -= 0.1;
        document.body.style.fontSize = `${tamanhoAtualFonte}rem`;
    });
});
<script src="script.js"></script>
