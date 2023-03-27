<script>
    import duck from '$lib/images/duck.jpg';
</script>



<div class="container">
    <h1 class="text-3xl my-8">
        About
    </h1>
    <img alt="The project logo" src={duck} />
    <h1 class='pt-3'>How we achieved this</h1>
    <p>Hello, we are Daniel Cui, Bhargav Eranki, Prashant Kondayapalepu, and Shine Chang from Cupertino High School. Our goal is help high schools students find activities related to their career path in order to help them better prepare for college. Many high school students avoid prestigious oppurtunities because of the lack of information. Our website helps these high school students connect to different posts and become better connected to the community. </p>
    <p>This project was made using firebase, tailwindcss, express, and sveltekit. {"😁"}</p>
</div>




<style>
    body {
        font-family: Arial, sans-serif;
        background-color: rgb(24, 35, 198);
    }

    h1 {
        color: #333333;
        text-align: center;
    }

    .container {
        max-width: 600px;
        margin: 3rem;
        padding: 20px;
        background-color: #ffffff;
        border-radius: 10px;
        box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
    }

    img {
        display: block;
        margin: 0 auto;
        width: 200px;
        border-radius: 20%;
    }

    p {
        margin-top: 20px;
        padding: 0 3rem;
        line-height: 1.5;
        text-align: center;
    }
</style>