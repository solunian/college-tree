<script>
    import duck from '$lib/images/duck.jpg';
</script>

<head>
	<title>About Me</title>
</head>

<div class="container">
    <img alt="The project logo" src={duck} />
    <h1>Our Team</h1>
    <p>Hello, we are Daniel Cui, Bhargav Eranki, Prashant Kondayapalepu, Shine Chang. </p>
    <p>Feel free to get in touch with me at [insert email or social media links here].</p>
</div>




<style>
    body {
        font-family: Arial, sans-serif;
        background-color: rgb(15, 30, 231);
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