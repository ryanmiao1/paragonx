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
          name: 'Kallie Wang',
          title: 'Co-President',
          image: '/images/bio/kallie.png',
          bio: 'Kallie Wang is a senior at the Harker School who is passionate about math and the sciences. She won a USAJMO honorable mention award in 2024 and is a 5x AIME qualifier, 4x Math Prize for Girls qualifier, and USAPhO semifinalist. In her free time, she enjoys dancing and reading.'
        },
        {
          name: 'Harshil Nukala',
          title: 'Co-President',
          image: '/images/bio/harshil.png',
          bio: 'Harshil Nukala is a senior at Dougherty Valley High School. He is really interested in multiple STEM subjects and participated in many competitions from AMC and AIME to F=ma and USACO. Outside of olympiads, he is interested in the field of positive geometry. Harshil has many years of experience in teaching and loves to help the younger generation. In his free time, he likes to go on bike rides, play badminton, and practice carnatic singing.'
        },
        {
          name: 'Cyrus Ghane',
          title: 'Vice President',
          image: '/images/bio/cyrus.jpg',
          bio: 'Cyrus Ghane is a senior at The Harker School. He has earned an honorable mention on the USAPhO and is a 3x AIME qualifier. He is especially interested in the intersection of physics and neuroscience and enjoys playing soccer and the guitar in his free time.'
        }
      ],
      math: [
        {
          name: 'Arjun Joisha',
          title: 'Head of Math',
          image: '/images/bio/arjunj.png',
          bio: 'Arjun Joisha is a senior at the Lynbrook High School. He is a 3 time AIME qualifier, won a bronze medal twice and a silver medal once at the PiMC, and continues to compete in several other regional and college mathematics competitions, including the Stanford Math Tournament and the Berkeley Math Tournament. When not working on math competitions, he also enjoys competitive programming, and has reached USACO Gold. In his free time, you can find him hanging out with his friends, reading interesting math articles, or playing chess or Minecraft.'
        },
        {
          name: 'Hengrui Liang',
          image: '/images/bio/hengrui.png',
          bio: 'Hengrui is a junior at The Harker School. He is a USAMO medalist, USAJMO Winner, and a BMT and SMT Distinguished HM. In his free time, he enjoys playing chess and board games, reading science magazines, and hiking.'
        },
        {
          name: 'Andrew Shi',
          image: '/images/bio/andrewshi.jpg',
          bio: 'Andrew Shi is a sophomore at The Harker School. He is a USACO Platinum contestant and qualified once for the USAJMO, receiving an honorable mention. If he had to choose between math and CS, he would pick math. When not programming with his friends or doing math, you may find him playing tennis.'
        },
        {
          name: 'Benjamin Tang',
          image: '/images/bio/ben.jpg',
          bio: 'Benjamin Tang is a freshman at Del Norte High School in San Diego, California. He is interested in subjects that require critical thinking, like physics, math, coding, and chess, as he is a 3x AIME, USACO Silver qualifier, and chess FIDE Master. In his free time, Benjamin likes to hike and run (despite being very bad), code useless fun coding projects, and play board games.'
        },
        {
          name: 'Vihaan Gupta',
          image: '/images/bio/vihaan.jpeg',
          bio: 'Vihaan Gupta is a sophomore at the Harker School interested in various STEM subjects. He is a 6x AIME Qualifier, USA(J)MO Top Honors, and SMT/BMT Top 10 recipient. In his free time, he enjoys playing all sorts of games with his friends.'
        }
      ],
      cs: [
        {
          name: 'Yash Belani',
          title: 'Head of Computer Science',
          image: '/images/bio/yash.png',
          bio: 'Yash Belani is a junior at the Harker School. He is competing in the USACO Platinum division and attends many coding competitions in the US like BAPC, Proco, mBIT, and M(IT)2. He is also a problem writer for Teamscode, HPI, and Codeforces. In his free time, he enjoys playing many sports like basketball, table tennis, or tennis.'
        },
        {
          name: 'Ellie Zhou',
          title: 'Head of Computer Science',
          image: '/images/bio/ellie.png',
          bio: 'Ellie is a junior at Westmont High School. She is competing in USACO gold, has qualified for AIME several times, won awards at the Synopsys Science Fair for her research, and loves learning about and working on AI & computer vision projects. She also led a team making it to the Wharton Global High School Investment Competition finale. In her free time, she enjoys swimming, dancing, and playing with her dog. She is excited to spread her love of computer science and help students see how powerful and amazing it can be!'
        },
        {
          name: 'Ryan Miao',
          image: '/images/bio/ryan.png',
          bio: 'Ryan is a junior at The Harker School. He is an AIME qualifier, USNCO national qualifier, USACO Gold Division competitor, and has experience in Java and Python. He is also interested in Neuroscience and Artificial Intelligence and enjoys playing tennis and dancing in his free time.'
        },
        {
          name: 'Vaishnav Krishnan',
          image: '/images/bio/vaishnav.png',
          bio: 'Vaishnav is a senior at Obra D. Tompkins High School in Katy, Texas. He represents his school in UIL Computer Science and is currently competing in USACO Gold. He is very passionate about teaching computer science and enjoys learning advanced techniques in computer science such as dynamic programming and segment trees. In his free time, he likes playing music and working out at the gym.'
        },
        {
          name: 'Regina Zhang',
          image: '/images/bio/regina.png',
          bio: 'Regina is a sophomore at The Harker School. She is competing in the USACO Silver division and has coded with C++ and Java. In her free time, she enjoys dancing and spending time with her cats.'
        },
        {
          name: 'Rachel Li',
          image: '/images/bio/rachel.jpg',
          bio: 'Rachel is a sophomore at The Harker School. She is currently a USACO silver competitor and has experience coding in C++, Python, and Java. She has also qualified for AIME and received category awards in both local and state science fairs. In her free time, she builds mini dollhouse kits.'
        },
        {
          name: 'Avi Malhotra',
          image: 'images/bio/avi.jpeg',
          bio: 'Avi Malhotra is a freshman at Fremont High School in California. He is interested in math, computer science, physics, and robotics. He is an AIME qualifier, USACO Silver, BMT DHM, and loves making random machine learning models(especially in the field of medicine). In his free time, he likes to play tennis, basketball, and spend time with friends.'
        }
      ],
      physics: [
        {
          name: 'Shamik Khowala',
          title: 'Head of Physics',
          image: '/images/bio/shamik.png',
          bio: 'Shamik Khowala is a junior at the Harker School. He has qualified for AIME four times as well as participated in several college math competitions, including BMT, HMMT, and SMT. He is also part of Harker’s Science Bowl team. He has earned a bronze medal in USAPhO and a bronze in National Astronomy Competition (NAC). At school, he is an active member of the math, physical sciences, and astronomy clubs. In his free time, he loves to explore advanced math and physics topics and solve interesting problems.'
        },
        {
          name: 'Pascal Qin',
          image: '/images/bio/pascal.png',
          bio: 'Pascal Qin is a junior at The Harker School. He has qualified for AIME and USACO Silver, earned silver at USAPhO, and earned bronze at the National Astronomy Competition. Pascal has studied physics for two years now and has participated in several physics contests, such as USAYPT and Physics Brawl. In his free time, he enjoys playing basketball and listening to music.'
        },
        {
          name: 'Karthik Veeramallu',
          image: '/images/bio/karthik.png',
          bio: 'Karthik Veeramallu is a senior at Obra D. Tompkins High School in Katy, Texas, who is an AIME qualifier, USAPhO qualifier, the president of his school physics club, and an officer of his school math club. Fluent in Java, he is interested in building projects and modeling real world scenarios. In his free time, he enjoys working his job, volunteering, and teaching independently.'
        },
        {
          name: 'Lucas Wu',
          image: '/images/bio/lucas.png',
          bio: 'Lucas Wu is a sophomore at The Harker School. He won First Award at the Synopsys Science and Engineering Fair, qualified for CSEF, and earned an honorable mention at USAPhO. He has also qualified for AIME. Lucas is deeply passionate about physics, especially Electromagnetism, and can often be found doing interesting physics problems. Outside of math and science, he plays basketball, piano, and runs outside.'
        },
        {
          name: 'Andy Long',
          image: '/images/bio/andy.webp',
          bio: 'Andy is a senior at Seven Lakes High School in Katy, Texas. He is really passionate about physics and is a 2x USAAAO semifinalist, TXSEF finalist, president of his school’s Physics Club, an officer for his school’s astronomy club, and a bronze medalist at the National Astronomy Competition. This summer he will be participating in the Astrophysics program at SSP and in his free time he really enjoys playing pickleball and going out with friends.'
        },
        {
          name: 'Eric Dong',
          image: '/images/bio/eric.jpg',
          bio: 'Eric Dong is a senior at The Harker School. He is active in STEM competitions, having competed in, earned awards in, and prepared for the AMC, AIME, BMT, SMT, F=ma, and USAAAO. He is also a president of his school’s astronomy club and an active member of the science bowl team. He also enjoys engaging in research, having interned at UC Davis and having worked on a project about neutron star habitability. Outside of STEM, he is an avid clarinetist and competitive swimmer.'
        },
        {
          name: 'Alex Jin',
          image: '/images/bio/alexj.jpg',
          bio: 'Alex Jin is a rising senior from Southridge School in Vancouver, Canada. Having qualified for the Canadian National IOAA Training Camp and the Canadian Junior Physics Olympiad (where he won second place), he hopes to make others love physics as much as he does. He is currently doing theoretical cosmology research and likes to play chess and soccer in his spare time.'
        }
      ],
      chem: [
        {
          name: 'Leo Zhang',
          title: 'Head of Chemistry',
          image: '/images/bio/leo.png',
          bio: 'Leo Zhang is a junior at The Harker School. He has qualified for AIME two times and made it to the national level of USNCO. In his free time, he enjoys playing chess, Brawl Stars, card games, and solving difficult logic puzzles.'
        },
        {
          name: 'Kevin He',
          image: '/images/bio/kevinhe.png',
          bio: 'Kevin is a junior at The Harker School. He has qualified for the AIME, earned an honorable mention at USAPhO, and also takes part in other STEM related activities such as USAYPT, USNCO, and robotics where he is a design lead on the school team. In his free time, he loves to play golf, saxophone, and chess.'
        },
        {
          name: 'William Jiang',
          image: '/images/bio/william.png',
          bio: 'William is a junior at The Harker School. He is very passionate about physics and chemistry, participating in competitions like USAYPT, Physics Brawl, and USNCO, as well as working on research projects related to the intersection of physics, chemistry, and machine learning. In his free time, he enjoys playing chess and solving interesting physics problems.'
        },
        {
          name: 'Richard Peng',
          image: '/images/bio/richard.png',
          bio: 'Richard Peng is a junior at Archbishop Mitty High School. He has earned honors in USNCO Nationals and does science bowl as well. He enjoys the intuitive nature of chemistry and how it can explain the world. Richard also enjoys biology, economics, and badminton.'
        }
      ],
      bio: [
        {
          name: 'Terry Xie',
          image: '/images/bio/terry.png',
          title: 'Head of Biology',
          bio: 'Terry is a senior at The Harker School who is passionate about biology and math. He is a USABO Semifinalist, and has qualified for AIME twice. He has also worked on an independent bioinformatics research project which he presented at the ICMI, and placed 8th at regional JSHS with. Terry has some wet lab experience as well through an internship at the Serrano lab through the BU RISE program. In his free time, Terry enjoys reading and playing water polo.'
        },
        {
          name: 'Shreyas Kini',
          image: '/images/bio/shreyas.jpg',
          bio: 'Shreyas Kini is a senior at Obra D. Tompkins High School in Katy, Texas. He is a two time USABO Semifinalist, the president of his science olympiad and biology clubs, and has placed as a runner up in the Brain Bee Texas division. Shreyas is excited to spread a passion for biology in others, as seen in his past experience as a director of the American Regional Biology Competition nonprofit. Outside of biology, Shreyas loves to play basketball, go on long runs, work out at the gym, and play the cello.'
        },
        {
          name: 'Annie Yu',
          image: '/images/bio/annie.png',
          bio: 'Annie Yu is a sophomore at The Harker School. She is a biology coach for Harker’s Middle School Science Bowl team and has taught at various other organizations. In her free time, she enjoys reading and writing literature, volunteering, and reading Campbell Biology.'
        },
        {
          name: 'Melody Wang',
          image: '/images/bio/melody.png',
          bio: 'Melody Wang is a high school junior at Basis Independent Fremont. She is a USABO semifinalist and a BBO gold medalist. She leads the Neuroscience Club at her school and also teaches dance at different community organizations. She is also passionate about research, competing in the  California Science and Engineering Fair and also getting into Broadcom Masters Top 300. In her spare time she enjoys nature walks and baking.'
        }
      ],
      outreach: [
        {
          name: 'Teresa Song',
          title: 'Head of Outreach',
          bio: 'Teresa Song is a sophomore at the Harker School and a two-time Scholastic Arts national gold medalist. In her free time, she can be found sneaking into the pantry for snacks, reading, or running.',
          image: '/images/bio/teresa.jpg'
        },
        {
          name: 'Akshitaa Arun',
          bio: 'Akshitaa Arun (Akshu/Ash) is a senior in Tamil Nadu, India. She has attended various math camps in India such as PROMYS INDIA 2024, RAMTP 2023, AGMNC 2022 & 2023. She is a teaching assistant Athemath, a part of the international outreach team of URBAN HARMONY PROJECT and runs NC^2! She enjoys tutoring outside school, and showing people that math can be fun! She loves puzzles (especially sudoku) and singing!',
          image: '/images/bio/akshitaa.png'
        },
        {
          name: 'Mason Chang',
          image: '/images/bio/mason.png',
          bio: 'Mason Chang is a freshman at the Harker School. He has received an honorable Mention in the USMDO, and serves as the officer of outreach at the Harker Data Science Club. Last summer, he worked on an independent research project, collecting data worldwide and coming to conclusions on how much impact certain lifestyle habits have on mental health and daily stress levels, submitting his findings to a panel of college professors and industry professionals. He also conducts wet-lab experiments at home, running gel electrophoresis and isolating DNA from a pineapple using household materials. In his free time outside of biology, he enjoys piano and basketball.'
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
