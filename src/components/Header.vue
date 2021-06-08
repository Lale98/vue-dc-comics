<template>
  <div>
      <nav>
          <section id="logo">
              <img src="../assets/img/dc-logo.png" alt="logo">
          </section>
          <section id="pages">
              <ul>
                  <li v-for="(link,index) in links" :key="index" :class="{active : link.current}"> {{ link.text }} </li>
              </ul>
          </section>
      </nav>
  </div>
</template>

<script>

export default {
    name : "Header",
    data : function () {
        return {
            links : [
                {
                    text :"CHARACTERS",
                    current: false,
                    url: "/"
                },
                {
                    text :"COMICS",
                    current: true,
                    url: "/"
                },
                {
                    text :"MOVIES",
                    current: false,
                    url: "/"
                },
                {
                    text :"TV",
                    current: false,
                    url: "/"
                },
                {
                    text :"GAMES",
                    current: false,
                    url: "/"
                },
                {
                    text :"COLLECTIBLES",
                    current: false,
                    url: "/"
                },
                {
                    text :"VIDEOS",
                    current: false,
                    url: "/"
                },
                {
                    text :"FANS",
                    current: false,
                    url: "/"
                },
                {
                    text :"NEWS",
                    current: false,
                    url: "/"
                },
                {
                    text :"SHOP",
                    current: false,
                    url: "/"
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
    $colorBlue : #0282F9;
    
    
    nav {
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        #logo {
            height: 100%;
            display: flex;
            align-items: center;


        }

        img {
            height: 80%;
        }
    }
    ul {
        list-style: none;
        display: flex;


        li {
            line-height: 96px;
            margin : 0 10px;
            font-size: 14px;
            cursor: pointer;
            font-weight: 500;
            border-bottom: 4px solid white;


            &:hover {
                border-bottom: 4px solid $colorBlue;
                color: $colorBlue;
            }
        }
    }

    .active {
        color: $colorBlue;
        border-color: $colorBlue;
        font-weight: 500;
    }

</style>