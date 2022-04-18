<template lang="pug">
header.hero.MajorMono.bg-gray
  .container
    .row
      .col
        h1.hero-headline Fernando Cárdenas
    .row
      .col-md-4.offset-md-4
        p.hero-copy Full Stack
          br/
          strong &#123;&#123; Web & Mobile &#125;&#125;
          br/ Developer
    .row
      .col-md-4.offset-md-4
        figure
          img.logo(src="@/assets/logo.webp")

    .row
      .col-md-4.offset-md-4
        p.text-center.SourceCodePro
          a.active(href="mailto:hola@ferca.dev") hola@ferca.dev
        p.text-center.SourceCodePro
          a.active(href="https://github.com/cardenas413") github.com/cardenas413 (+140 Projects)
        p.text-center.SourceCodePro
          strong Ing. en Tecnologías de la Información y Comunicaciones
          br/
          small Escuela de Sistemas UT, UA de C
        hr
        p.text-center.SourceCodePro
          strong Professional in Game Development
          br/
          small Specialising in Game Programming
          br/
          | National Institute of Information Technology
        hr
        p.text-center.SourceCodePro
          strong Adobe Certified Associate
          br/
          small Web Communication Using Adobe Dreamweaver
          br/
          | Certiport
        hr
        p.text-center.SourceCodePro
          strong Microsoft Partner Network
          br/
          small Gorilas Online (Co-Founder)
          br/
          | Microsoft 2018
        hr
        p.text-center.SourceCodePro
          strong Developer Certification
          br/
          small PayPal México
        hr
        p.text-center.SourceCodePro
          strong Skills
          br/
          small PHP (6 Years)
          br/
          small VUE / JS (4 Years)
          br/
          small CSS / SCSS / Vuex
          br/
          small GIT / TS / Sass / i18n Generator
          br/
          small Laravel / Echo / Mix / Sanctum
          br/
          small pug / GraphQL / Apollo / Bootstrap
          br/
          small Linux / Windows / MacOs
          br/
          | MySQL
        hr
</template>

<script lang="ts">
import {defineComponent} from 'vue'

export default defineComponent({
  data() {
    return {
      /*wHeight: "60vh",
      navigator: {
        justifyContents: {
          left: {
            float: "initial",
            justify: "center",
          },
          center: {
            float: "initial",
            justify: "center",
          },
          right: {
            float: "initial",
            justify: "center",
          },
        },
        logo: {
          maxWidth: "250px",
          marginTop: "",
        },
        heroHeadLine: {
          fontSize: "",
          marginTop: "",
        },
        heroCopy: {
          fontSize: ""
        }
      }*/
    }
  },
  computed: {
    //width() {
    //  return (window.innerWidth > 0) ? window.innerWidth : screen.width;
    //}
  },
  mounted() {
    //if (this.width < 991) {
    //  this.navigator.heroHeadLine.fontSize = "1.7rem";
    //} else {
    //  this.navigator.heroHeadLine.fontSize = "5rem";
    //}

    //window.addEventListener('scroll', this.handleScroll);
  },
  methods: {
    /*handleScroll(event: Event) {
      if (document.body.scrollTop > 10 || document.documentElement.scrollTop > 10) {

        if (this.width < 991) {
          this.wHeight = "0px";
          this.navigator = {
            justifyContents: {
              left: {
                float: "initial",
                justify: "center",
              },
              center: {
                float: "initial",
                justify: "center",
              },
              right: {
                float: "initial",
                justify: "center",
              },
            },
            logo: {
              maxWidth: "0px",
              marginTop: "",
            },
            heroHeadLine: {
              fontSize: "1.3rem",
              marginTop: "",
            },
            heroCopy: {
              fontSize: "1rem"
            }
          }
        } else {
          this.wHeight = "0px";
          this.navigator = {
            justifyContents: {
              left: {
                float: "left",
                justify: "flex-start",
              },
              center: {
                float: "none",
                justify: "center",
              },
              right: {
                float: "right",
                justify: "flex-end",
              },
            },
            logo: {
              maxWidth: "60px",
              marginTop: "10px",
            },
            heroHeadLine: {
              fontSize: "1.3rem",
              marginTop: "28px",
            },
            heroCopy: {
              fontSize: "1rem"
            }
          }
        }
      } else {

        if (this.width < 991) {
          this.wHeight = "60vh";
          this.navigator = {
            justifyContents: {
              left: {
                float: "initial",
                justify: "center",
              },
              center: {
                float: "initial",
                justify: "center",
              },
              right: {
                float: "initial",
                justify: "center",
              },
            },
            logo: {
              maxWidth: "250px",
              marginTop: "",
            },
            heroHeadLine: {
              fontSize: "1.7rem",
              marginTop: "",
            },
            heroCopy: {
              fontSize: "1.3rem"
            }
          }
        } else {
          this.wHeight = "60vh";

          this.navigator = {
            justifyContents: {
              left: {
                float: "initial",
                justify: "center",
              },
              center: {
                float: "initial",
                justify: "center",
              },
              right: {
                float: "initial",
                justify: "center",
              },
            },
            logo: {
              maxWidth: "250px",
              marginTop: "",
            },
            heroHeadLine: {
              fontSize: "5rem",
              marginTop: "",
            },
            heroCopy: {
              fontSize: "2rem"
            }
          }
        }


      }
    }*/
  }
})


</script>


<style scoped lang="scss">

.hero {
  box-sizing: border-box;
  padding: 2rem;
  transition-duration: .7s;
  width: 100%;
  top: 0px;
  //position: fixed;
}

.hero-headline {
  font-size: 1.5em;
  text-align: center;
  white-space: nowrap;
  margin-bottom: 3vh;
}

.hero-copy {
  font-size: 1em;
  text-align: center;
  margin-bottom: 3vh;

}
.logo{
  width: 180px;
  margin-left: 50%;
  left: -90px;
  position: relative;
}


</style>
