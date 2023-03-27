<script>
    import Graduation from '$lib/images/Grad.png';
    import CollegeTreeThing from '../lib/components/CollegeTreeThing.svelte';
</script>


<div>
    <img alt="The project logo" src={Graduation} class="w-full p-0 -z-20" />
    <CollegeTreeThing/>
    
    <div class="px-56 pt-5">
        <div class="flex flex-col gap-4">
            <h1 class="text-3xl my-5">
              Branch out with <b class="text-purple-900">college tree</b>!
            </h1>
            <h2 class="text-2xl">Mission Statement</h2>
            <p>Our mission is to connect high school students with oppurtunities related to their career choices. Many high school students lack the oppurtunity to participate in activites because they simply can't find anything that fits their future career. College Tree targets these individuals and helps them by connecting them to events in relation to their interests. We acheived this by using a database with stores information of the user and searches based on their characteristics.</p>
            <p>By connecting high school students with topics that they are interested in, we believe they have a better chance in getting into the college of their choice. </p>
        </div>

    </div>
</div>
