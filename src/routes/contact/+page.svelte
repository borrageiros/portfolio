<style>
    .content{
        right: 5%;
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
<div id="content">
    <div class="content">

        <h3>Contact</h3>
        <hr><br><br>
        <p>I’m currently looking for any new opportunities,<br> my inbox is always open. <br> Whether you have a question or just want to say hi, I’ll try my best to get back to you!</p>
        
        <h3 style="margin-top: 5vh;">Email</h3>
        <hr><br><br>
        <div class="email">
            <button onclick="navigator.clipboard.writeText('adrianborrageirosmourelos@gmail.com');alert('Email copied')"><img src="/copy.png" alt="ClipBoard"></button>
            <p>adrianborrageirosmourelos@gmail.com</p>
        </div>
        <br><br><hr>
        <div class="buttons">
            <a href="mailto:email@example.com"><button>SEND MAIL</button></a>
            <a href="/whatsapp"><button>WHATSAPP</button></a>
        </div>
    </div>
</div>