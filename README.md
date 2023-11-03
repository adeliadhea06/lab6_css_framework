# lab6_css_framework

Nama : DHea Dwi Adelia

NIM : 312210116

Kelas : TI.22.A.1

### Intruksi Praktikum

1. Persiapkan text editor misalnya VSCode.

2. Buat folder baru dengan nama lab6_css_framework

3. Buat file baru dokumen html

4. Buat struktur dasar dari dokumen HTML.

5. Buatlah layout web sederhana menggunakan css frameword (Twitter Bootsrtap).

6. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

### Langkah - Langkah

1. Buatlah file dengan nama __jQueryEffects_Sliding.html___. Kemudian masukkan kodingan sebagai berikut:

      <!DOCTYPE html>
      <html>
      <head>
          <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
          </script>
          <script>
          $(document).ready(function(){
              $("#flip").click(function(){
                  $("#panel").slideToggle("slow");
              });
          });
          </script>
      
          <style type="text/css">
          #panel, #flip {
              padding:5px;
              text-align:center;
              background-color: #e5eecc;
              border:solid 1px #c3c3c3;
          }
          #panel {
              padding:50px;
              display:none;
          }
          </style>
      </head>
      <body>
          <div id="flip">Click to slide the panel down or up</div>
          <div id="panel">Hello World!</div>
      </body>
      </html>

   ![Screenshot (468)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/e7262279-207f-417a-8e6d-0774f451188b)

   Berikut adalah hasilnya:

   ![Screenshot (443)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/9b0c8b13-8bfe-40b3-ab0b-4fcb279502e9)

   ![Screenshot (444)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/976a7215-092f-477c-9fbb-2da9f5ab577f)


2. Selanjutnya membuat file baru lagi dengan nama __jQueryEffects_Animation.html. Kemudian masukkan kodingan sebagai berikut:

      <!DOCTYPE html>
      <html>
      <head>
          <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.2/jquery.min.js">
          </script>
          <script>
          $(document).ready(function(){
              $("button").click(function(){
                  var div=$("div");
                  div.animate({height:'300px',opacity:'0,4'},"slow");
                  div.animate({width:'300px',opacity:'0,8'},"slow");
                  div.animate({height:'100px',opacity:'0,4'},"slow");
                  div.animate({width:'100px',opacity:'0,8'},"slow");
              });
          });
          </script>
          </head>
          
          <body>
              <button>Start Animation</button>
              <div style="background:#98bf21;height:100px;width:100px;position:absolute;">
              </div>
      </body>
      </html>

    ![Screenshot (469)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/7ce811ca-d066-482b-b436-82085d91d0fd)

   Berikut adalah hasilnya:

   ![image](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/90235218-ed7d-46e3-af12-8723790e3d97)

   ![image](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/8aa0b468-5594-4b10-95d9-8064eaeedd97)

   ![image](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/7ee1a81c-1e82-4f25-8329-b38d0381a8da)

   ![image](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/70389dde-e868-407f-a5e9-be3a7410d0f7)

   ![image](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/66e9610c-26df-472b-ac53-e6b84c4dd8c2)


3. Dan yang terkhir adalah membuat file dengan nama __jQueryUIDraggable.html__. Kemudian masukkan kodingan berikut:

      <!DOCTYPE html>
      <html lang="en">
          <head>
              <script src="http://code.jquery.com/jquery-1.9.1.js"></script>
              <script src="http://code.jquery.com/ui/1.10.3/jquery-ui.js"></script>
              <style>
              #draggable {
                  width: 125px;
                  height: 125px;
                  background-color: #FFF;
                  text-align: center;
                  padding: 1px 5px;
                  border: 1px solid #AAA;
                  margin: auto;
                  float: left;
              }
              #containment-wrapper {
                  width: 95%;
                  height: 200px;
                  border: 1px solid #4E4E4E;
                  padding: 10px;
              }
              </style>
              <script>
              $(function (){
                  $("#draggable").draggable({
                      containment: "#containment-wrapper",scroll:false
                  })
              })
              </script>
          </head>
          <body>
              <div id="containment-wrapper">
                  <div id="draggable">
                      <p>I'm contained within the box</p>
                  </div>
              </div>
      </body>
      </html>

    ![Screenshot (470)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/fe78eda2-f5fa-4430-a77d-e2466077b2d9)

    ![Screenshot (471)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/90d408bb-2375-4fc7-8479-f1794bd0696a)

   Berikut adalah hasilnya:

   ![image](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/775b322f-f0bd-412f-be57-a9fee7dfa435)


### TWITTER BOOTSTRAP

Disini kita akan membuat layout sederhana dengan menggunakan css framework(Twitter Bootstrap).

