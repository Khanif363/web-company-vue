<template>
          <!-- ======= Header ======= -->
    <header id="header" class="header fixed-top" data-scrollto-offset="0">
      <div class="container-fluid d-flex align-items-center justify-content-between">
  
        <a href="index.html" class="logo d-flex align-items-center scrollto me-auto me-lg-0 ms-3">
          <!-- Uncomment the line below if you also wish to use an image logo -->
          <!-- <img src="./assets/img/logo.png" alt=""> -->
          <!-- <h1>HeroBiz<span>.</span></h1> -->
          <img src="./assets/img/logo-per-removebg-preview.png" alt="">
        </a>
  
        <nav id="navbar" class="navbar">
          <ul>
            <li class="active"><a class="nav-link scrollto " href="index.html">{{ $t("navbar.home") }}</a></li>
            <li><a class="nav-link scrollto" href="index.html#about">{{ $t("navbar.tentang") }}</a></li>
            <!-- <li><a class="nav-link scrollto" href="index.html#komitmen">{{ $t("navbar.komitmen") }}</a></li> -->
            <li><a class="nav-link scrollto" href="index.html#produk">{{ $t("navbar.produk") }}</a></li>
            <li><a class="nav-link scrollto" href="index.html#contact">{{ $t("navbar.kontak") }}</a></li>
            <div class="nav-link scrollto">
              <select v-model="language" @change="changeLanguage" class="custome-select" style="border-radius:20px;">
                <option value="id">Indonesia</option>
                <option value="en">English</option>
                <option value="man">中文</option>
              </select>
            </div>
          </ul>
          <i class="bi bi-list mobile-nav-toggle d-none"></i>
        </nav><!-- .navbar -->
  
        <!-- <a class="btn-getstarted scrollto" href="index.html#about">Get Started</a> -->
  
      </div>
    </header><!-- End Header -->
    <section id="hero-animated" class="hero-animated d-flex align-items-center">
      <div class="container d-flex flex-column justify-content-center align-items-center text-center position-relative" data-aos="zoom-out">
        <img src="./assets/img/design-awal.png" class="img-fluid animated">
        <h2>{{ $t("home.judul") }} <span>{{ $t("home.judulSpan") }}</span></h2>
        <p>{{ $t("home.slogan") }}</p>
        <div class="d-flex">
          <!-- <a href="#about" class="btn-get-started scrollto">Get Started</a> -->
          <a href="https://www.youtube.com/watch?v=LXb3EKWsInQ" class="glightbox btn-watch-video d-flex align-items-center"><i class="bi bi-play-circle"></i><span>{{ $t("home.tonton") }}</span></a>
        </div>
      </div>
    </section>
  
    <main id="main">
  

      <!-- ======= About Section ======= -->
      <section id="about" class="about">
        <div class="container" data-aos="fade-up">
  
          <div class="section-header">
            <h2>{{ $t("tentang.tentang") }}</h2>
            <p>{{ $t("tentang.desc") }}</p>
          </div>
  
          <div class="row g-4 g-lg-5" data-aos="fade-up" data-aos-delay="200">
  
            <div class="col-lg-5">
              <div class="">
                <img src="./assets/img/vsi.png" style="border-radius: 1%;" class="img-fluid" alt="">
              </div>
            </div>
  
            <div class="col-lg-7 ">
              <h3 class="pt-0 pt-lg-5 text-center">{{ $t("tentang.judulvisi") }}</h3>
  
              <!-- Tabs -->
              <ul class="nav nav-pills ms-4 mb-3">
                <li><a class="nav-link active" data-bs-toggle="pill" href="#tab1">{{ $t("tentang.visi") }}</a></li>
                <li><a class="nav-link" data-bs-toggle="pill" href="#tab2">{{ $t("tentang.misi") }}</a></li>
                <li><a class="nav-link" data-bs-toggle="pill" href="#tab3">{{ $t("tentang.tujuan") }}</a></li>
              </ul><!-- End Tabs -->
  
              <!-- Tab Content -->
              <div class="tab-content ms-4 mr-4">
  
                <div class="tab-pane fade show active" id="tab1">
  
                  <!-- <p class="fst-italic">Consequuntur inventore voluptates consequatur aut vel et. Eos doloribus expedita. Sapiente atque consequatur minima nihil quae aspernatur quo suscipit voluptatem.</p> -->
  
                  <!-- <div class="d-flex align-items-center mt-4">
                    <i class="bi bi-check2"></i>
                    <h4>Repudiandae rerum velit modi et officia quasi facilis</h4>
                  </div> -->
                  <p class="mt-5">{{ $t("tentang.descVisi") }}</p>
  
  
                </div><!-- End Tab 1 Content -->
  
                <div class="tab-pane fade show" id="tab2">
                  <p class="mt-5"><ol>
                    <li>{{ $t("tentang.descMisi1") }}</li>
                    <li>{{ $t("tentang.decsMisi2") }}</li>
                  </ol></p>
                </div><!-- End Tab 2 Content -->
  
                <div class="tab-pane fade show" id="tab3">
                  <p class="mt-5">
                    <ol>
                      <li>{{ $t("tentang.desctujuan1") }}</li>
                      <li>{{ $t("tentang.desctujuan2") }}</li>
                    </ol>
                  </p>
                </div><!-- End Tab 2 Content -->
                
              </div>
  
            </div>
  
          </div>
  
        </div>
      </section><!-- End About Section -->
  
      <!-- ======= Testimonials Section ======= -->
      <section id="testimonials" class="testimonials">
        <div class="container" data-aos="fade-up">
  
          <div class="testimonials-slider swiper">
            <div class="swiper-wrapper">
  
              <div class="swiper-slide">
                <div class="testimonial-item">
                  <img src="./assets/img/testimonials/testimonials-1.jpg" class="testimonial-img" alt="">
                  <h3>Saul Goodman</h3>
                  <h4>Ceo &amp; Founder</h4>
                  <div class="stars">
                    <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i>
                  </div>
                  <p>
                    <i class="bi bi-quote quote-icon-left"></i>
                    Proin iaculis purus consequat sem cure digni ssim donec porttitora entum suscipit rhoncus. Accusantium quam, ultricies eget id, aliquam eget nibh et. Maecen aliquam, risus at semper.
                    <i class="bi bi-quote quote-icon-right"></i>
                  </p>
                </div>
              </div><!-- End testimonial item -->
  
              <div class="swiper-slide">
                <div class="testimonial-item">
                  <img src="./assets/img/testimonials/testimonials-2.jpg" class="testimonial-img" alt="">
                  <h3>Sara Wilsson</h3>
                  <h4>Designer</h4>
                  <div class="stars">
                    <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i>
                  </div>
                  <p>
                    <i class="bi bi-quote quote-icon-left"></i>
                    Export tempor illum tamen malis malis eram quae irure esse labore quem cillum quid cillum eram malis quorum velit fore eram velit sunt aliqua noster fugiat irure amet legam anim culpa.
                    <i class="bi bi-quote quote-icon-right"></i>
                  </p>
                </div>
              </div><!-- End testimonial item -->
  
              <div class="swiper-slide">
                <div class="testimonial-item">
                  <img src="./assets/img/testimonials/testimonials-3.jpg" class="testimonial-img" alt="">
                  <h3>Jena Karlis</h3>
                  <h4>Store Owner</h4>
                  <div class="stars">
                    <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i>
                  </div>
                  <p>
                    <i class="bi bi-quote quote-icon-left"></i>
                    Enim nisi quem export duis labore cillum quae magna enim sint quorum nulla quem veniam duis minim tempor labore quem eram duis noster aute amet eram fore quis sint minim.
                    <i class="bi bi-quote quote-icon-right"></i>
                  </p>
                </div>
              </div><!-- End testimonial item -->
  
              <div class="swiper-slide">
                <div class="testimonial-item">
                  <img src="./assets/img/testimonials/testimonials-4.jpg" class="testimonial-img" alt="">
                  <h3>Matt Brandon</h3>
                  <h4>Freelancer</h4>
                  <div class="stars">
                    <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i>
                  </div>
                  <p>
                    <i class="bi bi-quote quote-icon-left"></i>
                    Fugiat enim eram quae cillum dolore dolor amet nulla culpa multos export minim fugiat minim velit minim dolor enim duis veniam ipsum anim magna sunt elit fore quem dolore labore illum veniam.
                    <i class="bi bi-quote quote-icon-right"></i>
                  </p>
                </div>
              </div><!-- End testimonial item -->
  
              <div class="swiper-slide">
                <div class="testimonial-item">
                  <img src="./assets/img/testimonials/testimonials-5.jpg" class="testimonial-img" alt="">
                  <h3>John Larson</h3>
                  <h4>Entrepreneur</h4>
                  <div class="stars">
                    <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i>
                  </div>
                  <p>
                    <i class="bi bi-quote quote-icon-left"></i>
                    Quis quorum aliqua sint quem legam fore sunt eram irure aliqua veniam tempor noster veniam enim culpa labore duis sunt culpa nulla illum cillum fugiat legam esse veniam culpa fore nisi cillum quid.
                    <i class="bi bi-quote quote-icon-right"></i>
                  </p>
                </div>
              </div><!-- End testimonial item -->
  
            </div>
            <div class="swiper-pagination"></div>
          </div>
  
        </div>
      </section><!-- End Testimonials Section -->
  
      <!-- ======= Pricing Section ======= -->
  
      <!-- ======= F.A.Q Section ======= -->


