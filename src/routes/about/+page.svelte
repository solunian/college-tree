<script>
    import duck from '$lib/images/duck.jpg';
</script>

<head>
	<title>About Me</title>
</head>

<div class="container">
    
    <!-- svelte-ignore missing-declaration -->
    <img alt="The project logo" src={duck} />
    <h1>Our Goal</h1>
    <p>Hello, we are Daniel Cui, Bhargav Eranki, Prashant Kondayapalepu, and Shine Chang from Cupertino High School. Our goal is help high schools students find activities related to their career path in order to help them better prepare for college. Many high school students avoid prestigious oppurtunities because of the lack of information. Our website helps these high school students connect to different posts and become better connected to the community. </p>
    <p>By connecting high school students with topics that they are interested in, we believe they have a better chance in getting into the college of their choice. </p>
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
        margin: 0 auto;
        padding: 20px;
        background-color: #ffffff;
        border-radius: 10px;
        box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
    }

    img {
        display: block;
        margin: 0 auto;
        width: 200px;
        border-radius: 50%;
    }

    p {
        margin-top: 20px;
        line-height: 1.5;
        text-align: justify;
    }
</style>