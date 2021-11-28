<template>
  <div style="height: 95%">
    <span class="fontawesome-legend"> Fontawesome icons</span>
    <span> | </span>
    <span class="bootstrap-legend"> Bootstrap icons</span>
    <span> | </span>
    <span class="mdi-legend"> Material design icons</span>
    <vue-pdf-app pdf="sample.pdf"></vue-pdf-app>
  </div>
</template>

<script>
// VuePdfApp component is registered in src/main.js

export default {
  name: "IconsCustomization",
};
</script>

<style scoped>
/* ****** Fontawesome icons ****** */
>>> #toolbarViewerLeft .vue-pdf-app-icon::before,
>>> #toolbarViewerLeft .vue-pdf-app-icon::after,
.fontawesome-legend::before {
  font-family: "Font Awesome 5 Free";
  color: red;
}

>>> .vue-pdf-app-icon.page-up::before {
  content: "\f19c";
}

>>> .vue-pdf-app-icon.page-down::before {
  content: "\f14a";
}

>>> .vue-pdf-app-icon.view-find::before {
  content: "\f024";
}

>>> .vue-pdf-app-icon.sidebar-toggle::before,
.fontawesome-legend::before {
  content: "\f1d8";
}

/* ****** Material design icons ****** */
>>> #toolbarViewerRight .vue-pdf-app-icon::before,
>>> #toolbarViewerRight .vue-pdf-app-icon::after,
.mdi-legend::before {
  font-family: "Material Design Icons";
  color: mediumseagreen;
}

>>> .vue-pdf-app-icon.presentation-mode::before {
  content: "\f07b4";
}

>>> .vue-pdf-app-icon.print-button::before {
  content: "\f07c9";
}

>>> .vue-pdf-app-icon.open-file::before {
  content: "\f0ad4";
}

>>> .vue-pdf-app-icon.download-button::before {
  content: "\f0bca";
}

>>> .vue-pdf-app-icon.secondary-toolbar-toggle::before {
  content: "\f0031";
}

>>> .vue-pdf-app-icon.bookmark-button::before,
.mdi-legend::before {
  content: "\f0021";
}

/* ****** Bootstrap icons ****** */
>>> #toolbarViewerMiddle .vue-pdf-app-icon::before,
>>> #toolbarViewerMiddle .vue-pdf-app-icon::after,
.bootstrap-legend::before {
  font-family: "bootstrap-icons";
  color: orange;
}

>>> .vue-pdf-app-icon.dropdown-toolbar-button::after {
  content: "\f1d5";
}

>>> .vue-pdf-app-icon.zoom-out::before {
  content: "\f18c";
}

>>> .vue-pdf-app-icon.zoom-in::before,
.bootstrap-legend::before {
  content: "\f15c";
}
</style>
