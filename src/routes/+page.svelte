<script>
    import Graduation from '$lib/images/Grad.png';
    import CollegeTreeThing from '../lib/components/CollegeTreeThing.svelte';
    import Niche from '$lib/images/Niche.jpg';
    import UsNews from '$lib/images/usnews.webp';
    import CollegeBoard from '$lib/images/CollegeBoard.png';
</script>


<div>
  <img alt="The project logo" src={Graduation} class="w-full p-0 -z-20" />
  <CollegeTreeThing/>
  
  <div class="px-4 sm:px-8 md:px-36 lg:px-56 pt-5">
      <div class="flex flex-col gap-4">
        <h1 class="text-3xl my-5">
          Branch out with <b class="text-purple-900">college tree</b>!
        </h1>
        <h2 class="text-2xl">Mission Statement</h2>
        <p class="text-xl">Our mission is to connect high school students with opportunities related to their career choices. Many high school students lack the oppurtunity to participate in activites because they simply can't find anything that fits their future career. College Tree targets these individuals and helps them by connecting them to events in relation to their interests. We acheived this by using a database with stores information of the user and searches based on their characteristics.</p>
        <p class="text-xl">By connecting high school students with topics that they are interested in, we believe they have a better chance in getting into the college of their choice. </p>
      </div>
  </div>

  <div class="flex flex-row gap-8 my-20 px-20 items-center">
    <a href="https://www.niche.com" class="flex flex-col items-center">
      <img src={Niche} alt="niche">
      <p>
        Niche is an excellent resource for high schoolers who want to make informed decisions about their academic and career paths. With comprehensive information on schools, majors, and careers, Niche can help you find the right fit for your interests and aspirations. Our website features detailed profiles of colleges and universities, including reviews from students and alumni, as well as data on acceptance rates, average test scores, and more. We also offer resources for exploring majors and careers, such as salary data, job outlooks, and descriptions of typical job duties. With Niche, you can compare schools and majors, get advice on the admissions process, and make informed decisions about your future.
      </p>
    </a>

    <a href="https://www.usnews.com/best-colleges" class="flex flex-col items-center">
      <img src={UsNews} alt="us news" class="w-96 h-56">
      <p>
        US College News is an invaluable resource for high schoolers who are considering their options for higher education. With in-depth coverage of college admissions, financial aid, and academic programs, US College News can help you make informed decisions about your future. Our team of experienced journalists and researchers provides up-to-date information on the latest trends and developments in the world of higher education, making it easy for you to stay ahead of the curve. Whether you're trying to choose the right college, navigate the admissions process, or find ways to finance your education, US College News has the information and insights you need to succeed. So if you're a high schooler who wants to make the most of your college journey, look no further than US College News.
      </p>
    </a>

    <a href="https://www.collegeboard.org" class="flex flex-col items-center">
      <img src={CollegeBoard} alt="college board" class="">
      <p>
        College Board is an essential resource for high schoolers who are planning to pursue higher education. As the organization responsible for administering standardized tests like the SAT and AP exams, College Board has a wealth of resources and information to help students prepare for college. On our website, you can access free test preparation materials, including practice tests, study guides, and sample questions. We also offer tools for finding and applying to colleges, such as our BigFuture platform, which provides personalized college recommendations based on your interests and preferences. Additionally, we offer a range of financial aid and scholarship resources to help make college more affordable. With College Board, you can stay on track for college admissions and take advantage of all the opportunities available to you. 
      </p>
    </a>
  </div>
</div>