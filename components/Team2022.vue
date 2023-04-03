<template>
    <Container name="team">
      <section class="content-section">
        <HashHeader title="MEMBER" />
        <div class="contents">
          <div class="team-grid">
            <div v-for="(teamMember, index) in team" :key="index"
              :class="['team-card', `rot-${Math.floor(Math.random() * 24) * 15}`]">
              <a :href="teamMember.url" target="_blank" rel="noopener noreferrer">
                <div class="picture-wrapper smooth-transition">
                  <img :src="teamMember.picture" alt="profile picture" class="profile-pic" />
                </div>
              </a>
              <h4 class="title">{{ teamMember.name }}</h4>
              <h6 class="title">{{teamMember.pos}}</h6>
            </div>
          </div>
        </div>
      </section>
    </Container>
  </template>
  
  <script>
  import Container from "~/components/Container";
  import HashHeader from "~/components/HashHeader";
  
  export default {
    components: {
      Container,
      HashHeader,
    },
    data() {
      return {
        team: [
          {
            // Event 
            // tech 
            // media 
            // dec  
            // social 

            // Event 

              name: "Garima Raj",
              url: "https://www.linkedin.com/in/garima-raj-b78292253",
              pos: "Assistant Co-ordinator",
              picture: require("~/assets/Team/Team2k22/Garima.jpg"),
              rotation: 75,
            },
            {
            name: "Nishtha Dave",
              url: "https://www.linkedin.com/in/nistha-dave-68330b240",
              pos: "Event Management Representative",
              picture: require("~/assets/Team/Team2k22/Nistha.jpg"),
              rotation: 75,
            },
            {
            name: "Krisha Panchal",
            url: "https://www.linkedin.com/in/krisha-panchal-b5b292253",
            pos:'Event Management Member',
            picture: require("~/assets/Team/Team2k22/Krisha.jpg"),
            rotation: 205,
          },
          {
            name: "Anju Rajput",
            url: "https://www.linkedin.com/in/anju-rajput-9062bb253/",
            pos:'Event Management Member',
            picture: require("~/assets/Team/Team2k22/Anju.jpg"),
            rotation: 150,
          },
          {
            name: "Nishtha Patel",
            url: "https://www.linkedin.com/in/nishtha-patel-b255a725b", 
            pos:'Event Management Member',
            picture: require("~/assets/Team/Team2k22/P_Nishtha.jpg"),
            rotation: 150,
          },
          {
            name: "Dwivedi Shrushti",
            url: "https://www.linkedin.com/in/sristy-dwivedi-b6634625b", 
            pos:'Event Management Member',
            picture: require("~/assets/Team/Team2k22/Sristy.jpg"),
            rotation: 150,
          },
          {
            name: "Pari Patel",
            url: "https://www.linkedin.com/in/pari-patel-b77223259/",
            pos:'Event Management Member',
            picture: require("~/assets/Team/Team2k22/Pari.jpg"),
            rotation: 150,
          },
          {  // add 23/03/23
          name: "Pathan Tabassum",
          url: "https://www.linkedin.com/in/tabassum-pathan-17b82726b",
          pos:'Event Management Member',
          picture: require("~/assets/Team/Team2k22/Tabassum.jpg"),
          rotation: 120,
          },

          // tech 
          {
            name: "Gorani Ravi",
            url: "https://www.linkedin.com/in/ravi-gorani",
            pos:'Tech Member',
            picture: require("~/assets/Team/Team2k22/Ravi.jpg"),
            rotation: 75,
          },
          {
          name: "Jaimin Parmar",
          url: "https://www.linkedin.com/in/jaimin0410",
          pos:'Tech Member',
          picture: require("~/assets/Team/Team2k22/Jaimin.jpg"),
          rotation: 95,
          },
          {
          name: "PRAJAPATI YASH",
          url: "https://www.linkedin.com/in/yash-prajapati-998043237",
          pos:'Tech Member',
          picture: require("~/assets/Team/Team2k22/Yash.jpg"),
          rotation: 120,
          },
          {
          name: "KUBER JAYDEEP",
          url: "https://www.linkedin.com/in/jay-kuber-7291a7252",
          pos:'Tech Member',
          picture: require("~/assets/Team/Team2k22/Jaydeep.jpg"),
          rotation: 120,
          },
          {
          name: "Dev Golwala",
          url: "https://www.linkedin.com/in/dev-golwala-bab4ab243",
          pos:'Tech Member',
          picture: require("~/assets/Team/Team2k22/Dev.jpg"),
          rotation: 120,
          },
          {
          name: "Yashvi Viradiya",
          url: "https://www.linkedin.com/in/yashvi-viradiya-53bb29254",
          pos:'Tech Member',
          picture: require("~/assets/Team/Team2k22/Yashvi.jpg"),
          rotation: 120,
          },
                               // add 23/03/23
          {
          name: "Dhruvi Vadhaiya ",
          url: "https://www.linkedin.com/in/dhruvi-vadhaiya-5164961a4",
          pos:'Tech Member',
          picture: require("~/assets/Team/Team2k22/dhruvi.jpg"),
          rotation: 120,
          },
        
          // media 
          {
          name: "Jansari Srushti",
          url: "https://www.linkedin.com/in/srushti-jansari-79019b256/",
          pos:'Media Production Representative',
          picture: require("~/assets/Team/Team2k22/srushti.jpg"),
          rotation: 75,
          },
          {
          name: "Niki Vaghela",
          //   url: "https://www.linkedin.com/in/preet-shah-25b3461b9",  
          pos:'Media Production Member',
          picture: require("~/assets/Team/Team2k22/Niki.jpg"),
          rotation: 150,
          },
        
          {
            name: "Patel Disha",
            url: "https://www.linkedin.com/in/disha-patel-7b3343253",
            pos:'Media Production Member',
            picture: require("~/assets/Team/Team2k22/Disha.jpg"),
            rotation: 65,
          },
          {
            name: "Tandel Priyanshu",
            url: "https://www.linkedin.com/in/priyanshu-tandel-56a707250",
            pos:'Media Production Member',
            picture: require("~/assets/Team/Team2k22/Priyanshu.jpg"),
            rotation: 65,
          },

          {
            name: "Darji mallika",
            url: "https://www.linkedin.com/in/nistha-dave-68330b240",
            pos:'Media Production Member',
            picture: require("~/assets/Team/Team2k22/Mallika.jpg"),
            rotation: 65,
          },
          // Docu 
         
        ],
      };
    },
  };
  </script>
  
  <style lang="scss" scoped>
  .content-section {
    display: flex;
    flex-direction: column;
    padding: 20px 0;
    font-family: "Segoe UI";
  
    .contents {
      padding: 1rem 4rem;
      text-align: center;
  
      @include respond-below(sm) {
        padding: 1rem 0rem;
      }
  
      .team-grid {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        column-gap: 20px;
        row-gap: 30px;
  
        @include respond-below(md) {
          grid-template-columns: repeat(3, 1fr);
        }
  
        @include respond-below(sm) {
          grid-template-columns: repeat(2, 1fr);
        }
  
        @include respond-below(xs) {
          grid-template-columns: repeat(1, 1fr);
        }
  
        .team-card {
          padding-bottom: 1rem;
          display: flex;
          flex-direction: column;
          box-shadow: rgba(255, 107, 0, 0.07) 0px 0px 10px 2px;
          border-radius: 1rem;
          // justify-content: center;
          align-items: center;
  
          .picture-wrapper {
            border-style: solid;
            border-width: 3px;
            border-color: red red white red;
            width: 210px;
            height: 210px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            margin-top: 1rem;
  
            .profile-pic {
              width: 200px;
              height: 200px;
              border-radius: 50%;
              // background: var(red);
            }
  
            @include respond-below(md) {
              width: 170px;
              height: 170px;
  
              .profile-pic {
                width: 160px;
                height: 160px;
              }
            }
  
            @include respond-below(sm) {
              width: 140px;
              height: 140px;
  
              .profile-pic {
                width: 130px;
                height: 130px;
              }
            }
          }
  
          .title {
            font-size: 1.2rem;
            text-align: center;
            margin: 1rem 0rem;
            color: rgba(233, 83, 34, 1);
  
            @include respond-below(sm) {
              font-size: 1rem;
              margin-top: 10px;
            }
          }
        }
      }
    }
  }
  </style>
  