<template>
  <Container name="team">
    <section class="content-section">
      <HashHeader title="TEAM" />
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
          
            name: "Sachin Makwana",
            url: "https://www.linkedin.com/in/sachin-makwana-ab556919",
            pos: "Mentor",
            picture: require("~/assets/Team/menter.jpg"),
            rotation: 75,
          },
          {
          name: "Jay Patel",
            url: "https://in.linkedin.com/in/jay-patel-112569114",
            pos: "Mentor",
            picture: require("~/assets/Team/menter.jpg"),
            rotation: 75,
          },
          
        {
          name: "Het Chauhan",
          url: "https://www.linkedin.com/in/het-chauhan-3ab838233/",
          pos:'Director',
          picture: require("~/assets/Team/het.jpg"),
          rotation: 150,
        },
        {
          name: "Krish Patel",
          url: "https://www.linkedin.com/in/krish-patel-5780bb128/",
          pos:'Director',
          picture: require("~/assets/Team/krish.jpg"),
          rotation: 150,
        },
        {
          name: "Dhrupal Prajapati",
          url: "https://www.linkedin.com/in/dhrupal-prajapati-660396169",
          pos:'Director',
          picture: require("~/assets/Team/dhrupal.jpg"),
          rotation: 150,
        },
        {
        name: "Ashvi Patel",
        url: "https://www.linkedin.com/in/ashvi-patel-170556245",
        pos:'Co-Ordinator',
        picture: require("~/assets/Team/ashvi.jpg"),
        rotation: 75,
      },
      {
        name: "Preet Shah",
        url: "https://www.linkedin.com/in/preet-shah-25b3461b9",
        pos:'Assitant Co-Ordinator',
        picture: require("~/assets/Team/preet.jpg"),
        rotation: 150,
      },
        
// sign off form code hive on 27 feb last committ 

        // {
        //   name: "Hiren Lalani",
        //   url: "https://www.linkedin.com/in/hiren-lalani-8a6ba41b9/",
        //   pos:'Tech Lead',
        //   picture: require("~/assets/Team/hiren.jpg"),
        //   rotation: 75,
        // },
      //   {
      //   name: "Ravi Singh Patel",
      //   url: "https://www.linkedin.com/in/ravi-patel2303/",
      //   pos:'Tech Lead',
      //   picture: require("~/assets/Team/ravi.jpg"),
      //   rotation: 120,
      // },
        {
        name: "Mobin Desai",
        url: "https://www.linkedin.com/in/mobin-desai-4a5b3b22b/",
        pos:'Media Production',
        picture: require("~/assets/Team/mobin.jpg"),
        rotation: 95,
      },
      
      
      {
            name: "Darji Nehaben",
            url: "https://www.linkedin.com/in/neha-darji-590b92202",
            pos:'Documantaion Member',
            picture: require("~/assets/Team/Team2k22/Neha.jpg"),
            rotation: 65,
          },
      
      
        {
          name: "PRINCE PATEL",
          url: "https://www.linkedin.com/in/prince-patel-133452205",
          pos:'Social Media Manager',
          picture: require("~/assets/Team/prince.jpeg"),
          rotation: 65,
        },
        {
        name: "Mihir Prajapati",
        url: "https://www.linkedin.com/in/mihir-prajapati-692142246",
        pos:'Social Media Manager',
        picture: require("~/assets/Team/mhir.jpg"),
        rotation: 120,
      },
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