<section id="produk" class="about">
    <div class="container" data-aos="fade-up">

        <div class="section-header">
            <h2>{{ $t("produk.judul") }}</h2>
            <p>{{ $t("produk.produkdesc") }}</p>
        </div>

        <div data-aos="fade-up" data-aos-delay="200">

          <div class="container">

              <div class="row row-cols-1 row-cols-sm-2 row-cols-md-4 g-3">
                  <div class="col">
                      <div class="card shadow-sm">
                          <img src="./assets/img/aloe.png" alt=""
                              class="bd-placeholder-img card-img-top" width="100%" height="225">
                          <!-- <svg class="bd-placeholder-img card-img-top" width="100%" height="225" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="#55595c"/><text x="50%" y="50%" fill="#eceeef" dy=".3em">Thumbnail</text></svg> -->

                          <div class="card-body">
                              <h5><strong>{{ $t("produk.aloe") }}</strong></h5>
                              <p class="card-text">{{ $t("produk.descaloe") }}</p>
                              <div class="d-flex justify-content-between align-items-center">
                              </div>
                          </div>
                      </div>
                  </div>
                  <div class="col">
                      <div class="card shadow-sm">
                          <img src="./assets/img/betel-nut.png" alt=""
                              class="bd-placeholder-img card-img-top" width="100%" height="225">
                          <!-- <svg class="bd-placeholder-img card-img-top" width="100%" height="225" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="#55595c"/><text x="50%" y="50%" fill="#eceeef" dy=".3em">Thumbnail</text></svg> -->

                          <div class="card-body">
                              <h5><strong>{{ $t("produk.betel") }}</strong></h5>
                              <p class="card-text">{{ $t("produk.descbetel") }}</p>
                              <div class="d-flex justify-content-between align-items-center">
                              </div>
                          </div>
                      </div>
                  </div>
                  <div class="col">
                      <div class="card shadow-sm">
                          <img src="./assets/img/lalpari-crove.png" alt=""
                              class="bd-placeholder-img card-img-top" width="100%" height="225">
                          <!-- <svg class="bd-placeholder-img card-img-top" width="100%" height="225" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="#55595c"/><text x="50%" y="50%" fill="#eceeef" dy=".3em">Thumbnail</text></svg> -->

                          <div class="card-body">
                              <h5><strong>{{ $t("produk.lalpari") }}</strong></h5>
                              <p class="card-text">{{ $t("produk.desclalpari") }}</p>
                              <div class="d-flex justify-content-between align-items-center">
                              </div>
                          </div>
                      </div>
                  </div>
                  <div class="col">
                      <div class="card shadow-sm">
                          <img src="./assets/img/coofe-beans.png" alt=""
                              class="bd-placeholder-img card-img-top" width="100%" height="225">
                          <!-- <svg class="bd-placeholder-img card-img-top" width="100%" height="225" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="#55595c"/><text x="50%" y="50%" fill="#eceeef" dy=".3em">Thumbnail</text></svg> -->

                          <div class="card-body">
                              <h5><strong>{{ $t("produk.coffe") }}</strong></h5>
                              <p class="card-text">{{ $t("produk.desccoffe") }}</p>
                              <div class="d-flex justify-content-between align-items-center">
                              </div>
                          </div>
                      </div>
                  </div>
              </div>

          </div>

        </div>

    </div>
