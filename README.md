<!-- ----------------------------Home page -------------------------------- -->


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="body.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,600;1,300;1,400;1,500&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.2.1/css/fontawesome.min.css">
<script src="https://kit.fontawesome.com/283c56fb1a.js" crossorigin="anonymous"></script>
<title>document</title>
</head>
<body>


    <div class="navbar">
   
            <div class="logo" style="display: flex;">
                <img src="C:\Users\REYZEN\Downloads/images.png" width="120px">
                <li style="font-family:'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif; pointer-events: none; font-size:x-large; text-decoration: none;list-style: none;display: grid;justify-content: center;align-items: center;color: white;">Book M!</li>
             </div>
     
             <div class="search">
                 <i class="fa-solid fa-magnifying-glass" style="color: white;"></i>
               
                    <input type="text"  placeholder="Search" style=" border: 2px solid #0583D2; font-size: large;width: 35vh; padding: 5px 10px;border-radius: 10px;font-family:'Times New Roman', Times, serif;">
           
                
             </div>
             <nav>
                 <ul>
                     <li><i class="fa-solid fa-house" style="margin-right: 5px; color: white;"></i> <a href="index-1.html" style="font-size: large;">Home</a></li>
                     <li><a href="" style="font-size: large;">About</a></li>
                     <li><a href="" style="font-size: large;">Contect</a></li>
                     <li><a href="" style="font-size: large;">Details</a></li>
                     <li><a href="" style="font-size: large;">More</a></li>
                    
                 </ul>
                 <li class="A"><i class="fa-solid fa-bars fa-xl" style="color: white;"></i>
                
                    <ul id="B">
                        <ul id="B1">
                            <li><a href="index-1.html" style="font-size: large;">Home</a></li>
                            <li><a href="" style="font-size: large;">About</a></li>
                            <li><a href="" style="font-size: large;">Contect</a></li>
                            <li><a href="" style="font-size: large;">Details</a></li>
                            <li><a href="" style="font-size: large;">More</a></li>
                        </ul>
                   
                    </ul>
                
                
                   
                </li>     
             </nav>
     
            
             <a href="login_page.html" class="login" style="font-size: large;">Login</a>
             <a href="signup.html" class="sinup" style="font-size: large;">Sign Up</a>

                
      
    </div>
<!-- ----------------------------new offer -------------------------------- -->

    <div class="Mainco">


        <div class="Contenarw">
            <span class="nextxE">&#10095</span>
            <span class="backxE">&#10094</span>
    
                <div class="slideRowE">
                    <div class="slideE" id="lastImageDuplicateE">
                        <img src="C:\Users\REYZEN\Downloads/off5.jpg" alt="">
                    </div>
                    <div class="slideE">
                        <img src="C:\Users\REYZEN\Downloads/off1.jpg" alt="">
                    </div>
                    <div class="slideE">
                        <img src="C:\Users\REYZEN\Downloads/off2.jpg" alt="">
                    </div>
                    <div class="slideE">
                        <img src="C:\Users\REYZEN\Downloads/off3.jpg" alt="">
                    </div>
                    <div class="slideE">
                        <img src="C:\Users\REYZEN\Downloads/off4.jpg" alt="">
                    </div>
                    <div class="slideE">
                        <img src="C:\Users\REYZEN\Downloads/off5.jpg" alt="">
                    </div>
                    <div class="slideE" id="firstImageDuplicateE">
                        <img src="C:\Users\REYZEN\Downloads/off1.jpg" alt="">
                    </div>
                   
            
            </div>

          
            <div class="dotsE">
                <div class="dotE activeE"></div>
                <div class="dotE"></div>
                <div class="dotE"></div>
                <div class="dotE"></div>
                <div class="dotE"></div>
            </div>
         
        </div>
  
    </div>

    <script>
        const carouselrowE = document.querySelector(".slideRowE");
        const carouselslideE = document.getElementsByClassName("slideE");
        const dotsE = document.getElementsByClassName("dotE");
        const nextbtnxE = document.querySelector(".nextxE");
        const backbtnxE = document.querySelector(".backxE");
    
        let indexE = 1;
         
         widthE = carouselslideE[0].clientWidth;
         carouselrowE.style.transform = 'translateX('+(-widthE * indexE)+'px)';
    
         nextbtnxE.addEventListener("click" ,nextSlideE);
            function nextSlideE(){
                if(indexE>=carouselslide.length-1){return};
                carouselrowE.style.transition = 'transform 0.5s ease-out';
                indexE++;
                carouselrowE.style.transform = 'translateX('+(-widthE * indexE)+'px)';
                dotLableE();
    
            }
    
        backbtnxE.addEventListener("click" ,backSlideE);
            function backSlideE(){
                if(indexE<=01){return};
                carouselrowE.style.transition = 'transform 0.5s ease-out';
                indexE--;
                carouselrowE.style.transform = 'translateX('+(-widthE * indexE)+'px)';
               dotLableE();
    
    
            }
    
            carouselrowE.addEventListener("transitionend",function(){
                if(carouselslideE[indexE].id ==="firstImageDuplicateE" ){
                    carouselrowE.style.transition ="none";
                    indexE=carouselslideE.length -indexE;
                    carouselrowE.style.transform = 'translateX('+(-widthE * indexE)+'px)';
                    dotLableE();
    
                }
              
                 if(carouselslideE[indexE].id ==="lastImageDuplicateE" ){
                    carouselrowE.style.transition ="none";
                    indexE=carouselslideE.length -2;
                    carouselrowE.style.transform = 'translateX('+( -widthE * indexE)+'px)';
                    dotLableE();
    
                }
            });
            function autoslideE(){
                deleteIntarvalE = setInterval(timer,3000);
                function timer(){
                    nextSlideE();
                }
          
            }
            autoslideE();
    
    const maincontenarE = document.querySelector(".Contenarw");
    
    maincontenarE.addEventListener("mouseover",function(){
        clearInterval(deleteIntarvalE);
    });
    maincontenarE.addEventListener("mouseout",autoslideE);
    
    function dotLableE(){
       for(i=0;i<dots.length;i++){
        dotsE[i].className = dotsE[i].className.replace(' activeE',' ');
       }
       dotsE[indexE-1].className += ' activeE';
    }
    
    
    </script>

