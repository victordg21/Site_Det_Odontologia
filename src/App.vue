<script setup lang="ts">

let faq1: boolean = false
const number1: number = 1
let faq2: boolean = false
const number2: number = 2
let faq3: boolean = false
const number3: number = 3
let faq4: boolean = false
const number4: number = 4
let faq5: boolean = false
const number5: number = 5
let faq6: boolean = false
const number6: number = 6
let faq7: boolean = false
const number7: number = 7
let faq8: boolean = false
const number8: number = 8


function addOrRemove (faq: boolean, number: number){
    const answer = document.querySelector(`#answer${number}`)
    const question = document.querySelector(`#question${number}`)

    if (faq1 == false){
        //@ts-ignore
        question.classList.add('is-open-question')
        //@ts-ignore
        answer.classList.add('is-open-answer')
        return faq1 = true
    }else{
        //@ts-ignore
        question.classList.remove('is-open-question')
        //@ts-ignore
        answer.classList.remove('is-open-answer')
        return faq1 = false
    }
}

</script>

<template>
    <header class="navbar navbar-expand-lg sticky-top" id="cabecalho">
        <div class="container">
            <img class="navbar-brand" src="./assets/images/Logo.png" alt="Logo da D&T">
            <button class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#menu-navegacao">
                <span class="navbar-toggler-icon"></span>
            </button>
            <nav class="navbar-collapse collapse justify-content-end" id="menu-navegacao">
                <ul class="nav nav-pills d-block d-md-flex">
                    <li class="nav-item">
                        <a class="nav-link fw-bold" href="#quemsomos">Quem Somos</a>
                    </li> 
                    <li class="nav-item">
                        <a class="nav-link fw-bold" href="#dentistas">Dentistas</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link fw-bold" href="#casos">Casos</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link fw-bold" href="#contato">Contato</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
    <div data-bs-spy="scroll" daya-bs-target="cabecalho" data-bs-smooth-scroll="true">
        <section id="quemsomos">
            <div class="container">
                <div class="row imagem-texto">
                    <div class="col-lg-6">
                        <img src="./assets/images/equipe.png" class="d-block w-100" alt="Equipe D&T">
                    </div>
                    <div class="col-lg-6 texto-quemsomos">
                        <h2 class="fw-bold">Quem Somos ?</h2>
                        <p class="fw-bold">
                            A D&T Odontologia foi fundada em 2015, e partiu de uma ideia conjunta do dentista e sócio da empresa, Dr. Douglas em conjunto com sua sócia e dentista Dra. Thais. A ideia tinha como objetivo criar uma sociedade com alguns dentistas com o intuito de trazer felicidade para as pessoas em forma de sorriso
                            e poder realizar um trabalho que consiga trazer transformações para seus pacientes, passando uma experiência única.
                        </p>
                        <p class="fw-bold">
                            Ao longo dos anos a clínica odontológica foi crescendo e conseguindo espalhar seu objetivo de transformar não apenas sorrisos, mas sim vidas.
                            A D&T Odontologia trabalha em diversas áreas, com um grande enfoque na parte estética, na confecção das famosas lentes de contatos dentais como seu principal produto. 
                        </p>
                        <p class="fw-bold">
                            A empresa vem crescendo ao longo dos anos e cada vez mais chama a atenção das pessoas, que vem de todo o Brasil em busca
                            da sua transformação e experiência única, pois a D&T também promove um ambiente de trabalho muito profissional, mas que acima
                            de tudo cria laços com seus pacientes, facilitando todo o trabalho e promovendo uma experiência inigualável.
                        </p>
                    </div>
                </div>
            </div>
        </section>
        <section id="dentistas">
            <div class="container">
                <div class="row">
                    <h2 class="fw-bold">Dentistas</h2>
                </div>
                <div class="row">
                    <div class="col-lg-4 col-md-6">
                        <img src="./assets/images/douglas.jpg" class="d-block-w-100" alt="Dentista Dr. Douglas">
                        <h4 class="fw-bold">Dr.Douglas</h4>
                        <h6>CRO-PB 2927</h6>
                    </div>
                    <div class="col-lg-4 col-md-6">
                        <img src="./assets/images/thais.jpg" class="d-block-w-100" alt="Dentista Dra. Thais">
                        <h4 class="fw-bold">Dra.Thais</h4>
                        <h6>CRO-PB 4556</h6>
                    </div>
                    <div class="col-lg-4 col-md-6">
                        <img src="./assets/images/gustavo.jpg" class="d-block-w-100" alt="Dentista Dr. Gustavo">
                        <h4 class="fw-bold">Dr.Gustavo</h4>
                        <h6>CRO-PB 7906</h6>
                    </div>
                </div>
            </div>
        </section>
        <section id="casos">
            <div class="container">
                <div class="row">
                    <h2 class="fw-bold">Casos</h2>
                </div>
                <div class="row">
                    <div class="carousel slide" data-bs-ride="carousel" id="carousel">
                        <div class="carousel-inner">
                            <div class="carousel-item active" data-bs-interval="3000">
                                <img src="./assets/images/matheus.png" alt="Sorriso de Matheus">
                            </div>
                            <div class="carousel-item" data-bs-interval="3000">
                                <img src="./assets/images/waguinho.png" alt="Sorriso de Waguinho">
                            </div>
                            <div class="carousel-item" data-bs-interval="3000">
                                <img src="./assets/images/mayara.png" alt="Sorriso de Mayara">
                            </div>
                            <div class="carousel-item" data-bs-interval="3000">
                                <img src="./assets/images/sincero.png" alt="Sorriso de Sincero">
                            </div>
                        </div>
                        <button class="carousel-control-prev" type="button" data-bs-target="#carousel" data-bs-slide="prev">
                            <span class="carousel-control-prev-icon"></span>
                        </button>
                        <button class="carousel-control-next" type="button" data-bs-target="#carousel" data-bs-slide="next">
                            <span class="carousel-control-next-icon"></span>
                        </button>
                        <div class="carousel-indicators">
                            <button type="button" data-bs-target="#carousel" class="active" data-bs-slide-to="0"></button>
                            <button type="button" data-bs-target="#carousel" data-bs-slide-to="1"></button>
                            <button type="button" data-bs-target="#carousel" data-bs-slide-to="2"></button>
                            <button type="button" data-bs-target="#carousel" data-bs-slide-to="3"></button>
                        </div>
                    </div>
                </div>
                <div class="row referencia">
                        <a href="./casos.html" class="nav-link fw-bold casos-vermais">Ver mais</a>
                </div>
            </div>
        </section>
        <section id="contato">
            <div class="container">
                <div class="row">
                    <h2 class="fw-bold">Contato</h2>
                </div>
                <div class="row">
                    <h3>Telefone</h3>
                    <h5 class="numero-telefone">(83)3244-4450</h5>
                    <h3>Redes Sociais</h3>
                    <ul class="social-links">
                        <li class="fs-5">
                            <a href="https://www.facebook.com/profile.php?id=100063776628574&mibextid=LQQJ4d">
                                <i class="bi bi-facebook cor-logos"></i>
                            </a>
                        </li>
                        <li class="fs-5">
                            <a href="https://api.whatsapp.com/send/?phone=5583987661600&text&type=phone_number&app_absent=0">
                                <i class="bi bi-whatsapp cor-logos"></i>
                            </a>
                        </li>
                        <li class="fs-5">
                            <a href="https://www.instagram.com/det_odontologia/">
                                <i class="bi bi-instagram cor-logos"></i>
                            </a>
                        </li>
                    </ul>
                    <h3>Endereço</h3>
                    <h5> Av. Monteiro da Franca, 659 - Loja 15 - Manaíra, João Pessoa - PB, 58038-320</h5>
                </div>
            </div>
        </section>
        <section id="perguntas">
            <div class="container">
                <h2 class="fw-bold">Perguntas Frequentes</h2>
                <ul class="faq-questions">
                    <li @click="addOrRemove(faq1, number1)" class="faq-questions-item">
                        <div class="question" id="question1">
                            Quanto tempo em média duram as lentes de contato?
                        </div>
                        <div class="answer" id="answer1">
                            Com os devidos cuidados, higiene correta e realizando as manutenções, a duração é de cerca de 15 a 20 anos.
                        </div>
                    </li>
                    <li @click="addOrRemove(faq2, number2)" class="faq-questions-item">
                        <div class="question" id="question2">
                            As lentes de contato ficam amareladas com o tempo tomando bebidas com corantes?
                        </div>
                        <div class="answer" id="answer2">
                            Não, as lentes de contato tem uma superfície muito selada devido ao processo de cristalização no forno, que
                            vai a uma temperatura de mais de 800. Portanto, as lentes não sofrem alteração com o passar do tempo.
                        </div>
                    </li>
                    <li @click="addOrRemove(faq3, number3)" class="faq-questions-item">
                        <div class="question" id="question3">
                            É necessária a manutenção das lentes?
                        </div>
                        <div class="answer" id="answer3">
                            Sim, assim como os dentes naturais, com as lentes são necessárias uma ou duas visitas ao ano para realizar uma
                            limpeza e verificar se está tudo bem.
                        </div>
                    </li>
                    <li @click="addOrRemove(faq4, number4)" class="faq-questions-item">
                        <div class="question" id="question4">
                            Os dentes são desgastados para colocar as lentes?
                        </div>
                        <div class="answer" id="answer4">
                            Sim, os dentes são desgastados em 99% dos casos, porém somente o mínimo necessário. Desgastes minimamente invasivos.
                        </div>
                    </li>
                    <li @click="addOrRemove(faq5, number5)" class="faq-questions-item">
                        <div class="question" id="question5">
                            Vocês colocam aparelho?
                        </div>
                        <div class="answer" id="answer5">
                            Sim, a clínica também realiza o trabalho ortodôntico.
                        </div>
                    </li>
                    <li @click="addOrRemove(faq6, number6)" class="faq-questions-item">
                        <div class="question" id="question6">
                            O valor é de todo o sorriso ou por lente?
                        </div>
                        <div class="answer" id="answer6">
                            O valor é calculado por lentes.
                        </div>
                    </li>
                    <li @click="addOrRemove(faq7, number7)" class="faq-questions-item">
                        <div class="question" id="question7">
                            Vocês colocam implantes?
                        </div>
                        <div class="answer" id="answer7">
                            Sim, na clínica colocamos implantes, coroas, lentes de contato, ponte fixa e além disso trabalhamos com a parte ortodôntica.
                        </div>
                    </li>
                    <li @click="addOrRemove(faq8, number8)" class="faq-questions-item">
                        <div class="question" id="question8">
                            É necessário colocar aparelho antes de por as lentes?
                        </div>
                        <div class="answer" id="answer8">
                            Em alguns casos é sim preciso, sendo muito de cada caso a depender de como os dentes possam estar posicionados, acaba sendo
                            necessária a parte ortodôntica antes das lentes de contato.
                        </div>
                    </li>
                </ul>
            </div>
        </section>
        <footer>
            <div class="container">
                <p class="fw-bold">
                    &copy; D&T Odontologia - Todos os direitos reservados - 2023
                </p>
            </div>
        </footer>
    </div>
