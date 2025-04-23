<template>
    <section class="container-fluid pt-4" id="news-area">
        <div class="col-md-12">
            <h3 class="main-title">Fique por dentro das nossas novidades</h3>
        </div>
        <p>Assine nossa lista de e-mails, e receba nossos conteúdos sobre desenvolvimento de software</p>
        <form action="">
            <input type="email" name="email" id="email-input" class="form-control" placeholder="Digite seu email">
            <input type="submit" value="Inscrever" id="news-btn">
        </form>

        <div id="call-area">
            <div class="container">
                <div class="row">
                    <p>Deseja fazer um orçamento sem compromisso?</p>
                    <button class="rounded-5 p-3" id="call-btn">Orçar</button>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
#news-area {
    text-align: center;
    background-color: #F9F9F9;
}

#news-area p {
    font-size: 18px;
    margin-bottom: 40px;
}

#email-input {
    border-radius: 0;
    border-top-left-radius: 20px;
    border-bottom-left-radius: 20px;
    border: 1px solid #65DAF9;
    display: inline;
    box-sizing: border-box;
    width: 40%;
    height: 40px;
}

#news-btn {
    border-top-right-radius: 20px;
    border-bottom-right-radius: 20px;
    border: 1px solid #65DAF9;
    background-color: #65DAF9;
    color: #FFF;
    text-transform: uppercase;
    height: 40px;
    padding: 0 30px;
    margin-left: -130px;
    position: absolute;
    transition: .5s;
}

#news-btn:hover {
    background-color: #FFF;
    color: #65DAF9;
}

#call-area {
    margin-top: 60px;
    background-color: #65DAF9;
    text-transform: uppercase;
}

#call-area .container {
    padding: 40px 100px;
}

#call-area .row {
    display: block;
    text-align: center;
}

#call-area p {
    color: #FFF;
    font-weight: bold;
    font-size: 20px;
    margin-bottom: 0;
    height: 60px;
    line-height: 60px;
    letter-spacing: 2px;
    display: inline;
}

#call-area #call-btn {
    border:none;
    background-color: #FFF;
    color: #65DAF9;
    font-weight: bold;
    margin-left: 30px;
    font-size: 20px;
    width: auto;
    letter-spacing: 2px;
}
</style>