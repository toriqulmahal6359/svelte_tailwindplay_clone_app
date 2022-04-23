<script>
    import Card from "../shared/Card.svelte";
    const cardList = [
        {option: "Customizing Your tailwind.config.js file", id: 1},
        {option: "Extracting classes with @apply", id: 2},
        {option: "Code Completion with instant preview", id: 3},
    ]
</script>

<div class="left_side">
    <div class="card-liner">
        <Card>
            <div class="card">
                <div class="header">
                    <img src="img/tailwind_logo.svg" alt="" class="img_process">
                </div>
                <div class="para_1">
                    <span>An advanced online playground for Tailwind CSS, including support for things like:</span>
                </div>
                <div class="list-options">
                    <ul class="tw_options">
                        {#each cardList as list (list.id)}
                            <li class="flex items-center">
                                <svg class="h-6 w-4 flex-none fill-sky-100 stroke-sky-500 stroke-2 tick" stroke-linecap="round" stroke-linejoin="round">
                                    <circle cx="12" cy="12" r="11"></circle>
                                    <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none"></path>
                                </svg>
                                <p class="op_tw">{list.option}</p>
                            </li>
                        {/each}
                    </ul>
                </div>
                <div class="para_2">
                    <p>Perfect for learning how the framework works, prototyping a new idea, or creating a demo to share online.</p>
                </div>
                <div class="hr"><hr></div>
                <div class="card-footer">
                    <b class="f_1">Want to Dig deeper into Tailwind?</b><br>
                    <b class="f_2"><a href="https://tailwindcss.com/docs" style="color:blueviolet">Read The Docs!!</a></b>
                </div>
            </div>
        </Card>
    </div>
</div>


<style>
    @media (min-width: 540px){
        .left_side{
            height: calc(100vh - 50px);
            margin: auto;
            width: 50%;
            padding: 10px;
            position: absolute;
            left: 24%;
            /* top: 0; */
            overflow-x: auto;
            overflow-y: hidden;
        }
        .card-liner{
            background-image: url("/img/beams.jpg");
        }
        /* .card{
            height: 600px;
            width: 60%;
        } */
        .header{
            text-align: center;
        }
        .img_process{
            resize: none;
            height: 25px;
            width: 100%;
            margin-left: -400px;
            padding: 15px;
            /* position: absolute; */
            /* top: 0;
            left: 0; */
        }
        ul{
            list-style: none;
            /* bottom: 25px; */
        }
        .tw_options{
            text-align: left;
        }
        li{
            display: flex;
            align-items: center;
            flex-direction: column;
        }
        .tick{
            position: relative;
            height: 25px;
            display: flex;
            /* left: 50px; */
        }
        .op_tw{
            margin-top: -24px;
            top: 20%;
            padding-left: 50px;
        }
        .items-center{
            display: flex;
            align-items: flex-start;
        }
        .para_1, .para_2{
            resize: none;
            white-space: normal;
            padding: 25px;
            margin-right: 90px;
            text-align: left;
            text-overflow: ellipsis;
            position: relative;
        }
        /* .para_2{
            margin-top: 100px;
        } */
        .card-footer{
            text-align: left;
            margin: 10px 0px 5px;
            padding: 20px 0 5px;
        }
        .f_1, .f_2{
            resize: none;
            margin-left: 25px;
            margin-top: 10px;
            white-space: normal;
            text-overflow: ellipsis;
        }
        .stroke-2 {
            stroke-width: 2;
        }
        .stroke-sky-500 {
            stroke: #0ea5e9;
        }
        .fill-sky-100 {
            fill: #e0f2fe;
        }
        .flex-none {
            flex: none;
        }
    }
</style>