<!-------------------categorise------------------------->


<div class="categorise">

    <div class="opctionbar">

        <div class="op1">
            
            <a href="index-2.html"><p>Movie </p></a>
       
        </div>
        <div class="op1">
            <a href="index-3.html"><p>Events </p></a>
       
        </div>
        <div class="op1">
            <a href="index-4.html"><p>Streem </p></a>
       
        </div>
        <div class="op1">
            <a href="index-5.html"><p >Sports </p></a>
        </div>
        <div class="slidar">

        <div id="op2">
            <p>Filter</p>
      <i class="fa-solid fa-chevron-down" style=" color: #000000;"></i>
         
            <ul id="list">
            <li id="in"><a href="#">Language</a>
            <div class="inlist">
                <ul>
                    <li>Hindi<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>English<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Gujarati<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Tamil<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Telugu<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Malialam<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Panjabi<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Marathi<input type="checkbox" style="margin-left: 10px;"></li>
    

                </ul>
            </div>
            
            
            </li>
            <li id="in"><a href="#">Format</a>
                <div class="inlist">
                    <ul>
                        <li>Drama<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Comedy<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Thrill<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Action<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Romantic<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Horror<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Crime<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Family<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Biography<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Historical<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Mystery<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Adventure<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Animation<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>classic<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Sports<input type="checkbox" style="margin-left: 10px;"></li>
                    <li>Sci-Fi<input type="checkbox" style="margin-left: 10px;"></li>
                
                </ul>
                </div>
                
                
                </li>
                <li id="in"><a href="#">Features</a>
                    <div class="inlist">
                        <ul>
                            <li>2D<input type="checkbox" style="margin-left: 10px;"></li>
                            <li>4DX<input type="checkbox" style="margin-left: 10px;"></li>
                            <li>MX4D<input type="checkbox" style="margin-left: 10px;"></li>
                            <li>IMAX2D<input type="checkbox" style="margin-left: 10px;"></li>
                            <li>3D<input type="checkbox" style="margin-left: 10px;"></li>
                        </ul>
                    </div>
                    
                    
                    </li>
                  
                 
             </ul>
              </div>
        </div>
   
              
    </div>

    <script>
        let filtar = document.getElementById("op2");
        let list = document.getElementById("list");

    filtar.onclick = function(){
        list.classList.toggle("open");}

    </script>