</section>




      <!-- ======= Team Section ======= -->
      <section id="team" class="team">
        <div class="container" data-aos="fade-up">
  
          <div class="section-header">
            <h2>Our Team</h2>
            <p>Architecto nobis eos vel nam quidem vitae temporibus voluptates qui hic deserunt iusto omnis nam voluptas asperiores sequi tenetur dolores incidunt enim voluptatem magnam cumque fuga.</p>
          </div>
  
          <div class="row gy-5">
  
            <div class="col-xl-4 col-md-6 d-flex" data-aos="zoom-in" data-aos-delay="200">
              <div class="team-member">
                <div class="member-img">
                  <img src="./assets/img/team/team-1.jpg" class="img-fluid" alt="">
                </div>
                <div class="member-info">
                  <div class="social">
                    <a href=""><i class="bi bi-twitter"></i></a>
                    <a href=""><i class="bi bi-facebook"></i></a>
                    <a href=""><i class="bi bi-instagram"></i></a>
                    <a href=""><i class="bi bi-linkedin"></i></a>
                  </div>
                  <h4>Walter White</h4>
                  <span>Chief Executive Officer</span>
                </div>
              </div>
            </div><!-- End Team Member -->
  
            <div class="col-xl-4 col-md-6 d-flex" data-aos="zoom-in" data-aos-delay="400">
              <div class="team-member">
                <div class="member-img">
                  <img src="./assets/img/team/team-2.jpg" class="img-fluid" alt="">
                </div>
                <div class="member-info">
                  <div class="social">
                    <a href=""><i class="bi bi-twitter"></i></a>
                    <a href=""><i class="bi bi-facebook"></i></a>
                    <a href=""><i class="bi bi-instagram"></i></a>
                    <a href=""><i class="bi bi-linkedin"></i></a>
                  </div>
                  <h4>Sarah Jhonson</h4>
                  <span>Product Manager</span>
                </div>
              </div>
            </div><!-- End Team Member -->
  
            <div class="col-xl-4 col-md-6 d-flex" data-aos="zoom-in" data-aos-delay="600">
              <div class="team-member">
                <div class="member-img">
                  <img src="./assets/img/team/team-3.jpg" class="img-fluid" alt="">
                </div>
                <div class="member-info">
                  <div class="social">
                    <a href=""><i class="bi bi-twitter"></i></a>
                    <a href=""><i class="bi bi-facebook"></i></a>
                    <a href=""><i class="bi bi-instagram"></i></a>
                    <a href=""><i class="bi bi-linkedin"></i></a>
                  </div>
                  <h4>William Anderson</h4>
                  <span>CTO</span>
                </div>
              </div>
            </div><!-- End Team Member -->
  
          </div>
  
        </div>
      </section><!-- End Team Section -->
  
          <!-- ======= Clients Section ======= -->
          <section id="clients" class="clients container"  style = "max-width:90%; height:90%;">
            <div class="container" data-aos="zoom-out">
      
              <div class="clients-slider swiper">
                <div class="swiper-wrapper align-items-center responsive">
                  <div class="swiper-slide" ><img src="./assets/img/clients/client-1.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                  <div class="swiper-slide"><img src="./assets/img/clients/client-2.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                  <div class="swiper-slide"><img src="./assets/img/clients/client-3.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                  <div class="swiper-slide"><img src="./assets/img/clients/client-4.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                  <div class="swiper-slide"><img src="./assets/img/clients/client-5.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                  <div class="swiper-slide"><img src="./assets/img/clients/client-6.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                  <div class="swiper-slide"><img src="./assets/img/clients/client-7.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                  <div class="swiper-slide"><img src="./assets/img/clients/client-8.png" style = "max-width:80%; height:80%;" class="img-fluid" alt=""></div>
                </div>
              </div>
      
            </div>
          </section><!-- End Clients Section -->
      
          <!-- ======= Call To Action Section ======= -->
          <section id="cta" class="cta">
            <div class="container" data-aos="zoom-out">
      
              <div class="row g-5">
      
                <div class="col-lg-8 col-md-6 content d-flex flex-column justify-content-center order-last order-md-first">
                  <h3>{{ $t("kerjasama.kerjasama") }} <em>{{ $t("kerjasama.kerjasamaSpan") }}</em> {{ $t("kerjasama.kerjasamaAkhir") }}</h3>
                  <p>{{ $t("kerjasama.decs") }}</p>
                  <a class="cta-btn align-self-start" href="wa.me/6281513110686">{{ $t("kerjasama.hubungi") }}</a>
                </div>
      
                <div class="col-lg-4 col-md-6 order-first order-md-last d-flex align-items-center">
                  <div class="img">
                    <img src="./assets/img/cta.jpg" alt="" class="img-fluid">
                  </div>
                </div>
      
              </div>
      
            </div>
          </section><!-- End Call To Action Section -->

      <!-- ======= Contact Section ======= -->
      <section id="contact" class="contact">
        <div class="container">
  
          <div class="section-header">
            <h2>{{ $t("kontak.desckontak") }}</h2>
            <p>{{ $t("kontak.decs") }}</p>
          </div>
  
        </div>
  
        <div class="map">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3989.8168746662486!2d109.3153257142695!3d-0.04877493554054083!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e1d59653cd55b01%3A0x594939744ddb8482!2sPT.%20Makmur%20Kita%20Perkasa!5e0!3m2!1sid!2sid!4v1647127453547!5m2!1sid!2sid" frameborder="0" allowfullscreen></iframe>
          <!-- <iframe src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d12097.433213460943!2d-74.0062269!3d40.7101282!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xb89d1fe6bc499443!2sDowntown+Conference+Center!5e0!3m2!1smk!2sbg!4v1539943755621" frameborder="0" allowfullscreen></iframe> -->
        </div><!-- End Google Maps -->
  
        <div class="container">
  
          <div class="row">
  
            <div class="col-lg-5">
  
              <div class="info">
                <h3>{{ $t("kontak.hubungi") }}</h3>
                <p>{{ $t("kontak.deschubungi") }}</p>
  
                <div class="info-item d-flex">
                  <i class="bi bi-geo-alt flex-shrink-0"></i>
                  <div>
                    <h4>{{ $t("kontak.lokasi") }}</h4>
                    <p>{{ $t("kontak.desclokasi") }}</p>
                  </div>
                </div><!-- End Info Item -->
  
                <div class="info-item d-flex">
                  <i class="bi bi-envelope flex-shrink-0"></i>
                  <div>
                    <h4>{{ $t("kontak.email") }}</h4>
                    <p>Makmurkitaperkasa@gmail.com</p>
                  </div>
                </div><!-- End Info Item -->
  
                <div class="info-item d-flex">
                  <i class="bi bi-phone flex-shrink-0"></i>
                  <div>
                    <h4>{{ $t("kontak.kontak") }}</h4>
                    <p>081513110686</p>
                  </div>
                </div><!-- End Info Item -->
  
              </div>
  
            </div>
  
            <div class="col-lg-3 container">
              <div  style="margin-top:40px" class="text-center">
                  <img src="./assets/img/qr-whatsapp.png" alt="">
                  <p class="container text-muted">{{ $t("qr.whatsapp") }}</p>
              </div>
            </div>
 
            <div class="col-lg-3 container">
              <div style="margin-top:40px" class="text-center">
                  <img src="./assets/img/qr-ig.png" alt="">
                  <p class="container text-muted" style="text-size:80%">{{ $t("qr.instagram") }}</p>
              </div>
            </div>
  
          </div>
  
        </div>
      </section><!-- End Contact Section -->
  
    </main><!-- End #main -->
  
    <!-- ======= Footer ======= -->
    <footer id="footer" class="footer">
  
      <div class="footer-content">
        <div class="container">
          <div class="row">
  
            <div class="col-lg-3 col-md-6">
              <div class="footer-info">
                <h3>{{ $t("footer.judul") }}</h3>
                <p>{{ $t("footer.alamat") }}<br><br>
                  <strong>{{ $t("footer.telepon") }}</strong> 081513110686<br>
                  <strong>{{ $t("footer.email") }}</strong> Makmurkitaperkasa@gmail.com<br>
                </p>
              </div>
            </div>
  
            <div class="col-lg-2 col-md-6 footer-links">
              <h4>Link</h4>
              <ul>
                <li><i class="bi bi-chevron-right"></i> <a href="index.html">{{ $t("navbar.home") }}</a></li>
                <li><i class="bi bi-chevron-right"></i> <a href="#about">{{ $t("navbar.tentang") }}</a></li>
                <li><i class="bi bi-chevron-right"></i> <a href="#komitmen">{{ $t("navbar.komitmen") }}</a></li>
                <li><i class="bi bi-chevron-right"></i> <a href="#produk">{{ $t("navbar.produk") }}</a></li>
                <li><i class="bi bi-chevron-right"></i> <a href="#contact">{{ $t("navbar.kontak") }}</a></li>
              </ul>
            </div>
  
            <!-- <div class="col-lg-3 col-md-6 footer-links">
              <h4>Layanan Kami</h4>
              <ul>
                <li><i class="bi bi-chevron-right"></i> <a href="#">Product Management</a></li>
              </ul>
            </div> -->
          </div>
        </div>
      </div>
  
      <div class="footer-legal text-center">
        <div class="container d-flex flex-column flex-lg-row justify-content-center justify-content-lg-between align-items-center">
  
          <div class="d-flex flex-column align-items-center align-items-lg-start">
            <div class="copyright">
              &copy; Copyright <strong><span>PT. Makmur Kita Perkasa</span></strong>. All Rights Reserved
            </div>
            <div class="credits">
              Didesain oleh <a href="https://bootstrapmade.com/">Khanif</a>
            </div>
          </div>
  
          <div class="social-links order-first order-lg-last mb-3 mb-lg-0">
            <a href="https://wa.me/6281513110686" target="_blank" class="whatsapp"><i class="bi bi-whatsapp"></i></a>
            <a href="https://instagram.com/makmurkitaperkasa?utm_medium=copy_link" target="_blank" class="instagram"><i class="bi bi-instagram"></i></a>
            <a href="https://www.facebook.com/profile.php?id=100078992497598" target="_blank" class="facebook"><i class="bi bi-facebook"></i></a>
          </div>
  
        </div>
      </div>
  
    </footer><!-- End Footer -->
  
    <a href="#" class="scroll-top d-flex align-items-center justify-content-center"><i class="bi bi-arrow-up-short"></i></a>
    <div id="preloader"></div>
  
</template>

<script>
export default {
  data() {
    return{
      language: null,
    }
  },
  methods: {
    changeLanguage(){
      localStorage.setItem("lang", this.language)
      window.location.reload()
    }
  },
  created(){
    if(localStorage.getItem("lang") == null) {
      localStorage.setItem("lang", "id")
    }
    this.language = localStorage.getItem("lang")
  }
}
</script>

<style>
</style>
