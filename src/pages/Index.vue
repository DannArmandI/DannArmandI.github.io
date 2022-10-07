<template>
  <div>
    <div class="page-header clear-filter" filter-color="orange">
      <parallax class="page-header-image"> </parallax>
      <div class="container">
        <div class="content-center brand">
          <img class="n-logo" src="img/logoBlanco.png" alt="" />
          <!-- <h1 class="h1-seo">Brics 21</h1> -->
          <h3>Soluciones Tecnologicas Y Digitales Para Tu Negocio</h3>
        </div>
        <!-- <h6 class="category category-absolute">
          Designed by
          <a href="http://invisionapp.com/" target="_blank">
            <img src="img/invision-white-slim.png" class="invision-logo" /> </a
          >. Coded by
          <a href="https://www.creative-tim.com" target="_blank">
            <img
              src="img/creative-tim-white-slim2.png"
              class="creative-tim-logo"
            /> </a
          >.
        </h6> -->
      </div>
    </div>
    <div class="main">
      <!-- <div class="section section-images">
        <div class="container">
          <div class="row">
            <div class="col-md-12">
              <div class="hero-images-container">
                <img src="img/hero-image-1.png" alt="" />
              </div>
              <div class="hero-images-container-1">
                <img src="img/hero-image-2.png" alt="" />
              </div>
              <div class="hero-images-container-2">
                <img src="img/hero-image-3.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div> -->
      <div id="who" class="section section-about-us">
        <div class="container">
          <div class="row">
            <div class="col-md-8 ml-auto mr-auto text-center">
              <h2 class="title">¿Quienes Somos?</h2>
              <h5 class="description" style="color: #2c2c2c">
                Brics es una empresa de desarrollo de soluciones tecnológicas
                que se enfoca en la construcción de sistemas digitales para
                medianas y grandes empresas. Brics es un concepto que se asemeja
                fonéticamente a “ladrillo” en inglés. El objetivo es ir
                aportando ladrillo a ladrillo al Roadmap Tecnológico de nuestros
                clientes. El 21 identifica el distrito 21 en el cual se
                encuentran las oficinas de Brics21
              </h5>
            </div>
          </div>
          <div class="separator separator-primary"></div>
          <div class="section-story-overview">
            <div class="row">
              <div class="col-md-6">
                <div
                  class="image-container image-left"
                  style="background-image: url('img/3.webp')"
                >
                  <!-- First image on the left side -->
                  <p
                    id="service"
                    class="blockquote blockquote-primary"
                    style="width: 230px"
                  >
                    <!-- <strong>-Mision</strong> -->
                    <!-- <br /> -->
                    Diseñamos, construimos e implementamos plataformas y
                    productos digitales junto a nuestros partners para alcanzar
                    sus objetivos estratégicos por medio de soluciones
                    tecnológicas.
                  </p>
                </div>
                <!-- Second image on the left side of the article -->
                <div
                  class="image-container"
                  style="background-image: url('img/2.webp')"
                ></div>
              </div>
              <div class="col-md-5">
                <!-- First image on the right side, above the article -->
                <div
                  class="image-container image-right"
                  style="background-image: url('img/1.webp')"
                ></div>
                <h3>Nuestros productos y servicios</h3>
                <p>
                  <strong>Inteligencia artificial:</strong> Soluciones basadas
                  en mecanismo y algoritmos de inteligencia artificial. Ya sean
                  predicciones, clasificación o categorización de personas u
                  objetos, reconocimiento de caracteres, entre otras muchas
                  otras.
                </p>
                <p>
                  <strong>Automatización:</strong> También podemos ofrecer
                  software de automatización. Por ejemplo, soluciones de
                  automatización de proceso industriales, generación de
                  reportes, bots de comunicación y generación de alertas.
                </p>
                <p>
                  <strong>Aplicaciones móviles:</strong> Aplicativos móviles
                  para distintos dispositivos.
                </p>
                <p>
                  <strong>Integraciones:</strong> Por otro lado, contamos con
                  experiencia en integraciones de sistemas digitales y redes
                  sociales, así que es un servicio que como Brics también
                  podemos ofrecer.
                </p>
                <p>
                  <strong>Bases de datos y continuidad operativa:</strong> De
                  igual forma con bases de datos y continuidad operativa. Que
                  son dos servicios que muchas empresas desconocen como una
                  necesidad hasta que se encuentran con ella. Como equipo
                  podemos gestionar bases de datos y ofrecer administración de
                  sistemas digitales.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- <basic-elements></basic-elements>
    <navigation></navigation>
    <tabs-section></tabs-section>
    <progress-pagination></progress-pagination>
    <notifications></notifications>
    <typography></typography>
    <javascript-components></javascript-components>
    <carousel-section></carousel-section>
    <nucleo-icons-section></nucleo-icons-section> -->
    <!-- <div class="section">
      <div class="container text-center">
        <div class="row justify-content-md-center">
          <div class="col-md-12 col-lg-8">
            <h2 class="title">Completed with examples</h2>
            <h5 class="description">
              The kit comes with three pre-built pages to help you get started
              faster. You can change the text and images and you're good to go.
              More importantly, looking at them will give you a picture of what
              you can built with this powerful Bootstrap 4 ui kit.
            </h5>
          </div>
        </div>
      </div>
    </div> -->
    <examples-section></examples-section>
    <team-develop/>
    <signup-form></signup-form>
    <!-- <download-section></download-section> -->
  </div>