<div class="lineE1"></div>

    <div class="centar">
       <div class="title1">
           <h1>Recommended Show</h1>

           
           <p>See all</p>
          </div>
    </div>
     
         
    <div class="gallry-wrep">
             
      <img src="C:\Users\REYZEN\Downloads/left.png" id="image1">
        <div class="gallery">
       
             <div class="ingallery">

              <div class="sepretbox">
                  <div class="box0">
                    <i class="fa-solid fa-heart fa-xl" style="position: absolute; z-index: 1; margin-top: 20px; margin-left: 180px; color: rgb(255, 48, 48);cursor: pointer;"></i>
                    <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/101.jpg" ></a>
                  </div>

                  <div class="box1">
                    
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                
                
                </div>
              </div>
            

             
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/201.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                      </div>
              </div>

              <!-- ================================================= -->

              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/103.jpg"></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                      </div>
              </div>
            <!-- ==================================================== -->
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/104.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                      </div>
              </div>
              <div class="sepretbox">
                <div class="box0">
                     <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/105.png" ></a>
                </div>

                <div class="box1">
                  <p>Jawan</p>
                  <p>threl,Action,Suspens</p>
                  <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                    
                  <div class="inbox1">
                      <a href=""><p> Book Now</p></a>
                  </div>
                    </div>
            </div>
           </div>
          
           <div class="ingallery">

              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/106.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                      </div>
              </div>
            
              <div class="sepretbox">
                <div class="box0">
                     <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/107.jpg" ></a>
                </div>

                <div class="box1">
                  <p>Jawan</p>
                  <p>threl,Action,Suspens</p>
                  <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                    
                  <div class="inbox1">
                      <a href=""><p> Book Now</p></a>
                  </div>
                    </div>
            </div>
             
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/108.jpg"></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                      </div>
              </div>

              
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/109.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                      </div>
              </div>
              <!-- ================================================== -->
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/110.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                    </div>
                      </div>
              </div>
            <!-- ===================================================== -->
                       

           </div>

          

         
        </div>
    
        <img src="C:\Users\REYZEN\Downloads/right.png" id="image2">


 </div>
 
<script src="projectfile.js"></script>

<!-- ------------------------------------------------------------------------------------ -->
<div class="lineE1"></div>

<div class="centar">
    <div class="title1">
        <h1>Live Events</h1>
     
    
    <p>See all</p></div>
 </div>

       
        <div class="gallry-wrep">
            <img src="C:\Users\REYZEN\Downloads/left.png" id="image3">
     
        <div class="gallery2">
       
             <div class="ingallery">

              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/111.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
              </div>
            
            </div>
             
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/112.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
              </div>
            </div>
              <!-- ================================================= -->

              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/113.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
              </div>
            </div>
            <!-- ==================================================== -->
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/114.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
              </div>
                 
           </div>
           <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/115.jpg" ></a>
            </div>

            <div class="box1">
              <p>Jawan</p>
              <p>threl,Action,Suspens</p>
              <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                
              <div class="inbox1">
                  <a href=""><p> Book Now</p></a>
                </div>
        </div>
           
     </div>
        </div>
           <div class="ingallery">

              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/116.webp" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
              </div>
            </div>

            <div class="sepretbox">
                <div class="box0">
                     <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/117.jpg" ></a>
                </div>

                <div class="box1">
                  <p>Jawan</p>
                  <p>threl,Action,Suspens</p>
                  <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                    
                  <div class="inbox1">
                      <a href=""><p> Book Now</p></a>
                    </div>
            </div>
               
         </div>
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/112.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
                      </div>
              </div>

           
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/113.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
              </div>
            </div>
              <!-- ================================================== -->
              <div class="sepretbox">
                  <div class="box0">
                       <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/114.jpg" ></a>
                  </div>

                  <div class="box1">
                    <p>Jawan</p>
                    <p>threl,Action,Suspens</p>
                    <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                      
                    <div class="inbox1">
                        <a href=""><p> Book Now</p></a>
                      </div>
              </div>
            <!-- ===================================================== -->
                 
           </div>
      
      
        </div>
    </div>
        <img src="C:\Users\REYZEN\Downloads/right.png" id="image4">
  
    </div>

<script>
let scrollContenar1 = document.querySelector(".gallery2");
let nextbtn1 = document.getElementById("image3");
let backbtn1 = document.getElementById("image4");


nextbtn1.addEventListener("click",()=>{
    
    scrollContenar1.style.scrollBehavior = "smooth";
    scrollContenar1.scrollLeft  -= 1600;


});
backbtn1.addEventListener("click",()=>{
    scrollContenar1.style.scrollBehavior = "smooth";
   
    scrollContenar1.scrollLeft  += 1600;
  
});

