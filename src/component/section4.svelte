<script>
    import Swal from "sweetalert2";
    import './page.css';

    import Message5_block1_1 from './message/secation5/section5_block1/message5-1-1.svelte'
    import Message5_block1_2 from './message/secation5/section5_block1/message5-1-2.svelte'
    import Message5_block1_3 from './message/secation5/section5_block1/message5-1-3.svelte'

    import Message5_block2_1 from './message/secation5/section5_block2/message5-2-1.svelte'

    import Message5_block3_1 from './message/secation5/section5_block3/message5-3-1.svelte'
    
    import img6 from '../assets/images/block1-img1.jpg';
    import img7 from '../assets/images/block1-img2.jpg';

    import img8 from '../assets/images/block2-img1.jpg';
    import img9 from '../assets/images/block2-img2.jpg';
    import img10 from '../assets/images/block2-img3.jpg';
    
    import img11 from '../assets/images/block3-img1.jpg';
    import img12 from '../assets/images/block3-img2.jpg';
    import img13 from '../assets/images/block3-img3.jpg';

    var data = {
      "itemId": "0987654321",
      "itemName": "PMNTS"
    };

    var items = [
      { 
        "itemId": "1234567890", 
        "itemName": "Natthasit Suksumran"
      },
    ];

</script>

<div class="img-section5">
  <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-3">

    <div class="relative p-16 col-span-1">
      <div class="z-[1] relative">
        <img src="{img6}" alt="img block1 section5" class="img5-circle">
        <div class="font-thin  text-center font-sans mb-[2em] text-[4vw] md:text-[1.9vw] my-16 min-h-[3.5em] border-b-2 border-blue-300">
          Gas Pipeline Network
        </div>

        <Message5_block1_1 />

        <Message5_block1_2 />

        <div class="mb-10 sm:flex justify-center">
          <img src="{img7}" alt="img1 block2 section5">
        </div>

        <Message5_block1_3 />

        <div class="text-center visible sm:visible  md:invisible">
          <button class="bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
            Dowload PDF
          </button>
        </div>

      </div>
    </div>

    <div class="relative p-16 col-span-1">
      <div class="z-[1] relative">
        <img src="{img8}" alt="img block2 section5" class="img5-circle">
        <div class="font-thin  text-center font-sans mb-[2em] text-[4vw] md:text-[1.9vw] my-16 min-h-[3.5em] border-b-2 border-blue-300">
          Combined Cycle Power Plant (CCPP)
        </div>

        <Message5_block2_1 />

        <div class="mb-10">
          <div class="text-[3vw] md:text-[1.5vw] mb-6 text-center ">
            Typical Process of CCPP
          </div>
          <div class="sm:flex justify-center">
            <img src="{img9}" alt="img2 block2 section5">
          </div>
        </div>

        <div class="mb-10">
          <div class="text-[3vw] md:text-[1.5vw] mb-6 text-center">
            Typical Process of CCPP
          </div>
          <div class="sm:flex justify-center">
            <img src="{img10}" alt="img2 block2 section5">
          </div>
        </div>

        <div class="text-center visible sm:visible  md:invisible">
          <button class="bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
            Dowload PDF
          </button>
        </div>

      </div>
    </div>
    
    <div class="relative p-16 col-span-1">
      <div class="z-[1] relative">
        <img src="{img11}" alt="img block3 section5" class="img5-circle">
        <div class="font-thin  text-center font-sans mb-[2em] text-[4vw] md:text-[1.9vw] my-16 min-h-[3.5em] border-b-2 border-blue-300">
          Electrical Transmission Line
        </div>

        <Message5_block3_1 />

        <div class="mb-10">
          <div class="text-[3vw] md:text-[1.5vw] mb-6 text-center">
            Typical Process of CCPP
          </div>
          <div class="sm:flex justify-center">
            <img src="{img12}" alt="img2 block3 section5">
          </div>
        </div>

        <div class="mb-10">
          <div class="text-[3vw] md:text-[1.5vw] mb-6 text-center">
            Preliminary Transmission Line Route
          </div>
          <div class="sm:flex justify-center">
            <img src="{img13}" alt="img2 block3 section5">
          </div>
        </div>

        <div class="text-center visible sm:visible md:invisible">
          <button class="bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
            Dowload PDF
          </button>
        </div>

      </div>
    </div>

  </div>

  <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-3 invisible sm:invisible md:visible">
    <div class="col-span-1 text-center relative mb-6">
      {#each items as itemsData}
        {#if itemsData.itemId == null || itemsData.itemId == ""}
        <button 
          disabled
          class=" bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
          Dowload PDF
        </button>
        {:else}
          <button on:click={() => {
            var file = "";
            var text = "";

            if (file == "" || file == null) {
              text = 'Now! no file to dowload!';
            } else {
              text = 'Dowload';
            }

            Swal.fire({
              title: text,
              icon: 'warning',
              confirmButtonText: 'OK!',
              cancelButtonText: 'Cancel',
              showCancelButton: true,
              showCloseButton: false,
              allowOutsideClick: false,
              allowEscapeKey: false
              }).then(result => {
                if (result.value) {
                  Swal.fire(
                    'Great!', 
                    "See you again next time!", 
                    'success'
                  )
                }
              });
            }}
            class=" bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
            Dowload PDF
          </button>
        {/if}

        <div class="my-2 invisible">
          <p>{itemsData.itemId}</p>
          <p>{itemsData.itemName}</p>
        </div>
      {/each}
    </div>

    <div class="col-span-1 text-center">
      {#if data.itemId == null || data.itemId == "" || data.itemId == "undefined" }
        <button 
          class="bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
          Dowload PDF
        </button>
      {:else}
        <button on:click={() => {
          Swal.fire({
            title: 'Notification!',
            text: 'You will not be able to dowload file!',
            icon: 'warning',
            confirmButtonText: 'OK',
            cancelButtonText: 'Cancel',
            showCancelButton: true,
            showCloseButton: true,
            showDenyButton: true,
            denyButtonText: `Have a question?`,
          }).then(result => {
            if (result.value) {
              Swal.fire(
                'Great!', 
                'See You again next time!', 
                'success'
              );
            } 
            else if (result.dismiss === Swal.DismissReason.cancel) {
              Swal.fire(
                'Cancelled', 
                'Get well soon :)', 
                'error'
              );
            }
            else if (result.isDenied) {
              Swal.fire({
                title: 'You Question?',
                input: 'text',
                icon: 'question',
                // inputAttributes: {
                //   autocapitalize: 'off'
                // },
                confirmButtonText: 'Submit',
                showCancelButton: true,
                showLoaderOnConfirm: true,
                allowOutsideClick: false,
                allowEscapeKey: false
              }).then(result => {
                if (result.isConfirmed) {
                  Swal.fire(
                    'Good job', 
                    'Thank you for question. We will reply as soon as possible.', 
                    'success'
                  );
                }
              })
            }
          });
        }}
        class="bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
        Dowload PDF
      </button>
      {/if}
    </div>

    <div class="col-span-1 text-center">
      {#if data.itemId == null || data.itemId == "" || data.itemId == "undefined"}
        <button 
          disabled
          class="bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
          Dowload PDF
        </button>
      {:else}
        <button
          class="bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md">
          Dowload PDF
        </button>
      {/if}
    </div>
  </div>

</div>


