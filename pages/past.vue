<template>
  <div>
    <v-container>
      <h2 class="text-md-h2 text-h3 text-center">
        People behind ParagonX Academy
      </h2>
      <div style="width: 80px; height: 4px" class="my-4 secondary mx-auto" />
    </v-container>
    <officer-list :people="people" title="Past Officers" />
  </div>
</template>

<script>
export default {
  name: 'PastPage',
  data () {
    return {
      people: [
        {
          name: 'Joe Li',
          title: 'Founder, Stanford \'28',
          image: '/images/bio/joe.png',
          bio: 'Joe graduated from the Harker School in 2024. He is a USACO Finalist, USAPhO Gold Medalist, and 4x AIME qualifier. His CS journey began in the fall of 2017, when he first started learning C++ with X-Camp. In his free time, he plays violin and does karate.'
        },
        {
          name: 'Austin Geng',
          title: 'MIT \'28',
          image: '/images/bio/austin.jpg',
          bio: 'Austin Geng graduated from the Benjamin Franklin High School in 2024. He is an International Olympiad in Informatics Gold Medalist and Math Olympiad Program invitee and has narrowly missed a perfect AMC10. In both math and competitive programming, he especially enjoys ad hoc problems. In his free time, he likes to code (unrelatedly in JavaScript) and play video games.'
        },
        {
          name: 'Aniketh Tummala',
          title: 'UC Berkeley \'28',
          image: '/images/bio/aniketh.jpg',
          bio: 'Aniketh graduated from The Harker School in 2024. As well as being a USAPhO Silver medalist and top 50th in the nation in the Physics Bowl, he is a USACO Platinum contestant and 4 times AIME qualifier. In his free time, he enjoys taking his two dogs for walks around his neighborhood and playing the piano.'
        },
        {
          name: 'Harry Chen',
          title: 'CalTech \'28',
          image: '/images/bio/harry.jpg',
          bio: 'Harry graduated from Northwood High School in Irvine in 2024. He competed in USACO Platinum and has experience in full-stack web development. Harry also was involved with NLP research. In his free time Harry likes to play tennis.'
        },
        {
          name: 'Thomas Liu',
          title: 'MIT \'28',
          image: '/images/bio/thomas.jpg',
          bio: 'Thomas graduated from The Harker School in 2024. Fluent in C++, he enjoys competitive programming and is a USACO Finalist. In his spare time he enjoys playing video games and solving coding problems. He also dabbles in web development and AI.'
        },
        {
          name: 'Gautam Bhooma',
          title: 'UC Berkeley \'28',
          image: '/images/bio/gautam.jpg',
          bio: 'Gautam graduated from the Harker School in 2024. He is a National Top 300 Broadcom MASTERS Semifinalist after winning the Grand Prize of the Synopsys Championship in 2020. As the captain of the Harker Science Bowl team, he led his team to advance to the 2020 Science Bowl National Championships.'
        },
        {
          name: 'Arjun Gurjar',
          title: 'UC Berkeley \'28',
          image: '/images/bio/arjung.jpg',
          bio: 'Arjun Gurjar graduated from The Harker School in 2024. In addition to being a nationalist in the North South Science Bee, he is passionate about biology and has many years of experience in teaching students as well as conducting wet lab research. Apart from studying for USABO, Arjun likes editing videos, going on walks, and listening to music.'
        },
        {
          name: 'Kevin Zhang',
          title: 'UIUC \'28',
          image: '/images/bio/kevin.png',
          bio: 'Kevin graduated from The Harker School in 2024. Besides studying computer science and physical sciences, he is also interested in arts and design with experience in digital mediums such as Photoshop and Canva. He was also a graphic designer for the Harker Programming Club and produced media for his school’s journalism program too. In his free time, he enjoys photo and video editing, as well as playing and watching basketball.'
        },
        {
          name: 'Dustin Miao',
          title: 'CMU \'28',
          image: '/images/bio/dustin.jpg',
          bio: 'Dustin graduated from the Harker School in 2024. He is in USACO\'s platinum division and a master on Codeforces, and is also interested in web development and artificial intelligence. In his spare time, he enjoys playing cello.'
        },
        {
          name: 'Arnav Swaroop',
          title: 'UC Berkeley \'28',
          image: '/images/bio/arnav.png',
          bio: 'Arnav Swaroop graduated from The Harker School in 2024. He enjoys Physics, Earth+Space Science, and biology. He is a USESO finalist, a USABO semifinalist, and has other STEM accolades in the above fields. He won the Regional Science Bowl in 2020, and was part of Harker\'s High School Science Bowl A Team and a senior Middle School Science Bowl coach. When not studying science, he works on his diverse array of research projects ranging from astrophysics to biochemistry.'
        },
        {
          name: 'Henry Yao',
          title: 'Johns Hopkins \'28',
          image: '/images/bio/henry.png',
          bio: 'Henry graduated from Lynbrook High School in 2024. He is passionate about STEM overall, and has won USAJMO HM and AMC10 DHR three times, and came close to USAPHO along with 5\'s in most AP Physics content. He is also passionate about STEM research and has taught and TA\'d classes at Alphastar and other summer camps. When he isn\'t grinding school, Henry enjoys biking, eating food, and listening to music.'
        },
        {
          name: 'Andrew Xie',
          title: 'MIT \'29',
          image: '/images/bio/andrewxie.jpg',
          bio: 'Andrew (Weian) Xie is a senior at The Hotchkiss School in Connecticut. An avid fan of math contests, he has qualified for the AIME 4 times, USAJMO 2 times, where he earned Top Winner and attended MOP in 2023. He is very passionate about promoting mathematical interest in younger kids, especially in under-represented communities, having co-founded a middle school math competition sponsored by his school, as well as AoPS and AwesomeMath. Outside of math, he enjoys playing the piano, reading poetry, cross country practice, and listening to R&B.'
        },
        {
          name: 'Andrew Liang',
          title: 'Stanford \'29',
          image: '/images/bio/andrew.png',
          bio: 'Andrew Liang graduated from The Harker School in 2025. He is a USACO Gold contestant and International Science and Engineering Fair (ISEF) Finalist. He enjoys teaching other students and helping them discover their own passions. In his spare time, he likes to play chess and listen to classical music.'
        },
        {
          name: 'Alex Huang',
          title: 'Oxford \'30',
          image: '/images/bio/alex.jpg',
          bio: 'Alex Huang graduated from The Harker School in 2025 and is a 2021 MathCounts National Round qualifier, four-time AIME qualifier, participant in The Ross Mathematics Program 2023 and 2024, and PRIMES-USA 2024 researcher. Fluent in C++, Java, and Python, he enjoys applying scientific machine learning to elucidate biophysical processes. To disseminate his knowledge to aspiring students, he has led volunteer teaching initiatives and has won the President\'s Volunteer Service Gold Award three times. In his free time, he enjoys playing bridge and engaging friends in thought-provoking conversations.'
        },
        {
          name: 'Juliana Li',
          image: '/images/bio/juliana.png',
          title: 'Harvard \'29',
          bio: 'Juliana Li graduated from The Harker School in 2025. She is a 4x AIME qualifier, was invited to MathCounts Nationals, is competing in USACO Gold, and won 1st place in biology research at both the local & state science fair. In her free time, she enjoys web/app development, volunteering, and dancing.'
        },
        {
          name: 'Jacqueline Huang',
          image: '/images/bio/jacqueline.png',
          title: 'Stanford \'29',
          bio: 'Jacqueline Huang graduated from The Harker School in 2025. She is a USAPhO medalist, 4x AIME qualifier, and has several years of experience in teaching math and science. She enjoys hiking and reading in her free time.'
        },
        {
          name: 'Aarush Vailaya',
          image: '/images/bio/aarush.jpg',
          title: 'MIT \'29',
          bio: 'Aarush Vailaya graduated from The Harker School in 2025. He is a 5 time qualifier of AIME, USAMO gold medalist, won 1st place in both the Synopsys Physical Sciences & Engineering as well as the Bay Area Math Olympiad, a USAMTS gold medalist, and competed in many math events, including the Stanford Math Tournament, AMC 10, and AIME. He also participated in the HCSSiM and SUMaC summer programs, and does math research through PRIMES-USA. While not doing math, he enjoys working on random coding projects, grinding Wynncraft, and playing piano.'
        },
        {
          name: 'Neil Krishnan',
          image: '/images/bio/neil.jpg',
          title: 'MIT \'29',
          bio: 'Neil Krishnan graduated from The Harker School in 2025. In addition to getting 1st award in Synopsys Physical Sciences & Engineering and qualifying for CSEF and Broadcom Masters, he has done a lot of math as a five-time AIME qualifier, USAMO silver medalist, USAMTS gold winner (near perfect score), and recipient of multiple distinguished honorable mentions in BMT. He has also participated in in math summer programs, namely Hampshire College Summer Studies in Mathematics and USA-Canada MathCamp. Neil also likes doing mathematical research on friends-and-stranger graphs and graph connectivity. In his free time, he enjoys playing piano and doing NYT mini crosswords (and the regular if he feels smart that day).'
        },
        {
          name: 'Sophia Liu',
          image: '/images/bio/sophia.png',
          title: 'Stanford \'29',
          bio: 'Sophia Liu graduated from The Harker School in 2025. A lover of graphic design and fine arts, she manages outreach/media for a few organizations, serves as an art editor for The Expressionist, and is a Scholastic Arts national gold and silver medalist. Aside from art, she researches childhood cognitive development and neuroscience.'
        },
        {
          name: 'James Lin',
          image: '/images/bio/james.png',
          title: 'UT Austin \'30',
          bio: 'James Lin graduated from The Harker School in 2026. He was a USACO platinum contestant, three-time AIME qualifier, and USAJMO qualifier. He has also competed in many math and computer science competitions, such as SMT, Teamscode, and LIT. In his free time, he reads and listens to music.'
        },
        {
          name: 'Samuel Tong',
          image: '/images/bio/samuel.png',
          title: 'Cornell \'30',
          bio: 'Samuel graduated from The Harker School in 2026. He competed in the USACO Gold division, and he uses his expertise in computer science on bioinformatics and drug reaction models. Samuel is a retired fencer, and he loves watching dramas and walking his dog.'
        },
        {
          name: 'Kallie Wang',
          title: 'Harvard \'30',
          image: '/images/bio/kallie.png',
          bio: 'Kallie Wang graduated from The Harker School in 2026 and is passionate about math and the sciences. She won a USAJMO honorable mention award in 2024 and is a 5x AIME qualifier, 4x Math Prize for Girls qualifier, and USAPhO semifinalist. In her free time, she enjoys dancing and reading.'
        },
        {
          name: 'Harshil Nukala',
          title: 'UC Berkeley \'30',
          image: '/images/bio/harshil.png',
          bio: 'Harshil Nukala graduated from Dougherty Valley High School in 2026. He is really interested in multiple STEM subjects and participated in many competitions from AMC and AIME to F=ma and USACO. Outside of olympiads, he is interested in the field of positive geometry. Harshil has many years of experience in teaching and loves to help the younger generation. In his free time, he likes to go on bike rides, play badminton, and practice carnatic singing.'
        },
        {
          name: 'Cyrus Ghane',
          title: 'Yale \'30',
          image: '/images/bio/cyrus.jpg',
          bio: 'Cyrus Ghane graduated from The Harker School in 2026. He has earned an honorable mention on the USAPhO and is a 3x AIME qualifier. He is especially interested in the intersection of physics and neuroscience and enjoys playing soccer and the guitar in his free time.'
        },
        {
          name: 'Jiaqi Wu',
          image: '/images/bio/jiaqi.jpeg',
          title: 'MIT \'30',
          bio: 'Jiaqi Wu graduated from Harvard-Westlake School in 2026. She is a US Physics Camp attendee, NAC gold medalist and Math Prize for Girls qualifier. Outside of physics and math, she likes to read and make desserts.'
        },
        {
          name: 'Shreyas Kini',
          image: '/images/bio/shreyas.jpg',
          title: 'Rice \'30',
          bio: 'Shreyas Kini graduated from Obra D. Tompkins High School in 2026. He is a two time USABO Semifinalist, the president of his science olympiad and biology clubs, and has placed as a runner up in the Brain Bee Texas division. Shreyas is excited to spread a passion for biology in others, as seen in his past experience as a director of the American Regional Biology Competition nonprofit. Outside of biology, Shreyas loves to play basketball, go on long runs, work out at the gym, and play the cello.'
        },
        {
          name: 'Anushka Polapally',
          image: '/images/bio/anushka.png',
          title: 'UT Austin \'30',
          bio: 'Anushka Polapally graduated from Obra D. Tompkins High School in 2026. She is an AIME qualifier and USACO Silver qualifier, along with being an officer of her school’s math club. Anushka is very passionate about teaching competition math to others, shown by her contribution to forming a contest math team and classes at her high school. In her free time, you can find Anushka listening to music, playing with her dog, and eating food with her friends.'
        },
        {
          name: 'Arjun Joisha',
          image: '/images/bio/arjunj.png',
          title: 'Georgia Tech \'30',
          bio: 'Arjun Joisha graduated from Lynbrook High School in 2026. He is a 3 time AIME qualifier, won a bronze medal twice and a silver medal once at the PiMC, and continues to compete in several other regional and college mathematics competitions, including the Stanford Math Tournament and the Berkeley Math Tournament. When not working on math competitions, he also enjoys competitive programming, and has reached USACO Gold. In his free time, you can find him hanging out with his friends, reading interesting math articles, or playing chess or Minecraft.'
        },
        {
          name: 'Terry Xie',
          image: '/images/bio/terry.png',
          title: 'Johns Hopkins \'30',
          bio: 'Terry graduated from The Harker School in 2026 and is passionate about biology and math. He is a USABO Semifinalist, and has qualified for AIME twice. He has also worked on an independent bioinformatics research project which he presented at the ICMI, and placed 8th at regional JSHS with. Terry has some wet lab experience as well through an internship at the Serrano lab through the BU RISE program. In his free time, Terry enjoys reading and playing water polo.'
        },
        {
          name: 'Karthik Veeramallu',
          image: '/images/bio/karthik.png',
          title: 'Brown \'30',
          bio: 'Karthik Veeramallu graduated from Obra D. Tompkins High School in 2026. He is an AIME qualifier, USAPhO qualifier, the president of his school physics club, and an officer of his school math club. Fluent in Java, he is interested in building projects and modeling real world scenarios. In his free time, he enjoys working his job, volunteering, and teaching independently.'
        },
        {
          name: 'Eric Dong',
          image: '/images/bio/eric.jpg',
          title: 'CMU \'30',
          bio: 'Eric Dong graduated from The Harker School in 2026. He is active in STEM competitions, having competed in, earned awards in, and prepared for the AMC, AIME, BMT, SMT, F=ma, and USAAAO. He is also a president of his school’s astronomy club and an active member of the science bowl team. He also enjoys engaging in research, having interned at UC Davis and having worked on a project about neutron star habitability. Outside of STEM, he is an avid clarinetist and competitive swimmer.'
        },
        {
          name: 'Vaishnav Krishnan',
          title: 'UT Austin \'30',
          image: '/images/bio/vaishnav.png',
          bio: 'Vaishnav graduated from Obra D. Tompkins High School in 2026. He represents his school in UIL Computer Science and is currently competing in USACO Gold. He is very passionate about teaching computer science and enjoys learning advanced techniques in computer science such as dynamic programming and segment trees. In his free time, he likes playing music and working out at the gym.'
        },
        {
          name: 'Akshitaa Arun',
          bio: 'Akshitaa Arun (Akshu/Ash) graduated high school in 2026 in Tamil Nadu, India. She has attended various math camps in India such as PROMYS INDIA 2024, RAMTP 2023, AGMNC 2022 & 2023. She is a teaching assistant Athemath, a part of the international outreach team of URBAN HARMONY PROJECT and runs NC^2! She enjoys tutoring outside school, and showing people that math can be fun! She loves puzzles (especially sudoku) and singing!',
          image: '/images/bio/akshitaa.png'
        },
        {
          name: 'Hengrui Liang',
          image: '/images/bio/hengrui.png',
          bio: 'Hengrui is a senior at The Harker School. He is a USAMO medalist, USAJMO Winner, and a BMT and SMT Distinguished HM. In his free time, he enjoys playing chess and board games, reading science magazines, and hiking.'
        },
        {
          name: 'William Jiang',
          image: '/images/bio/william.png',
          bio: 'William is a senior at The Harker School. He is very passionate about physics and chemistry, participating in competitions like USAYPT, Physics Brawl, and USNCO, as well as working on research projects related to the intersection of physics, chemistry, and machine learning. In his free time, he enjoys playing chess and solving interesting physics problems.'
        },
        {
          name: 'Melody Wang',
          image: '/images/bio/melody.png',
          bio: 'Melody Wang is a high school senior at Basis Independent Fremont. She is a USABO semifinalist and a BBO gold medalist. She leads the Neuroscience Club at her school and also teaches dance at different community organizations. She is also passionate about research, competing in the  California Science and Engineering Fair and also getting into Broadcom Masters Top 300. In her spare time she enjoys nature walks and baking.'
        },
        {
          name: 'Teresa Song',
          bio: 'Teresa Song is a junior at the Harker School and a two-time Scholastic Arts national gold medalist. In her free time, she can be found sneaking into the pantry for snacks, reading, or running.',
          image: '/images/bio/teresa.jpg'
        },
        {
          name: 'Sid Gaur',
          image: '/images/bio/sid.png',
          bio: 'Sid Gaur is a junior at The Harker School. He earned 2nd place statewide at both the California Science and Engineering Fair and the Synopsys Science and Engineering Fair. He was also recognized as a finalist in the Harvard Undergraduate Research Journal Competition. At Harker, he serves as Co-Captain of the Science Bowl Team. Outside of science, Sid enjoys playing badminton and singing in choir.'
        },
        {
          name: 'Annie Yu',
          image: '/images/bio/annie.png',
          bio: 'Annie Yu is a junior at The Harker School. She is a biology coach for Harker’s Middle School Science Bowl team and has taught at various other organizations. In her free time, she enjoys reading and writing literature, volunteering, and reading Campbell Biology.'
        }
      ]
    }
  },
  head () {
    return {
      title: 'Past Officers',
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