</script>

 <!-- ----------------------------------------------------------------------------- -->




 
       
 <div class="gallry-wrep">
    <img src="C:\Users\REYZEN\Downloads/left.png" id="image5">
     
  <div class="gallery3">
 
       <div class="ingallery">

        <div class="sepretbox">
            <div class="box0">

                <i class="fa-solid fa-heart fa-xl" style="position: absolute; z-index: 1;"></i>
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/118.jpg" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
      
        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/119.jpg" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
       
        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/120.jpg" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>

        <!-- ================================================= -->

        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/121.jpg" ></a>
            </div>
            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
      <!-- ==================================================== -->
        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/122.png" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
           
     </div>
    
     <div class="ingallery">

        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/118.jpg" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
      
        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/119.jpg" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
       
        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/120.jpg" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>

        
        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/115.jpg" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
        <!-- ================================================== -->
        <div class="sepretbox">
            <div class="box0">
                 <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/116.webp" ></a>
            </div>

            <div class="box1">
                <p>Jawan</p>
                <p>threl,Action,Suspens</p>
                <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
                  
                <div class="inbox1">
                    <a href=""><p> Book Now</p></a>
                  </div>
          </div>
        </div>
      <!-- ===================================================== -->
           
     </div>


  </div>

<img src="C:\Users\REYZEN\Downloads/right.png" id="image6">
  
</div>


<script>
    let scrollContenar2 = document.querySelector(".gallery3");
let nextbtn2 = document.getElementById("image5");
let backbtn2 = document.getElementById("image6");



nextbtn2.addEventListener("click",()=>{
scrollContenar2.scrollLeft  -= 1600;


scrollContenar2.style.scrollBehavior = "smooth";
});
backbtn2.addEventListener("click",()=>{
scrollContenar2.style.scrollBehavior = "smooth";

scrollContenar2.scrollLeft  += 1600;
 if(clickon == 1){
    nextbtn1.style.display = "block";
    backbtn1.style.display = "none";
    clickon =0;
 }
});
</script>
</div>


<!-- ============================================================================== -->
<div class="small1">


    <!-- <div class="backgroundY">
        <img src="C:\Users\REYZEN\Downloads/X1.jpg" alt="">
    </div> -->


<div class="centar">
    <div class="title3">
        <h1 style="color: rgb(255, 255, 255);margin-top: 100px;
        margin-left: 100px;border-bottom: 2px solid rgb(255, 72, 0);
        width: 300px;">Primium Movies</h1>
         <i class="fa-solid fa-circle-play fa-2xl" style="color: rgb(255, 72, 0); margin-left: 380px;
    margin-top: -30px; position: absolute;"></i>
       </div>

      
 </div>
 
       
<div class="gallry-wrep">
       
    <img src="C:\Users\REYZEN\Downloads/left.png" id="image11">
<div class="gallery4">

   <div class="ingallery">

    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/128.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>
    </div>
  
    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/129.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>
    </div>
   
    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/130.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1" id="P1">
                <a href=""><p> Book Now</p></a>
              </div>
      </div>
    </div>

    <!-- ================================================= -->

    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/131.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>
    </div>
  <!-- ==================================================== -->
    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/122.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>
    </div>
       
 </div>

 <div class="ingallery">

    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/123.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>
  </div>
  <div class="sepretbox1">
    <div class="box0">
         <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/124.jpg" ></a>
    </div>

    <div class="boxP">
        <p>Jawan</p>
        <p>threl,Action,Suspens</p>
        <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
          
        <div class="inbox1">
            <a href=""><p id="P1"> Book Now</p></a>
          </div>
  </div>
</div>
   
    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/125.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>

</div>
    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/126.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>
</div>
    <!-- ================================================== -->
    <div class="sepretbox1">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/127.jpg" ></a>
        </div>

        <div class="boxP">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p id="P1"> Book Now</p></a>
              </div>
      </div>
  <!-- ===================================================== -->
       
 </div>


</div>

</div>
<img src="C:\Users\REYZEN\Downloads/right.png" id="image12">


</div>

<script>
    let scrollContenar5 = document.querySelector(".gallery4");
let nextbtn5 = document.getElementById("image11");
let backbtn5= document.getElementById("image12");


nextbtn5.addEventListener("click",()=>{


    scrollContenar5.scrollLeft  -= 1600;

scrollContenar5.style.scrollBehavior = "smooth";



});

backbtn5.addEventListener("click",()=>{


    scrollContenar5.style.scrollBehavior = "smooth";

scrollContenar5.scrollLeft  += 1600;
 if(clickon == 1){
    nextbtn1.style.display = "block";
    backbtn1.style.display = "none";
    clickon =0;
 }

});
</script>




</div>
<!-- ===================================================================================== -->

