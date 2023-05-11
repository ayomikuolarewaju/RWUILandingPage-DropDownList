<script> 
  import img15 from '../img/logo.svg'; 
  import img9 from '../img/icon-menu.svg';
  import img8 from '../img/icon-close-menu.svg';
  import img5 from '../img/icon-arrow-down.svg';
  import img6 from '../img/icon-arrow-up.svg';
  import img7 from '../img/icon-calendar.svg';
   import img10 from '../img/icon-planning.svg';
   import img11 from '../img/icon-reminders.svg';
   import img12 from '../img/icon-todo.svg';
let rev = true;
const reveler = ()=>{
    rev = !rev;
}
let rev2 = true;
const reveler2 = ()=>{
    rev2 = !rev2;
}
let rev3 = true;
const reveler3 = ()=>{
    rev3 = !rev3;
}
</script>



<div class="flex flex-row items-start justify-between mb-2 relative overflow-hidden">
    <div class="flex flex-row space-x-5 ">
        <ul class="flex flex-row space-x-5">
            <li class="flex flex-col"><img src="{img15}" alt="" srcset=""></li>
            <ul class="md:flex md:flex-col space-x-2 hidden">
                <li class="flex flex-col space-x-2" on:click={reveler} on:keydown><a href="/">Features</a></li>
                {#if rev}
                <div class="flex flex-col space-y-2 bg-white shadow-xl rounded-lg p-5">
                    <li class="flex flex-row space-x-3"><img src="{img12}" alt=""><small>Todo list</small></li>
                    <li class="flex flex-row space-x-3"><img src="{img7}" alt=""><small>Calendar</small></li>
                    <li class="flex flex-row space-x-3"><img src="{img11}" alt=""><small>Reminder</small></li>
                    <li class="flex flex-row space-x-3"><img src="{img10}" alt=""><small>Planning</small></li>
                </div> 
                {/if}

            </ul>
            <ul class="md:flex md:flex-col space-x-2 hidden">
                <li class="flex flex-col space-x-2" on:click={reveler2} on:keydown><a href="/">Company</a></li>
                {#if rev2}
                <div class="flex flex-col space-y-2 bg-white shadow-xl rounded-lg p-5">
                    <li class="flex flex-row space-x-3"><small>History</small></li>
                    <li class="flex flex-row space-x-3"><small>Our Team</small></li>
                    <li class="flex flex-row space-x-3"><small>Blog</small></li>
                </div> 
                {/if}

            </ul>
            <li class="md:flex md:flex-col hidden"><a href="/">Career</a></li>
            <li class="md:flex md:flex-col hidden"><a href="/">About</a></li>
        </ul>

    </div>
    <div class="space-x-5 hidden md:flex md:flex-row">
        <a href="/">Login</a>
        <a href="/" class="border-solid border-black border-2 rounded-md p-1">Register</a>
    </div>
    <div class="md:hidden cursor-pointer" on:click={reveler3} on:keydown>
        <img src="{img9}" alt="" srcset="" >
    </div>
</div>

    
{#if rev3}
<div class="container flex flex-col mx-auto justify-between mb-2 absolute bg-white
 z-50 w-2/3 h-full left-40 md:hidden overflow-hidden">
 <div class="flex flex-col space-x-10 space-y-10 ">
    <ul class="flex flex-col space-x-10 space-y-10 md:hidden">
        <li class="p-10"><img src="{img8}" alt="" srcset="" on:click={reveler3} on:keydown></li>
        <ul class="flex flex-col space-x-2">
            <li class="flex flex-col space-x-2" on:click={reveler} on:keydown><a href="/">Features</a></li>
            {#if rev}
            <div class="flex flex-col space-y-2 bg-white shadow-xl rounded-lg p-5">
                <li class="flex flex-row space-x-3"><img src="{img12}" alt=""><small>Todo list</small></li>
                <li class="flex flex-row space-x-3"><img src="{img7}" alt=""><small>Calendar</small></li>
                <li class="flex flex-row space-x-3"><img src="{img11}" alt=""><small>Reminder</small></li>
                <li class="flex flex-row space-x-3"><img src="{img10}" alt=""><small>Planning</small></li>
            </div> 
            {/if}

        </ul>
        <ul class="flex flex-col space-x-2">
            <li class="flex flex-col space-x-2" on:click={reveler2} on:keydown><a href="/">Company</a></li>
            {#if rev2}
            <div class="flex flex-col space-y-2 bg-white shadow-xl rounded-lg p-5">
                <li class="flex flex-row space-x-3"><small>History</small></li>
                <li class="flex flex-row space-x-3"><small>Our Team</small></li>
                <li class="flex flex-row space-x-3"><small>Blog</small></li>
            </div> 
            {/if}

        </ul>
        <li><a href="/">Career</a></li>
        <li><a href="/">About</a></li>
    </ul>

</div>

</div>
{/if}