</template>
<style scoped>
    *{
    font-family: 'Montserrat', sans-serif;
}

body{
    background-color: #ebdbc2;
}

header img{
    height: 120px;
}

.navbar{
    background-color: #ebdbc2;
}

.nav .nav-link.active{
    background-color: #2B4257;
    color: #ebdbc2;
}

.nav .nav-link,
.navbar-brand{
    color: #2B4257;
}

section{
    padding: 16px;
}

#perguntas h2{
    margin-bottom: 32px;
}

#quemsomos,
#casos,
#casos-pp2,
#perguntas{
    background-color: #03273d;
    color: #ebdbc2;
}

#dentistas,#contato{
    background-color: #2B4257;
    color: #ebdbc2;
}

#quemsomos p{
    font-size: 13px;
    margin-bottom: 4px;
}

#dentistas img{
    height: 400px;
}

#dentistas h4{
    margin-top: 8px;
    margin-bottom: 2px;
}

section img,
#casos-pp2 img{
    border-radius: 12px;
}

#casos img{
    width: 70%;
    display: block;
    margin: 0 auto;
}

.referencia{
    margin-top: 32px;
}

.referencia a{
    text-align: center;
    background-color: #ebdbc2;
    padding: 8px 0px;
    color: #03273d;
    border-radius: 6px;

}