<div class="categorise1">



<div class="centar">
    <div class="title1">
        <h1>Online Streaming Event</h1>

            <p>See all</p>
        
       </div>
 </div>

       
<div class="gallry-wrep">
       
    <img src="C:\Users\REYZEN\Downloads/left.png" id="image7">
<div class="gallery5">

   <div class="ingallery">

    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/r1.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
  
</div>
   
<div class="sepretbox">
    <div class="box0">
         <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/r2.png" ></a>
    </div>

    <div class="box1">
        <p>Jawan</p>
        <p>threl,Action,Suspens</p>
        <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
          
        <div class="inbox1">
            <a href=""><p> Watch Now</p></a>
          </div>
  </div>

</div>
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/r3.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>

    <!-- ================================================= -->

    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/r4.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
  <!-- ==================================================== -->
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/r5.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
       
 </div>

 <div class="ingallery">

    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/115.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
  
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/117.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
  
</div>

   
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/118.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>

    
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/119.jpg" ></a>
        </div>
        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
    <!-- ================================================== -->
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/120.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
  <!-- ===================================================== -->
       
 </div>


</div>

<img src="C:\Users\REYZEN\Downloads/right.png" id="image8">
</div>

<script>
    let scrollContenar3 = document.querySelector(".gallery5");
let nextbtn3 = document.getElementById("image7");
let backbtn3 = document.getElementById("image8");

nextbtn3.addEventListener("click",()=>{
scrollContenar3.scrollLeft  -= 1600;


scrollContenar3.style.scrollBehavior = "smooth";
});
backbtn3.addEventListener("click",()=>{
scrollContenar3.style.scrollBehavior = "smooth";

scrollContenar3.scrollLeft  += 1600;
 if(clickon == 1){
    nextbtn1.style.display = "block";
    backbtn1.style.display = "none";
    clickon =0;
 }
});
</script>

<!-- ============================================================================================= -->


       
<div class="gallry-wrep">
       
    <img src="C:\Users\REYZEN\Downloads/left.png" id="image9">
<div class="gallery6">

   <div class="ingallery">

    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/rr1.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
  

   
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/rr2.png" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>

    <!-- ================================================= -->

    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/rr3.webp" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
  <!-- ==================================================== -->
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/rr4.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/rr5.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
 </div>

 <div class="ingallery">

    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/112.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/113.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>

   
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/114.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
      </div>
    </div>

    
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/115.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p> Watch Now</p></a>
              </div>
           </div>
    </div>
    <!-- ================================================== -->
    <div class="sepretbox">
        <div class="box0">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/111.jpg" ></a>
        </div>

        <div class="box1">
            <p>Jawan</p>
            <p>threl,Action,Suspens</p>
            <p><i class="fa fa-star" style="color: rgb(252, 59, 139);"></i> 8.3/10</p>
              
            <div class="inbox1">
                <a href=""><p>Watch Now</p></a>
              </div>
      </div>
    </div>
  <!-- ===================================================== -->
       
 </div>


</div>


<img src="C:\Users\REYZEN\Downloads/right.png" id="image10">

</div>
<script>
    let scrollContenar4 = document.querySelector(".gallery6");
let nextbtn4 = document.getElementById("image9");
let backbtn4 = document.getElementById("image10");


nextbtn4.addEventListener("click",()=>{
scrollContenar4.scrollLeft  -= 1600;


scrollContenar4.style.scrollBehavior = "smooth";
});
backbtn4.addEventListener("click",()=>{
scrollContenar4.style.scrollBehavior = "smooth";

scrollContenar4.scrollLeft  += 1600;
 if(clickon == 1){
    nextbtn1.style.display = "block";
    backbtn1.style.display = "none";
    clickon =0;
 }
});
</script>

<div class="consaltuncy">

    
</div>


<div class="lineE1"></div>

<!-- -------------------kid-s shows---------------------- -->

<div class="centar">
    <div class="title1" style="margin-bottom: 60px;">
        <h1>Kid's shows</h1>
     
    
    <p  style="margin-right: 130px;">See all</p></div>
 </div>


<div class="gallry-wrep">
       
    <img src="C:\Users\REYZEN\Downloads/left.png" id="image13">
