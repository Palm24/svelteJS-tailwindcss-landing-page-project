<script>

  import './page.css'
  
  import img2 from '../assets/images/cover-section1-dashboard.jpg';
  
</script>

<!-- <style>
.img-section1-left {
  position: relative;
  background-image: url(../assets/images/bg-section1-banner-2.jpg);
  background-position-x: center;
  background-position-y: center;
  background-size: cover;
  background-repeat: no-repeat;
}

.img-label {
  position: absolute;
  left: 7%;
  bottom: 20%;
  width: 35%;
}
</style> -->

  <div class="grid grid-cols-1 md:grid-cols-4 lg:grid-cols-4">

      <div style="" class="img-section1-left p-52 md:row-span-6 lg:row-span-6 col-span-1 md:col-span-4 lg:col-span-3"> 
          <!-- <img src={img} alt="image1" class="img-label" /> -->
      </div>

      <div class="md:row-span-1 lg:row-span-1 md:col-span-4 lg:col-span-1">
          <img src={img2} alt="image2" class="w-full"/>
      </div>

      <div class="img-section1-right md:row-span-5 lg:row-span-5 md:col-span-4 lg:col-span-1">
          <div class="p-4 text-2xl text-center text-white bg-gradient-to-r from-blue-700 to-blue-400">
              <p>Domestic Gas to Power</p>
          </div>

          <div class="mx-10 text-xl divide-y-reverse divide-y-2 divide-blue-400 ">
              <div class="text-blue-700 p-2 font-semibold">
                  <p class="text-xl sm:text-2xl mt-2">Gas Pipeline</p>
              </div>
        
              <div class="p-2 text-blue-500">
                  <table>
                    <tbody>
                      <tr>
                        <td style="width: 50%;">Size : </td>
                        <td class="text-td-table">24" and 14"</td>
                      </tr>
                      <tr>
                        <td style="width: 50%;">Capacity : </td>
                        <td class="text-td-table">300 MMSCFD</td>
                      </tr>
                      <tr>
                        <td style="width: 50%;">Length :	</td>
                        <td class="text-td-table">
                          <div>Offshore 24" 300 KM</div>
                          <div>Onshore 24" 79 KM</div>
                          <div>Onshore 14" 21 KM</div>
                        </td>
                      </tr>
                    </tbody>
                  </table>
              </div>
          </div>

          <div class="mx-10 text-xl divide-y-reverse divide-y-2 divide-blue-400">
              <div class="text-blue-700 p-2 font-semibold">
                  <p class="text-xl sm:text-2xl mt-2">Power Plant <span class="font-thin">(Combined Cycle)</span></p>
              </div>
        
              <div class="p-2 text-blue-500">
                  <table>
                    <tbody>
                      <tr>
                        <td style="width: 60%;">Location : </td>
                        <td class="text-td-table">Kyalklat</td>
                      </tr>
                      <tr>
                        <td style="width: 60%;">Capacity : </td>
                        <td class="text-td-table">600 MW</td>
                      </tr>
                      <tr>
                        <td style="width: 60%;">Length :	</td>
                        <td class="text-td-table">100 MMSCFD</td>
                      </tr>
                    </tbody>
                  </table>
              </div>
          </div>

          <div class="mx-10 text-xl">
              <div class="text-blue-700 p-2 font-semibold">
                  <p class="text-xl sm:text-2xl mt-2">Supply Sources</p>
              </div>
        
              <div class="p-2 text-blue-500">
                  <table>
                    <tbody>
                      <tr>
                        <td style="width: 62%;">Zawtika : </td>
                        <td class="text-td-table">40 MMSCFD</td>
                      </tr>
                      <tr>
                        <td style="width: 62%;">M-3 : </td>
                        <td class="text-td-table">60 MMSCFD</td>
                      </tr>
                    </tbody>
                  </table>
              </div>
          </div>

          <div class="p-4 text-2xl text-center text-white bg-gradient-to-r from-blue-500 to-teal-400">
              <p>Pipeline Extension to Yangon</p>
          </div>

          <div class="mx-10 text-xl">
              <div class="text-blue-700 p-2 font-semibold">
                  <p class="text-xl sm:text-2xl mt-2">Gas Pipeline</p>
              </div>
        
              <div class="p-2 text-blue-500">
                  <table>
                    <tbody>
                      <tr>
                        <td style="width: 60%;">Size : </td>
                        <td class="text-td-table">24"</td>
                      </tr>
                      <tr>
                        <td style="width: 60%;">Capacity : </td>
                        <td class="text-td-table">300 MMSCFD</td>
                      </tr>
                      <tr>
                        <td style="width: 60%;">Length :	</td>
                        <td class="text-td-table">77 KM</td>
                      </tr>
                    </tbody>
                  </table>
              </div>
          </div>

      </div>
  </div>