.referencia a:hover{
    color: #03273d;
    background-color:#ebdbc2 ;
}

#contato h3{
    margin-top: 32px;
    margin-bottom: 16px;
}

.social-links li{
    list-style: none;
    display: inline;
    margin-right: 4px;

}

.social-links a{
    text-decoration: none;
}

.cor-logos{
    color: #ebdbc2;
}

footer{
    background-color: #ebdbc2;
    color: #2C4257;
    padding: 8px 0px;
}

#dentistas h2,
#casos h2{
    margin-bottom: 32px;
}

.casos-vermais{
    width: 70%;
    display: block;
    margin: 0 auto;
}

.faq-questions{
    padding: 0;
}
.faq-questions-item{
    background-color: #2B4257;
    list-style: none;
    margin-bottom: 16px;
}

.question{
    font-size: 20px;
    padding: 24px;
    display: block;
    cursor: pointer;
    font-weight: bold;
    position: relative;
}

.question::after{
    content: '+';
    position: absolute;
    top: 0;
    right: 24px;
    height: 100%;
    display: flex;
    align-items: center;
    font-size: 40px;
}

.is-open-question::after{
    content: '-';
}
.answer{
    background-color: #ebdbc2;
    color:#03273d;
    font-weight: bold;
    font-size: 20px;
    height: 0px;
    overflow: hidden;
}