<div class="gallery7">

   <div class="ingallery1">

  
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/k1.png" ></a>
        </div>

    </div>
  
   
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/k2.jpg" ></a>
        </div>

      
          
      
    </div>

    <!-- ================================================= -->

    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/k3.png" ></a>
        </div>

    </div>
  <!-- ==================================================== -->
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/k4.png" ></a>
        </div>

     
    </div>
       
 </div>

 <div class="ingallery1">

    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr3.jpg" ></a>
        </div>

    
    </div>
  
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/k2.jpg" ></a>
        </div>

    </div>
  


    
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr4.jpg" ></a>
        </div>

    </div>
    <!-- ================================================== -->
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr1.jpg" ></a>
        </div>

    </div>
  <!-- ===================================================== -->
       
 </div>


</div>

<img src="C:\Users\REYZEN\Downloads/right.png" id="image14">
</div>


<script>
    let scrollContenar6 = document.querySelector(".gallery7");
let nextbtn6 = document.getElementById("image13");
let backbtn6 = document.getElementById("image14");

nextbtn6.addEventListener("click",()=>{
scrollContenar6.scrollLeft  -= 1600;


scrollContenar6.style.scrollBehavior = "smooth";
});
backbtn6.addEventListener("click",()=>{
scrollContenar6.style.scrollBehavior = "smooth";

scrollContenar6.scrollLeft  += 1600;
 if(clickon == 1){
    nextbtn1.style.display = "block";
    backbtn1.style.display = "none";
    clickon =0;
 }
});
</script>



<div class="gallry-wrep">
       
    <img src="C:\Users\REYZEN\Downloads/left.png" id="image15">
<div class="gallery8">

   <div class="ingallery1">

    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr1.jpg" ></a>
        </div>

    </div>
  

   
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr2.jpg" ></a>
        </div>

      
          
      
    </div>

    <!-- ================================================= -->

    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr3.jpg" ></a>
        </div>

    </div>
  <!-- ==================================================== -->
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr4.jpg" ></a>
        </div>

     
    </div>
       
 </div>

 <div class="ingallery1">

    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/k3.png" ></a>
        </div>

    
    </div>
  

   
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/k2.jpg" ></a>
        </div>

       
    </div>


    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr2.jpg" ></a>
        </div>

    </div>
    <!-- ================================================== -->
    <div class="sepretbox">
        <div class="box01">
             <a href="Event discripction.html"> <img src="C:\Users\REYZEN\Downloads/kr1.jpg" ></a>
        </div>

    </div>
  <!-- ===================================================== -->
       
 </div>


</div>

<img src="C:\Users\REYZEN\Downloads/right.png" id="image16">
</div>


<script>
    let scrollContenar7 = document.querySelector(".gallery8");
let nextbtn7 = document.getElementById("image15");
let backbtn7 = document.getElementById("image16");

nextbtn7.addEventListener("click",()=>{
scrollContenar7.scrollLeft  -= 1600;


scrollContenar7.style.scrollBehavior = "smooth";
});
backbtn7.addEventListener("click",()=>{
scrollContenar7.style.scrollBehavior = "smooth";

scrollContenar7.scrollLeft  += 1600;
 if(clickon == 1){
    nextbtn1.style.display = "block";
    backbtn1.style.display = "none";
    clickon =0;
 }
});
</script>
</div>
</div>
<!--------------------offer bar------------------------>

 <div class="main">

<div class="contenarw">
  
    <span class="nextx">&#10095</span>
    <span class="backx">&#10094</span>
     <div class="slideRow">
        <div class="slide" id="lastImageDuplicate">
            <img src="C:\Users\REYZEN\Downloads/off5.jpg" alt="">
        </div>
        <div class="slide">
            <img src="C:\Users\REYZEN\Downloads/off1.jpg" alt="">
        </div>
        <div class="slide">
            <img src="C:\Users\REYZEN\Downloads/off2.jpg" alt="">
        </div>
        <div class="slide">
            <img src="C:\Users\REYZEN\Downloads/off3.jpg" alt="">
        </div>
        <div class="slide">
            <img src="C:\Users\REYZEN\Downloads/off4.jpg" alt="">
        </div>
        <div class="slide">
            <img src="C:\Users\REYZEN\Downloads/off5.jpg" alt="">
        </div>
        <div class="slide" id="firstImageDuplicate">
            <img src="C:\Users\REYZEN\Downloads/off1.jpg" alt="">
        </div>
       
    </div>
  
    <div class="dots">
        <div class="dot active"></div>
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
        <div class="dot"></div>
    </div>
