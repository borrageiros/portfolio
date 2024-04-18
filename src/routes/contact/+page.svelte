<div class="content">

    <h1>Contact</h1>
    <hr><br><br>
    <p class="info">I’m currently looking for any new opportunities,<br> my inbox is always open. <br> Whether you have a question or just want to say hi, I’ll try my best to get back to you!</p>
    
    <h1>Email</h1>
    <hr><br><br>
    <div class="email">
        <button onclick="navigator.clipboard.writeText('adrianborrageirosmourelos@gmail.com');alert('Email copied')"><img src="/copy.png" alt="ClipBoard"></button>
        <p>adrianborrageirosmourelos@gmail.com</p>
    </div>
    <br><br><hr>
    <div class="buttons">
        <a href="mailto:adrianborrageirosmourelos@gmail.com"><button>SEND MAIL</button></a>
        <a href="/whatsapp"><button>WHATSAPP</button></a>
    </div>
</div>
<style>
    @media only screen and (max-width: 768px) {
        .content{
            margin-top: 15vh;
        }
    }

    .info{
        margin-left: 5vh;
        margin-bottom: 5vh;
    }

    .buttons button{
        background-color: #1e1e1e;
        border: 2px solid white;
        border-radius: 25px;
        padding: 1%;
        margin: 3vh;
    }
    .buttons button:hover{
        border: 2px solid greenyellow;
        color: greenyellow;
        cursor: pointer;
    }

    .email{
        display: flex;
        align-items: center;
        margin-left: 5vh;
    }
    .email button{
        background-color: transparent;
        border: none;
        width: 5%;
    }
    .email p{
        margin-left: 1%;
    }
    .email img{
        width: 100%;
    }
    .email img:hover{
        content: url("/copy_hover.png");
        cursor: pointer;
    }
</style>