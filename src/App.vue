<template>
    <div class="wrapper">
        <nav class="TopFiveSigns">
            <ul>
                <li><a href="https://theastrocodex.com/natal-sun-in-aries/"><img src="./WZodiacs/VioletAries.jpeg"></a></li>
                <li><a href="https://astrostyle.com/virgo-moon-sign/"><img src="./WZodiacs/BlueVirgo.jpeg"></a></li>
                <li><a href="https://www.liveabout.com/scorpio-rising-rising-signs-207036"><img src="./WZodiacs/BlueScorpio.jpeg"></a></li>
                <li><a href="https://www.alwaysastrology.com/leo-midheaven.html"><img src="./WZodiacs/BlueLeo.jpeg"></a></li>
                <li><a href="https://cafeausoul.com/astrology/chart-angles/descendant"><img src="./WZodiacs/VioletTaurus.jpeg"></a></li>
            </ul>
        </nav>
        
        <section class="me">
            <h4 class="Title">Exemplvm Mevm Zodiaci</h4>
            <h5 class="name">Victor Orozco</h5>
        </section>

        <footer class="ending">
            <p>CopyRight &copy; MMXX</p>
        </footer>
    </div>
</template>

<script>
 export default {
  name: 'app',
  components: {

  }
 }
</script>

<style>
    .wrapper {
        display:grid;
        grid-gap:20px;
        background-image:url("./assets/EMZ.jpeg");
        background-repeat: no-repeat;
        background-size: cover;
    }

    .TopFiveSigns{
    }
        .TopFiveSigns ul {
            display: grid;
            grid-gap: 20px;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            list-style: none;
        }

        .TopFiveSigns a {
        }

        .TopFiveSigns img {
            width: 200px;    
            height: 150px;
        }


    .me {
        display: grid;
        grid-gap: 10px;
        grid-template-rows: 15px 20px;

    }


        .me h5{
        font-family: "Times New Roman", "Times";
        text-align: center;
        text-decoration: none;
        color:cornflowerblue
        }

        .me h4 {
        font-family: "Times New Roman", "Times";
        text-align: center;
        text-decoration: none;
        color:cornflowerblue
        }

    .ending p{
        font-family: 'Times New Roman', Times, serif;
        text-align: center;
        color: mediumpurple;
    }
</style>