</div>
</div>
<script>
    const carouselrow = document.querySelector(".slideRow");
    const carouselslide = document.getElementsByClassName("slide");
    const dots = document.getElementsByClassName("dot");
    const nextbtnx = document.querySelector(".nextx");
    const backbtnx = document.querySelector(".backx");

    let index = 1;
     
     width = carouselslide[0].clientWidth;
     carouselrow.style.transform = 'translateX('+(-width * index)+'px)';

     nextbtnx.addEventListener("click" ,nextSlide);
        function nextSlide(){
            if(index>=carouselslide.length-1){return};
            carouselrow.style.transition = 'transform 0.5s ease-out';
            index++;
            carouselrow.style.transform = 'translateX('+(-width * index)+'px)';
            dotLable();

        }

    backbtnx.addEventListener("click" ,backSlide);
        function backSlide(){
            if(index<=01){return};
            carouselrow.style.transition = 'transform 0.5s ease-out';
            index--;
            carouselrow.style.transform = 'translateX('+(-width * index)+'px)';
           dotLable();


        }

        carouselrow.addEventListener("transitionend",function(){
            if(carouselslide[index].id ==="firstImageDuplicate" ){
                carouselrow.style.transition ="none";
                index=carouselslide.length -index;
                carouselrow.style.transform = 'translateX('+(-width * index)+'px)';
                dotLable();

            }
          
             if(carouselslide[index].id ==="lastImageDuplicate" ){
                carouselrow.style.transition ="none";
                index=carouselslide.length -2;
                carouselrow.style.transform = 'translateX('+( -width * index)+'px)';
                dotLable();

            }
        });
        function autoslide(){
            deleteIntarval = setInterval(timer,1500);
            function timer(){
                nextSlide();
            }
      
        }
        autoslide();

const maincontenar = document.querySelector(".contenarw");

maincontenar.addEventListener("mouseover",function(){
    clearInterval(deleteIntarval);
});
maincontenar.addEventListener("mouseout",autoslide);

function dotLable(){
   for(i=0;i<dots.length;i++){
    dots[i].className = dots[i].className.replace(' active',' ');
   }
   dots[index-1].className += ' active';
}


</script>
    
<!----------------- public riwev ---------------->

<div class="centar" style="font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;">
    <div class="title1" style="margin-bottom: 60px;">
        <h1 id="oh">Top rate</h1>
     
    
    <p id="oP">See all vots &#10095&#10095</p></div>
 </div>

 <div class="mainrow">
    <div class="inmainrow">


<div class="nextrow" >
    <div class="box"> 
        <div class="dpbox">
            <div class="dp">
                <img src="C:\Users\REYZEN\Downloads/2009.jpg" alt="" >
                <div class="info">
                <h3>Josefjeny@1</h3>
                <div class="ret">
                    <i class="fa fa-star"></i>
                    <i class="fa fa-star"></i>
                    <i class="fa fa-star"></i>
                    <i class="fa-solid fa-star-half-stroke"></i>
                    <i class="fa-regular fa-star"></i>
                </div>
                </div>
                

        </div>
        </div>
        <div class="pera">

            <p>this is offer bar and it for sell
                Book any ​domestic one-way flight or hotel of your
                 choice from 12 noon onwards, till limited bookings last.
                </p>



                <div class="inpera">
                    <i class="fa-solid fa-thumbs-up fa-xl" style=" position: absolute; margin-left: 10px; margin-top: 100px; color: rgb(3, 170, 17);"></i>
                    <p style="margin-left: 40px;margin-top: 90px;position: absolute;">2.3k</p>
                    <i class="fa-solid fa-thumbs-down fa-xl" style=" position: absolute; margin-left: 90px; margin-top: 100px; color: rgb(170, 3, 3);"></i>
                    <p style="margin-left: 120px;margin-top: 90px;position: absolute;">100</p>
                    <p id="PX1">Comments&#10095</p>
                </div>
               
      
        </div>

        
    
    
</div>
    <div class="box"> 
        <div class="dpbox">
            <div class="dp">
                <img src="C:\Users\REYZEN\Downloads/2011.jpg" alt="" >
                <div class="info">

                    <h3>Josefjeny@1</h3>
                    <div class="ret">
                        <i class="fa fa-star"></i>
                        <i class="fa fa-star"></i>
                        <i class="fa fa-star"></i>
                        <i class="fa-solid fa-star-half-stroke"></i>
                        <i class="fa-regular fa-star"></i>
                    </div>
                </div>
              

        </div>
        </div>
        <div class="pera">

            <p>this is offer bar and it for sell
                Book any ​domestic one-way flight or hotel of your
                 choice from 12 noon onwards, till limited bookings last.
               </p>
               <div class="inpera">
               <i class="fa-solid fa-thumbs-up fa-xl" style=" position: absolute; margin-left: 10px; margin-top: 100px; color: rgb(3, 170, 17);"></i>
               <p style="margin-left: 40px;margin-top: 90px;position: absolute;">2.3k</p>
               <i class="fa-solid fa-thumbs-down fa-xl" style=" position: absolute; margin-left: 90px; margin-top: 100px; color: rgb(170, 3, 3);"></i>
               <p style="margin-left: 120px;margin-top: 90px;position: absolute;">100</p>
               <p id="PX1">Comments&#10095</p> </div>
     
    
    
            </div>
            </div>
    
  
