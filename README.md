# aula-5-melhorado
<section id="tropicalia" class="my-5 pt-6 secao-tropicalia">
        <div class="container d-flex align-items-center ">
                <div class="col-5">
                        <h2>O que foi a Tropicália?</h2>
                        <p class="p-2">A Tropicália, também conhecida como Tropicalismo, foi um movimento cultural
                                brasileiro que surgiu na década de 1960, tendo seu auge entre 1967 e 1968. Esse movimento
                                abrangeu várias expressões artísticas, como a música, o cinema, o teatro e as artes plásticas, e
                                teve como principal característica a mistura de elementos da cultura brasileira tradicional com
                                influências estrangeiras, especialmente do rock e da música pop. Fonte: Site Toda Matéria</p>
                </div>
        </div>
</section>
<section id="inicio" class="my-5">
        <div class="inicio-fundo d-flex justify-content-between align-items-center">
                <div class="esquerda-conteudo">
                        <h1 class="display-4 text-white fst-italic fw-bold">Boas-vindas a</h1>
                        <img src="img/logo-2.png" class="mb-3" width="563"
                                height="278" loading="lazy">
                        <a href="#tropicalia"
                                class="btn btn-primary btn-lg botao-inicio fw-semibold">Quero conhecer!</a>
                </div>
                <img src="img/lossy-page1-640px-Os_Mutantes.tif (1).png" alt="A imagem apresenta o grupo musical Os mutantes, sao tres pessoas cantando em  dois microfones" title="Os mutantes - CC0 Domínio Público / Acervo Arquivo Nacional" class="img-fluid img-inicio">
            </div>
</section>
                                teve como principal característica a mistura de elementos da cultura brasileira tradicional com
                                influências estrangeiras, especialmente do rock e da música pop. Fonte: Site Toda Matéria</p>
                </div>
        </div>
</section>
<body>
    <header class=" p-5">
        
        <nav class="container d-flex justify-content-between align-items-center" >
            <img src="img/logo.png" class="nav-img" loading="lazy">
            <ul class="nav mt-5">
                <li class="nav-item"><a class="nav-link" href="#inicio">Início</a></li>
                <li class="nav-item"><a class="nav-link" href="#galeria">Galeria</a></li>
                <li class="nav-item"><a class="nav-link" href="#contato">Contato</a></li>
            </ul>
                <div id="acessibilidade">
                    <button id="aumentar-fonte" class="btn btn-primary fw-bold">A+</button>
                    <button id="diminuir-fonte" class="btn btn-primary fw-bold">A-</button>
                </div>
        </nav>
</header>
.menu-acessibilidade{
    position: fixed;
    top:2rem;
    right:20px;
    z-index: 1000;
}
.rotacao-botao{
    transform: rotate(-90deg);
    transform-origin: right center;
}
.opcoes-acessibilidade{
    margin-top:10px;
    display: flex;
    flex-direction: column;
}
.opcoes-acessibilidade button{
    margin-bottom: 5px;
}
.apresenta-lista{
    display: none;
}
document.addEventListener('DOMContentLoaded', function(){
    const aumentaFonteBotao document.getElementById('aumentar-fonte');
    const diminuiFonteBotao document.getElementById('diminuir-fonte');

    let tamanhoAtualFonte = 1;
    aumentaFonteBotao.addEventListener('click', function(){
        tamanhoAtualFonte += 0.1;
        document.body.style.fontSize = `${tamanhoAtualFonte}rem`

    })

    diminuiFonteBotao.addEventListener('click', function(){
        tamanhoAtualFonte -= 0.1;
        document.body.style.fontSize = `${tamanhoAtualFonte}rem`

    })
})
const botaoDeAcessibilidade = document.getElementById('botao-acessibilidade')
const opcoesDeAcessibilidade = document.getElementById('opcoes-acessibilidade')
botaoDeAcessibilidade.addEventListener('click', function (){
 botaoDeAcessibilidade.classList.toggle('rotacao-botao');
 opcoesDeAcessibilidade.classList.toggle('apresenta-lista')
})
