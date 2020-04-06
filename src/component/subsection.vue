<template>
  <div class = "subSection">
    <figure class = "">
        <img src = "../assets/06_Question mark.png">  
    <section>
        <strong>Amanda: Tell us a litte about your company today.</strong>
        <br/><br/>
        <strong class = "Kristi">Kristi:</strong>
        <span>We believe in data demonatization.We believe that when 
            organization and people have access to data,they can make better and
            more impactful product for world.We are on mission to democratize
            data throughout the world and starting with helping organization find and activate their own data. </span>
    </section>
    <section>
        <br/>
        <p class = "midTitle">"We are on a mission to democratize data
        throughout the world and starting with
        helping organization find and active 
        their own data."</p>
        <br/><br/><br/>
        <strong>Amanda: Your humility,positiviy,and focus is incredibily inspiring.How do you
             think about culture?</strong>
        <p>
            <strong class = "Kristi">Kristi:</strong> We as company,created our own values,We use these value to 
            give each other good feedback on a weekly basis.Every Monday we have
            a company stand-up to give updates on business.At the end we wrap up
            with sharing appreciations to each other for living out different values.We also
            use these values to hold each other accountables.Its a great framework to give
            someone feedback by saying."When do.....this is so consistent
            with .... value"
        </p><br/>
        <hr/>
        <span>Kristi is a founder of knowledgeHound.</span><br/>
        <span>To know more about knowledgeHound, visit their <a>Website</a></span>


    </section>
    </figure>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .subSection{
        background-color: #f2f2f2;
    }

    figure > img{
        height: 300px;
    }
    section{
        width: 39%;
        margin : 0 auto;
        text-align: center;
    }
    .midTitle{
        color : #fe5242;
        font-size: 22px;
    }

    .Kristi{
        color : #fe5242;
    }

    @media only screen and (max-width: 768px){
        section{
            width: unset;
        }
        figure{
            margin: 0 20px 0 20px;
        }
    }

</style>