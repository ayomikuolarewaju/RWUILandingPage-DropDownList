<script> 
       import img13 from '../img/image-hero-desktop.png';
       import img14 from '../img/image-hero-mobile.png';
       import img2 from '../img/client-databiz.svg';
       import img1 from '../img/client-audiophile.svg';
       import img3 from '../img/client-maker.svg';
       import img4 from '../img/client-meet.svg';
    </script>
    
    <div class="container flex flex-col-reverse md:flex md:flex-row mx-auto items-center space-x-10">
        <div class="flex flex-col w-2/3 p-2 mt-5 items-start">
                <div class=" space-y-4 p-4 mt-5">
                    <h4 class="hidden text-black md:text-7xl font-bold md:flex">Make <br>Remote Work</h4>
                    <h4 class="text-black text-2xl font-bold hidden">Make Remote Work</h4>
                </div>
                <div class="space-y-4 p-4 mt-3 w-2/3">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.
                         Hic deserunt commodi soluta inventore quos,
                         unde architecto quisquam aperiam velit dolor 
                         sequi.
                    </p>
                </div>
                <div class="space-y-4 p-4 mt-3 w-3/3 ">
                    <button class="p-3 text-black text-xl font-bold border-solid border-black border-2 rounded-md">
                        Learn More
                    </button>
                </div>
                <div class="flex flex-row text-left space-x-10 mt-20">
                    <div>
                        <img src="{img2}" alt="" width="100" height="100">
                    </div>
                    <div>
                        <img src="{img1}" alt="" width="100" height="100">
                    </div>
                    <div>
                        <img src="{img3}" alt="" width="100" height="100">
                    </div>
                    <div>
                        <img src="{img4}" alt="" width="100" height="100">
                    </div>

                </div>
                
        </div>
        <div class="w-2/3 p-2 overflow-hidden">
            <div>
                <img src="{img13}" alt="" srcset="" class="hidden md:flex" width="400" height="400">
                <img src="{img14}" alt="" srcset="" class="md:hidden" width="400" height="400">
            </div>
        </div>
    </div>