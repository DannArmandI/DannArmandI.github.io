<template>
  <div>
    <navbar
      position="fixed"
      type="primary"
      :transparent="transparent"
      :color-on-scroll="colorOnScroll"
      menu-classes="ml-auto"
    >
      <template>
        <router-link
          v-popover:popover1
          class="navbar-brand"
          to="/"
          style="padding: 0"
        >
          <img src="img/logoBlanco.png" alt="" style="max-width: 82px" />
        </router-link>
        <!-- <el-popover
        ref="popover1"
        popper-class="popover"
        placement="bottom"
        width="200"
        trigger="hover"
      >
        <div class="popover-body">
          Designed by Invision. Coded by Creative Tim
        </div>
      </el-popover> -->
      </template>
      <template slot="navbar-menu">
        <li class="nav-item">
          <a class="nav-link" href="#">
            <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
            <p>Inicio</p>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#who">
            <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
            <p>¿Quienes Somos?</p>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#service">
            <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
            <p>Servicios</p>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#contact">
            <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
            <p>Contatanos</p>
          </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#projects">
            <!-- <i class="now-ui-icons arrows-1_cloud-download-93"></i> -->
            <p>Proyectos</p>
          </a>
        </li>
        <!-- <drop-down
        tag="li"
        title="Components"
        icon="now-ui-icons design_app"
        class="nav-item"
      >
        <nav-link to="/">
          <i class="now-ui-icons business_chart-pie-36"></i> ¿Quienes Somos?
        </nav-link>
        <a
          href="https://demos.creative-tim.com/vue-now-ui-kit/documentation"
          target="_blank"
          class="dropdown-item"
        >
          <i class="now-ui-icons design_bullet-list-67"></i> Documentation
        </a>
      </drop-down> -->
        <!-- <drop-down
        tag="li"
        title="Examples"
        icon="now-ui-icons design_image"
        class="nav-item"
      >
        <nav-link to="/landing">
          <i class="now-ui-icons education_paper"></i> Landing
        </nav-link>
        <nav-link to="/login">
          <i class="now-ui-icons users_circle-08"></i> Login
        </nav-link>
        <nav-link to="/profile">
          <i class="now-ui-icons users_single-02"></i> Profile
        </nav-link>
      </drop-down> -->
        <li class="nav-item">
          <a
            class="nav-link btn btn-neutral"
            v-on:click="modals.mini = true"
            href="javascript:void(0)"
          >
            <!-- <i class="now-ui-icons arrows-1_share-66"></i> -->
            <p>Iniciar Sesion</p>
          </a>
        </li>

        <li class="nav-item">
          <a
            class="nav-link"
            rel="tooltip"
            title="Follow us on Twitter"
            data-placement="bottom"
            href=""
            target="_blank"
          >
            <i class="fab fa-twitter"></i>
            <p class="d-lg-none d-xl-none">Twitter</p>
          </a>
        </li>
        <li class="nav-item">
          <a
            class="nav-link"
            rel="tooltip"
            title="Like us on Facebook"
            data-placement="bottom"
            href=""
            target="_blank"
          >
            <i class="fab fa-facebook-square"></i>
            <p class="d-lg-none d-xl-none">Facebook</p>
          </a>
        </li>
        <li class="nav-item">
          <a
            class="nav-link"
            rel="tooltip"
            title="Follow us on Instagram"
            data-placement="bottom"
            href=""
            target="_blank"
          >
            <i class="fab fa-instagram"></i>
            <p class="d-lg-none d-xl-none">Instagram</p>
          </a>
        </li>
      </template>
    </navbar>
    <modal
      :show.sync="modals.mini"
      class="modal-primary"
      :show-close="false"
      headerClasses="justify-content-center"
      type="mini"
    >
      <card class="card-signup" header-classes="text-center" color="orange">
        <template slot="header">
          <div class="modal-profile" style="margin: 0 auto">
            <i class="now-ui-icons users_circle-08"></i>
          </div>
          <h3 class="card-title title-up">Login</h3>
        </template>
        <template>
          <fg-input
            class="no-border"
            placeholder="Email"
            addon-left-icon="now-ui-icons ui-1_email-85"
          >
          </fg-input>
          <fg-input
            class="no-border"
            placeholder="Contrasena"
            addon-left-icon="now-ui-icons text_caps-small"
          >
          </fg-input>
        </template>
        <div class="card-footer text-center">
          <n-button
            type="default"
            round
            size="lg"
            v-on:click="modals.mini = false"
            >Cerrar</n-button
          >
          <n-button type="neutral" round size="lg" v-on:click="LogIn()"
            >Iniciar</n-button
          >
        </div>
      </card>
    </modal>
  </div>
</template>

<script>
import {
  DropDown,
  Navbar,
  NavLink,
  Modal,
  Button,
  FormGroupInput,
  Card,
} from "@/components";
import { Popover } from "element-ui";
export default {
  name: "main-navbar",
  props: {
    transparent: Boolean,
    colorOnScroll: Number,
  },
  components: {
    // DropDown,
    Card,
    Navbar,
    // NavLink,
    [Button.name]: Button,
    [Popover.name]: Popover,
    [FormGroupInput.name]: FormGroupInput,
    Modal,
  },
  data() {
    return {
      modals: {
        classic: false,
        mini: false,
      },
    };
  },
  methods: {
    LogIn() {
      this.$router.push('/dashboard')
    },
  },
};
</script>

<style scoped></style>