.is-open-answer{
    height: auto;
    padding: 24px;
}

footer p{
    margin: 8px 0px;
}

.numero-telefone{
    text-decoration: none;
    color: #ebdbc2;
}

#casos-pp2 img{
    margin: 32px 0px;
}

.button-respostas{
    background-color: #ebdbc2;
    color: #2C4257;
}

@media (max-width: 767px){
    
    #quemsomos h2{
        margin: 8px 0px;
    }

    #dentistas h6{
        margin-bottom: 32px;
    }

    #casos img{
        width: 100%;
    }

    .numero-telefone{
        text-decoration: none;
        color: #ebdbc2;
    }

    #dentistas h2,
    #casos h2,
    #casos-pp2 h2,
    #dentistas h4,
    #dentistas h6,
    #contato h2{
        text-align: center;
    }

    #dentistas img{
        display: block;
        margin: 0 auto;
    }

    .casos-vermais{
        width: 95%;
    }

    .question{
        font-size: 18px;
        padding-right: 40px;
    }
    .question::after{
        right: 12px;
    }

}

@media (min-width: 768px) and (max-width: 1023px){

    #quemsomos h2{
        margin: 16px 0px;
    }

    #quemsomos p{
        font-size: 18px;
    }

    #dentistas h6{
        margin-bottom: 32px;
    }

    #casos img{
        width: 100%;
    }

    .numero-telefone{
        text-decoration: none;
        color: #ebdbc2;
    }

    .casos-vermais{
        width: 95%;
    }

    .question{
        padding-right: 80px;
    }
}

</style>