1. Membuat file baru dengan nama __Twitter_Bootstrap.html__. Kemudian masukkan kodingan berikut:

      <!DOCTYPE html>
      <html lang="en">
          <head>
              <meta charset="utf-8">
              <meta name="viewport" content="width=device-width, initial-scale=1">
              <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-T3c6CoIi6uLrA9TneNEoa7RxnatzjcDSCmG1MXxSR1GAsXEV/Dwwykc2MPK8M2HN" crossorigin="anonymous">
              <title>Layout Sederhana</title>
          </head>
          <body>
              <div class="container shadow-lg">
                  <div class="card-body bg-light p-3">
                      <h1 class="text-secondary py-3 text-opacity-50 fw-bold">Layout Sederhana</h1>
                  </div>
                  <nav class="navbar navbar-expand-lg navbar-dark" style="background-color: #1f5faa;">
                      <div class="container-fluid">
                      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                          <span class="navbar-toggler-icon"></span>
                      </button>
                      <div class="collapse navbar-collapse" id="navbarSupportedContent">
                          <ul class="navbar-nav">
                          <li class="nav-item active ms-4">
                              <a class="nav-link text-light fs-5 fw-semibold" aria-current="page" href="index.html" >Home</a>
                          </li>
                          <li class="nav-item ms-4">
                              <a class="nav-link fs-5 fw-semibold" href="#">Article</a>
                          </li>
                          <li class="nav-item ms-4">
                              <a class="nav-link fs-5 fw-semibold" href="#">About</a>
                          </li>
                          <li class="nav-item ms-4">
                              <a class="nav-link fs-5 fw-semibold" href="#">Contact</a>
                          </li>
                          </ul>
                      </div>
                      </div>
                  </nav>
                  <div class="jumbotron p-2 text-secondary bg-opacity-25" style="background-color:#e4e4e5;">
                      <h1 class="p-3 text-secondary fw-bold">Hello World!</h1>
                      <p class="lead p-3 text-secondary">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                      <a href="#" class="btn btn-primary mb-3 fw-semibold mx-3">Learn more &raquo;</a></p>
                  </div>
                   <div class="row">
                      <div class="col-md-9">
                          <div class="row">
                              <div class="col-3 mx-4">
                                  <div class="col mt-4">
                                      <div class="card pt-3" style="border: 0;">
                                          <img src="https://dummyimage.com/120/db7d25/fff.png" class="card-img-top rounded-circle" alt="...">
                                          <div class="card-body">
                                              <h5 class="card-title text-center">Heading</h5>
                                              <p class="card-text text-center">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                                              <p class="card-text text-center"><a href="#" class="btn btn-secondary mt-2">View Detail</a></p>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                              <div class="col-3 mx-4">
                                  <div class="col mt-4">
                                      <div class="card pt-3" style="border: 0;">
                                          <img src="https://dummyimage.com/120/3e73e6/fff.png" class="card-img-top rounded-circle" alt="...">
                                          <div class="card-body">
                                              <h5 class="card-title text-center">Heading</h5>
                                              <p class="card-text text-center">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                                              <p class="card-text text-center"><a href="#" class="btn btn-secondary mt-2">View Detail</a></p>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                              <div class="col-3 mx-4">
                                  <div class="col mt-4">
                                      <div class="card pt-3" style="border: 0;">
                                          <img src="https://dummyimage.com/120/71e6d4/fff.png" class="card-img-top rounded-circle" alt="...">
                                          <div class="card-body">
                                              <h5 class="card-title text-center">Heading</h5>
                                              <p class="card-text text-center">Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                                              <p class="card-text text-center"><a href="#" class="btn btn-secondary mt-2">View Detail</a></p>
                                          </div>
                                      </div>
                                  </div>
                              </div>
                          </div>
                      </div>
                      <div class="col-md-3">
                          <div class="my-3 mt-5">
                              <div class="list-group" style="border-radius: 0;">
                                  <a href="#" class="list-group-item list-group-item-action active" aria-current="true" style="font-weight: bold;">Widget Header</a>
                                  <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                  <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                  <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                  <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                                  <a href="#" class="list-group-item list-group-item-action">Widget Link</a>
                              </div>
                              <div class="list-group my-4" style="border-radius: 0; border: 1px">
                                  <a href="#" class="list-group-item list-group-item-action active " aria-current="true" style="font-weight: bold;">Widget Text</a>
                                  <a href="#" class="list-group-item list-group-item-action">
                                      <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                                  </a>
                              </div>
                          </div>
                      </div>
                      <div>
                          <div class="mb-5" style="width: 900px; border: 0;">
                              <h2>First featurette heading.</h2>
                              <div class="row no-gutters">
                                  <div class="col-md-3">
                                      <img src="https://dummyimage.com/150/7b8a70/fff.png" class="card-img-top rounded-square" style="width: 200px;" alt="...">
                                  </div>
                                  <div class="col-md-8">
                                      <div class="card-body">
                                          <p class="card-text lead p-3 fs-5">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                                      </div>
                                  </div>
                              </div>
                          </div>
                          <div class="mt-5 mb-5" style="width: 900px; border: 0;">
                              <h2>First featurette heading.</h2>
                              <div class="row">
                                  <div class="col-md-8">
                                      <div class="card-body">
                                          <p class="lead p-3 fs-5">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                                      </div>
                                  </div>
                                  <div class="col-md-3">
                                      <img src="https://dummyimage.com/150/7b8a70/fff.png" class="card-img-top rounded-square" style="width: 200px;" alt="...">
                                  </div>
                              </div>
                          </div>
                      </div>
                      <div class="card-footer text-start bg-dark text-light p-2">
                          <p>&copy; 2021 - Universitas Pelita Bangsa</p>
                      </div>
                  </div>
              </div>
              <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL" crossorigin="anonymous"></script>
          </body>
      </html>


  Berikut adalah hasilnya:

  ![Screenshot (467)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/5154db13-6675-460c-8776-bf0c5eb6ab8c)


  - Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

    ![Screenshot (475)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/e7ce1ea3-2919-4f5e-b24c-8f43563a71ea)
    
    ![Screenshot (474)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/30194433-dea1-468e-a2e1-cc67f5250134)

    ![Screenshot (477)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/4e436af3-973d-4403-8fde-da653a4d6613)
    
    ![Screenshot (476)](https://github.com/adeliadhea06/lab6_css_framework/assets/115794875/f958ae25-9731-4906-afa8-37d213929588)


    ### Sekian, Terima Kasih.


