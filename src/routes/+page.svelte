<script>
    let birthDate = new Date("1999/04/26");

    function getAge(date) {
        const today = new Date();
        let age = today.getFullYear() - date.getFullYear();
        const m = today.getMonth() - date.getMonth();
        if (m < 0 || (m === 0 && today.getDate() < date.getDate())) {
            age--;
        }
        return age;
    }

    $: age = getAge(birthDate);
</script>

<div class="content">
    <div class="info">
        <div class="whoiam">
            <span style="color:red">&#123;<br/></span>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color:yellowgreen">name:</span>&nbsp;"Adrián Borrageiros Mourelos",<br/>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color:yellowgreen">age:</span><span style="color:red">&nbsp;{age}</span>,<br/>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color:yellowgreen">country:</span>&nbsp;"Spain",<br/>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color:yellowgreen">job:</span>&nbsp;"Full stack developer",<br/>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color:yellowgreen">email:</span>&nbsp;"<a href="mailto:adrianborrageirosmourelos@gmail.com">adrianborrageirosmourelos@gmail.com</a>",<br/>
            &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span style="color:yellowgreen">currentJob:</span>&nbsp;"<a href="https://www.netexlearning.com/">NetexLearning</a>"<br/>
            <span style="color:red">&#125;<br/></span>
        </div>        
    </div>
</div>

<style>
    .info {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 70vh;
        width: 60vw;
    }
    .whoiam {
        white-space: nowrap;
        font-size: 1.5rem;
        padding: 30px;
    }
    .whoiam > span{
        white-space: nowrap;
    }
    @media (max-width: 767px) {
        .whoiam {
            display: none;
        }
    }
</style>