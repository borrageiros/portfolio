<div id="content">
    <div class="info">
        <h1 class="name">Adrián Borrageiros Mourelos, <span id="years"></span>  years old</h1>
        <h2 class="who">Full stack developer from Spain</h2>
        <script> 
            function getAge(dateString) {
                var today = new Date();
                var birthDate = new Date(dateString);
                var age = today.getFullYear() - birthDate.getFullYear();
                var m = today.getMonth() - birthDate.getMonth();
                if (m < 0 || (m === 0 && today.getDate() < birthDate.getDate())) {
                    age--;
                }
                return age;
            }
            var years = document.getElementById('years');
            years.innerHTML = getAge("1999/04/26");
        </script>
    </div>
</div>