<div class="box" id="boxPX"> 
    <div class="dpbox">
        <div class="dp">
            <img src="C:\Users\REYZEN\Downloads/2010.jpg" alt="" >
            <div class="info">
                <h3>Josefjeny@1</h3>
                <div class="ret">
                    <i class="fa fa-star"></i>
                    <i class="fa fa-star"></i>
                    <i class="fa fa-star"></i>
                    <i class="fa-solid fa-star-half-stroke"></i>
                    <i class="fa-regular fa-star"></i>
                </div>
            </div>
               
           

    </div>
    </div>
    <div class="pera">

        <p>this is offer bar and it for sell
            Book any ​domestic one-way flight or hotel of your
             choice from 12 noon onwards, till limited bookings last.
         </p>
         <div class="inpera">
         <i class="fa-solid fa-thumbs-up fa-xl" style=" position: absolute; margin-left: 10px; margin-top: 100px; color: rgb(3, 170, 17);"></i>
         <p style="margin-left: 40px;margin-top: 90px;position: absolute;">2.3k</p>
         <i class="fa-solid fa-thumbs-down fa-xl" style=" position: absolute; margin-left: 90px; margin-top: 100px; color: rgb(170, 3, 3);"></i>
         <p style="margin-left: 120px;margin-top: 90px;position: absolute;">100</p>
         <p id="PX1">Comments&#10095</p> </div>
 



</div>

</div>
    
</div>
</div>
</div>
<!-- ----------------------------last colome----------------------------  -->
<!-- ----------------------------list box----------------------------  -->

<div class="details">

    <div class="perent_box">

        <div class="lbox">
            <h3>PASS CATEGORIES</h3>
            <div class="list">
                <ul>
                    <li>Silvar Pass</li>
                    <li>Gold Pass</li>
                    <li>Platinum Ppass</li>
                    
                </ul>
        
        
            </div>
           
        </div>
        <div class="lbox">
            <h3>HELP</h3>
            <div class="list">
                <ul>
                    <li>Returns</li>
                    <li>Secure Ppayments</li>
                    <li>Payments Method</li>
                    <li>Contact US</li>
                </ul>
        
        
            </div>
           
        </div>
        <div class="lbox">
            <h3>ABOUT US</h3>
            <div class="list">
                <ul>
                    <li>Careers</li>
                    <li>Terms & Conditions</li>
                    <li>Privacy Policy</li>
                    <li>Responsibility</li>
                </ul>
        
        
            </div>
           
        </div>
        <div class="lbox">
            <h3>FEEDBACK</h3>
            <div class="list">
                <ul>
                    <li>Leave a feedback</li>
                    
                </ul>
        
        
            </div>
           
        </div>
    </div>

    <!-- ----------------------------socialinfo box----------------------------  -->
    <div class="mbox">

        <div class="tbox">
     
          <div class="dataa1">
            <h3>FIND A COLLAGE</h3>
            <p>Locete a collage on map</p>
            <a href="" class="collage" style="font-size: large;">COLLAGE LOCATOR</a>
       
          </div>
        </div>
          <div class="tbox">
     
            <div class="dataa2">
              <h3>FOLLOW US</h3>
              <div class="follow_icone">
                <a href=""><i class="fa-brands fa-google fa-xl"></i></a>
                 
                <a href=""><i class="fa-brands fa-facebook fa-xl"></i></a>
     
                <a href=""> <i class="fa-brands fa-instagram fa-xl"></i></a>
      
                <a href=""><i class="fa-brands fa-linkedin-in fa-xl" ></i></a>

              </div>
          
               
         
  
            </div>
        </div>
            <div class="tbox">
     
                <div class="dataa3">
                  <h3>Alert ME</h3>
                  <p> updates in your inbox...</p>
                <div class="text">
                    <input type="email" placeholder="Email Id">
                    <label><button>Go</button></label>
                </div>
                 
                </div>
            </div>
       
    </div>


</div>

</body>
</html>
