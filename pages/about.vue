<template>
  <div>
    <v-container>
      <h2 class="text-md-h2 text-h3 text-center">
        People behind ParagonX Academy
      </h2>
    </v-container>
    <officer-list :people="executive" title="Executive Team" />
    <officer-list :people="math" title="Mathematics Officers" />
    <officer-list :people="cs" title="Computer Science Officers" />
    <officer-list :people="physics" title="Physics Officers" />
    <officer-list :people="chem" title="Chemistry Officers" />
    <officer-list :people="bio" title="Biology Officers" />
    <officer-list :people="outreach" title="Outreach Team" />
  </div>
</template>

<script>
export default {
  name: 'AboutPage',
  data () {
    return {
      executive: [
        {
          name: 'Ellie Zhou',
          title: 'Co-President',
          image: '/images/bio/ellie.png',
          bio: 'Ellie is a senior at Westmont High School. She is competing in USACO gold, has qualified for AIME several times, won awards at the Synopsys Science Fair for her research, and loves learning about and working on AI & computer vision projects. She also led a team making it to the Wharton Global High School Investment Competition finale. In her free time, she enjoys swimming, dancing, and playing with her dog. She is excited to spread her love of computer science and help students see how powerful and amazing it can be!'
        },
        {
          name: 'Shamik Khowala',
          title: 'Co-President',
          image: '/images/bio/shamik.png',
          bio: 'Shamik Khowala is a senior at the Harker School. He has qualified for AIME several times as well as achieved individual ranks and honors in several college math competitions like BMT, HMMT, SMT & PUMaC. He has captained Harker’s Science Bowl A team. He has earned a gold medal in USAMTS, bronze in USAPhO and a bronze in National Astronomy Competition (NAC). At school, he is an active member of the math, physical sciences, and astronomy clubs. In his free time, Shamik enjoys reading speculative fiction and WWII novels.'
        },
        {
          name: 'Yash Belani',
          title: 'Co-Vice President',
          image: '/images/bio/yash.png',
          bio: 'Yash Belani is a senior at the Harker School. He competes in the USACO Platinum division and was a USACO Finalist in 2026. He attends many coding competitions in the US like BAPC, Proco, mBIT, and M(IT)2. He is also a problem writer for Teamscode, HPI, Codeforces, and USACO. In his free time, he enjoys playing many sports like basketball, table tennis, or tennis.'
        },
        {
          name: 'Leo Zhang',
          title: 'Co-Vice President',
          image: '/images/bio/leo.png',
          bio: 'Leo Zhang is a senior at The Harker School. He has qualified for AIME two times and made it to the national level of USNCO. In his free time, he enjoys playing chess, Brawl Stars, card games, and solving difficult logic puzzles.'
        }
      ],
      math: [
        {
          name: 'Andrew Shi',
          image: '/images/bio/andrewshi.jpg',
          bio: 'Andrew Shi is a junior at The Harker School. He is a USACO Platinum contestant and qualified once for the USAJMO, receiving an honorable mention. If he had to choose between math and CS, he would pick math. When not programming with his friends or doing math, you may find him playing tennis.'
        },
        {
          name: 'Benjamin Tang',
          image: '/images/bio/ben.jpg',
          bio: 'Benjamin Tang is a sophomore at Del Norte High School in San Diego, Calfornia. He enjoys physics, math, coding, and chess. He is a 4x AIME + USAJMO qualifier, USACO Silver qualifier, and chess FIDE Master. In his free time, Benjamin likes to hike and run, code fun projects, and play board games.'
        },
        {
          name: 'Hengrui Liang',
          image: '/images/bio/hengrui.png',
          bio: 'Hengrui is a senior at The Harker School. He is a USAMO medalist, USAJMO Winner, and a BMT and SMT Distinguished HM. In his free time, he enjoys playing chess and board games, reading science magazines, and hiking.'
        },
        {
          name: 'Vihaan Gupta',
          image: '/images/bio/vihaan.jpeg',
          bio: 'Vihaan Gupta is a junior at the Harker School interested in various STEM subjects. He is a 6x AIME Qualifier, USA(J)MO Top Honors, and SMT/BMT Top 10 recipient. In his free time, he enjoys playing all sorts of games with his friends.'
        },
        {
          name: 'Philip Dong',
          image: '/images/bio/philip.jpeg',
          bio: 'Philip Dong is a sophomore at Cupertino High School, and is very interested in math, coding, and science. He got AMC 10 DHM, is an AIME qualifier, USA(J)MO qualifier, and achieved USNCO honors. He is really passionate about computational biology, and in his free time, he likes to play tennis, play the piano, play games, and eat.'
        },
        {
          name: 'Akshitaa Arun',
          bio: 'Akshitaa Arun (Akshu/Ash) graduated high school in 2026 in Tamil Nadu, India. She has attended various math camps in India such as PROMYS INDIA 2024, RAMTP 2023, AGMNC 2022 & 2023. She is a teaching assistant Athemath, a part of the international outreach team of URBAN HARMONY PROJECT and runs NC^2! She enjoys tutoring outside school, and showing people that math can be fun! She loves puzzles (especially sudoku) and singing!',
          image: '/images/bio/akshitaa.png'
        }
      ],
      cs: [
        {
          name: 'Regina Zhang',
          image: '/images/bio/regina.png',
          title: 'Head of Computer Science',
          bio: 'Regina is a junior at The Harker School. She is competing in the USACO Gold division using C++ and is an AIME qualifier. In her free time, she enjoys dancing and spending time with her cats.'
        },
        {
          name: 'Rachel Li',
          image: '/images/bio/rachel.jpg',
          bio: 'Rachel is a junior at The Harker School. She is currently a USACO silver competitor and has experience coding in C++, Python, and Java. She has also qualified for AIME and received category awards in both local and state science fairs. In her free time, she builds mini dollhouse kits.'
        },
        {
          name: 'Avi Malhotra',
          image: 'images/bio/avi.jpeg',
          bio: 'Avi Malhotra is a sophomore at Fremont High School in California. He is interested in math, computer science, physics, and robotics. He is an AIME qualifier, USACO Silver, BMT DHM, and loves making random machine learning models (especially in the field of medicine). In his free time, he likes to play tennis, basketball, and spend time with friends.'
        },
        {
          name: 'Dennis Yang',
          image: 'images/bio/dennis.png',
          bio: 'Dennis is a rising junior at Carlmont High School. He is a competitor in USACO and was a finalist during the \'25 and \'26 seasons. He also does USAAIO in which he qualified for camp in the \'26 season. Outside of programming and AI, he also does some research and math. In his free time, he likes finding good eats and sleeping.'
        },
        {
          name: 'Aiden Lei',
          image: 'images/bio/aiden.png',
          bio: 'Aiden is a junior at the Harker School. He is interested in computer science, physics, and finance. He competes in USACO gold and published 2 AI papers accepted at ICML and NAACL worshops. In his free time, he likes to talk with friends'
        },
        {
          name: 'Sarah Zhang',
          image: 'images/bio/sarah.png',
          bio: 'Sarah Zhang is a sophomore at Dublin Jerome High School in Dublin, Ohio. She loves anything STEM, especially math and computer science. She codes in Java and is a USACO Silver competitor. In her free time, she loves reading books, playing volleyball, and playing viola.'
        }
      ],
      physics: [
        {
          name: 'Lucas Wu',
          image: '/images/bio/lucas.png',
          title: 'Head of Physics',
          bio: 'Lucas Wu is a junior at The Harker School. He won the Gold Award at the Berkeley Physics Tournament, earned two honorable mentions at the USAPhO, and received Distinguished Honorable Mention at the Berkeley Math Tournament. He leads photonics research at UC Berkeley and has twice won First Award at the Synopsys Science and Engineering Fair, qualifying for CSEF both times. Lucas enjoys physics and can often be found solving interesting problems. In his free time, he plays piano, watches Formula 1, and runs.'
        },
        {
          name: 'Pascal Qin',
          image: '/images/bio/pascal.png',
          bio: 'Pascal Qin is a senior at The Harker School. He has qualified for AIME and USACO Silver, earned silver at USAPhO, and earned bronze at the National Astronomy Competition. Pascal has studied physics for two years now and has participated in several physics contests, such as USAYPT and Physics Brawl. In his free time, he enjoys playing basketball and listening to music.'
        },
        {
          name: 'Kevin He',
          image: '/images/bio/kevinhe.png',
          bio: 'Kevin is a senior at The Harker School. He has qualified for the AIME, earned an honorable mention at USAPhO, and also takes part in other STEM related activities such as USAYPT, USNCO, and robotics where he is a design lead on the school team. In his free time, he loves to play golf, saxophone, and chess.'
        }
      ],
      chem: [
        {
          name: 'Ryan Miao',
          image: '/images/bio/ryan.png',
          title: 'Head of Chemistry',
          bio: 'Ryan is a senior at The Harker School. He is a USNCO camper, 2x AIME, and is currently in USACO Gold. He enjoys playing tennis, dancing, and hanging out with his cats in his free time.'
        },
        {
          name: 'Jeffrey Yang',
          image: '/images/bio/jeffrey.png',
          bio: 'Jeffrey is a senior at the Princeton International School of Math and Science. He is a USNCO high honors. He enjoys playing valorant, roblox and tennis.'
        },
        {
          name: 'Richard Peng',
          image: '/images/bio/richard.png',
          bio: 'Richard Peng is a senior at Archbishop Mitty High School. He has earned honors in USNCO Nationals and does science bowl as well. He enjoys the intuitive nature of chemistry and how it can explain the world. Richard also enjoys biology, economics, and badminton.'
        },
        {
          name: 'Shivan Shrinivas',
          image: '/images/bio/shivan.png',
          bio: 'Shivan Shrinivas is a senior at Montgomery High School. He is a USNCO High Honors Medalist as well as a NJ Governor\'s School in the Sciences attendee. In his free time, he enjoys theater, piano, and writing physics simulations. He is looking forward to sharing his love of physics and chemistry with students!'
        }
      ],
      bio: [
        {
          name: 'Sanjith Senthil',
          image: '/images/bio/sanjith.png',
          bio: 'Sanjith Senthil is a senior at the Harker school. He is interested in computational biology and is a USABO semifinalist. Outside of STEM, he competes in debate tournaments and plays racing games.'
        }
      ],
      outreach: [
        {
          name: 'Mason Chang',
          title: 'Head of Outreach',
          image: '/images/bio/mason.png',
          bio: 'Mason Chang is a sophomore at the Harker School. He loves biology and enjoys running his own bioengineering experiments at home. He also does independent research projects. In his free time, he enjoys piano and basketball.'
        },
        {
          name: 'Selena Ghane',
          image: '/images/bio/selena.png',
          bio: 'Selena Ghane is a sophomore at The Harker School who is broadly interested in the diverse applications of computational physics modeling across domains. She is passionate about research and has qualified for the California Science and Engineering Fair. In her free time, she enjoys playing volleyball and reading academic blogs.'
        },
        {
          ame: 'Joyce Yan',
          image: '/images/bio/joyce.jpeg',
          bio: 'Joyce Yan is a sophomore at the Harker School and a two-time Scholastic Arts national gold medalist. She enjoys coding, eating pastries, and crocheting.'
        }
      ]
    }
  },
  head () {
    return {
      title: 'About',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'ParagonX Academy is a 501(c)(3) student-led non-profit organization that strives to provide high-quality, readily available STEM education to everyone in need through free curricula.'
        }
      ]
    }
  }
}
</script>
