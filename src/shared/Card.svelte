<div class="card absolute inset-0 bg-[url(/img/grid.svg)] bg-center [mask-image:linear-gradient(180deg,white,rgba(255,255,255,0))]">
    <slot>

    </slot>
</div>


<style>
    @media (min-width: 545px){
        .card{
            height: calc(100vh - 50px);
            background: #fff;   
            padding: 20px;
            border-radius: 6px;
            box-shadow: 0px 2px 4px rgba(0,0,0,0.1);
            max-height: 800px;
            text-align: center;
            overflow: hidden;
            position: absolute;
        }
    }

    /* @media (min-width: 245px){
        .card{
            position: fixed;
            z-index: 1;
        }
    } */
   
</style>