</template>
<script>
import { Parallax } from "@/components";
import BasicElements from "./components/BasicElementsSection";
import Navigation from "./components/Navigation";
import TabsSection from "./components/Tabs";
import ProgressPagination from "./components/ProgressPagination";
import Notifications from "./components/Notifications";
import Typography from "./components/Typography";
import JavascriptComponents from "./components/JavascriptComponents";
import CarouselSection from "./components/CarouselSection";
import NucleoIconsSection from "./components/NucleoIconsSection";
import SignupForm from "./components/SignupForm";
import ExamplesSection from "./components/ExamplesSection";
import DownloadSection from "./components/DownloadSection";
import TeamDevelop from "./components/TeamDevelop.vue";

export default {
  name: "index",
  bodyClass: "index-page",
  components: {
    Parallax,
    // BasicElements,
    // Navigation,
    // TabsSection,
    // ProgressPagination,
    // Notifications,
    // Typography,
    // JavascriptComponents,
    // CarouselSection,
    // NucleoIconsSection,
    SignupForm,
    ExamplesSection,
    TeamDevelop
},
  // created() {
  // const menuItems = document.getElementsByClassName(".nav-item");
  // const article1 = document.getElementById("app");
  // const article2 = document.getElementById("who");
  // const article3 = document.getElementById("article-3");
  // const article4 = document.getElementById("article-4");

  // const removeActiveMenuItem = () => {
  //   menuItems.forEach((item) =>
  //     item.classList.remove("main-menu__item--active")
  //   );
  // };

  // const addActiveMenuItem = (index) => {
  //   removeActiveMenuItem();
  //   menuItems[index].classList.add("main-menu__item--active");
  // };

  // const checkElement = (element) =>
  //   element.getBoundingClientRect().top > 0 &&
  //   element.getBoundingClientRect().top < 200;

  // window.addEventListener("scroll", () => {
  //   if (checkElement(article1)) {
  //     addActiveMenuItem(article1.dataset.index);
  //   } else if (checkElement(article2)) {
  //     addActiveMenuItem(article2.dataset.index);
  //   } else if (checkElement(article3)) {
  //     addActiveMenuItem(article3.dataset.index);
  //   } else if (checkElement(article4)) {
  //     addActiveMenuItem(article4.dataset.index);
  //   }
  // });
  // },
};
</script>
<style></style>
