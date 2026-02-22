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
          title: 'Massachusetts Institute of Technology \'28',
          image: '/images/bio/austin.jpg',
          bio: 'Austin Geng graduated from the Benjamin Franklin High School in 2024. He is an International Olympiad in Informatics Gold Medalist and Math Olympiad Program invitee and has narrowly missed a perfect AMC10. In both math and competitive programming, he especially enjoys ad hoc problems. In his free time, he likes to code (unrelatedly in JavaScript) and play video games.'
        },
        {
          name: 'Aniketh Tummala',
          title: 'Berkeley \'28',
          image: '/images/bio/aniketh.jpg',
          bio: 'Aniketh graduated from The Harker School in 2024. As well as being a USAPhO Silver medalist and top 50th in the nation in the Physics Bowl, he is a USACO Platinum contestant and 4 times AIME qualifier. In his free time, he enjoys taking his two dogs for walks around his neighborhood and playing the piano.'
        },
        {
          name: 'Harry Chen',
          title: 'California Institute of Technology \'28',
          image: '/images/bio/harry.jpg',
          bio: 'Harry graduated from Northwood High School in Irvine in 2024. He competed in USACO Platinum and has experience in full-stack web development. Harry also was involved with NLP research. In his free time Harry likes to play tennis.'
        },
        {
          name: 'Thomas Liu',
          title: 'Massachusetts Institute of Technology \'28',
          image: '/images/bio/thomas.jpg',
          bio: 'Thomas graduated from The Harker School in 2024. Fluent in C++, he enjoys competitive programming and is a USACO Finalist. In his spare time he enjoys playing video games and solving coding problems. He also dabbles in web development and AI.'
        },
        {
          name: 'Gautam Bhooma',
          title: 'Berkeley \'28',
          image: '/images/bio/gautam.jpg',
          bio: 'Gautam graduated from the Harker School in 2024. He is a National Top 300 Broadcom MASTERS Semifinalist after winning the Grand Prize of the Synopsys Championship in 2020. As the captain of the Harker Science Bowl team, he led his team to advance to the 2020 Science Bowl National Championships.'
        },
        {
          name: 'Arjun Gurjar',
          title: 'Berkeley \'28',
          image: '/images/bio/arjung.jpg',
          bio: 'Arjun Gurjar graduated from The Harker School in 2024. In addition to being a nationalist in the North South Science Bee, he is passionate about biology and has many years of experience in teaching students as well as conducting wet lab research. Apart from studying for USABO, Arjun likes editing videos, going on walks, and listening to music.'
        },
        {
          name: 'Kevin Zhang',
          title: 'University of Illinois Urbana-Champaign \'28',
          image: '/images/bio/kevin.png',
          bio: 'Kevin graduated from The Harker School in 2024. Besides studying computer science and physical sciences, he is also interested in arts and design with experience in digital mediums such as Photoshop and Canva. He was also a graphic designer for the Harker Programming Club and produced media for his school’s journalism program too. In his free time, he enjoys photo and video editing, as well as playing and watching basketball.'
        },
        {
          name: 'Dustin Miao',
          title: 'Carnegie Melon University \'28',
          image: '/images/bio/dustin.jpg',
          bio: 'Dustin graduated from the Harker School in 2024. He is in USACO\'s platinum division and a master on Codeforces, and is also interested in web development and artificial intelligence. In his spare time, he enjoys playing cello.'
        },
        {
          name: 'Arnav Swaroop',
          title: 'Berkeley \'28',
          image: '/images/bio/arnav.png',
          bio: 'Arnav Swaroop graduated from The Harker School in 2024. He enjoys Physics, Earth+Space Science, and biology. He is a USESO finalist, a USABO semifinalist, and has other STEM accolades in the above fields. He won the Regional Science Bowl in 2020, and was part of Harker\'s High School Science Bowl A Team and a senior Middle School Science Bowl coach. When not studying science, he works on his diverse array of research projects ranging from astrophysics to biochemistry.'
        },
        {
          name: 'Henry Yao',
          title: 'Johns Hopkins University \'28',
          image: '/images/bio/henry.png',
          bio: 'Henry graduated from Lynbrook High School in 2024. He is passionate about STEM overall, and has won USAJMO HM and AMC10 DHR three times, and came close to USAPHO along with 5\'s in most AP Physics content. He is also passionate about STEM research and has taught and TA\'d classes at Alphastar and other summer camps. When he isn\'t grinding school, Henry enjoys biking, eating food, and listening to music.'
        },
        {
          name: 'Andrew Xie',
          title: 'Massachusetts Institute of Technology \'29',
          image: '/images/bio/andrewxie.jpg',
          bio: 'Andrew (Weian) Xie is a senior at The Hotchkiss School in Connecticut. An avid fan of math contests, he has qualified for the AIME 4 times, USAJMO 2 times, where he earned Top Winner and attended MOP in 2023. He is very passionate about promoting mathematical interest in younger kids, especially in under-represented communities, having co-founded a middle school math competition sponsored by his school, as well as AoPS and AwesomeMath. Outside of math, he enjoys playing the piano, reading poetry, cross country practice, and listening to R&B.'
        },
        {
          name: 'Andrew Liang',
          title: 'Stanford University \'29',
          image: '/images/bio/andrew.png',
          bio: 'Andrew Liang graduated from The Harker School in 2025. He is a USACO Gold contestant and International Science and Engineering Fair (ISEF) Finalist. He enjoys teaching other students and helping them discover their own passions. In his spare time, he likes to play chess and listen to classical music.'
        },
        {
          name: 'Alex Huang',
          title: 'University of Southern California \'29',
          image: '/images/bio/alex.jpg',
          bio: 'Alex Huang graduated from The Harker School in 2025 and is a 2021 MathCounts National Round qualifier, four-time AIME qualifier, participant in The Ross Mathematics Program 2023 and 2024, and PRIMES-USA 2024 researcher. Fluent in C++, Java, and Python, he enjoys applying scientific machine learning to elucidate biophysical processes. To disseminate his knowledge to aspiring students, he has led volunteer teaching initiatives and has won the President\'s Volunteer Service Gold Award three times. In his free time, he enjoys playing bridge and engaging friends in thought-provoking conversations.'
        },
        {
          name: 'Juliana Li',
          image: '/images/bio/juliana.png',
          title: 'Harvard University \'29',
          bio: 'Juliana Li graduated from The Harker School in 2025. She is a 4x AIME qualifier, was invited to MathCounts Nationals, is competing in USACO Gold, and won 1st place in biology research at both the local & state science fair. In her free time, she enjoys web/app development, volunteering, and dancing.'
        },
        {
          name: 'Jacqueline Huang',
          image: '/images/bio/jacqueline.png',
          title: 'Stanford University \'29',
          bio: 'Jacqueline Huang graduated from The Harker School in 2025. She is a USAPhO medalist, 4x AIME qualifier, and has several years of experience in teaching math and science. She enjoys hiking and reading in her free time.'
        },
        {
          name: 'Aarush Vailaya',
          image: '/images/bio/aarush.jpg',
          title: 'Massachusetts Institute of Technology \'29',
          bio: 'Aarush Vailaya graduated from The Harker School in 2025. He is a 5 time qualifier of AIME, USAMO gold medalist, won 1st place in both the Synopsys Physical Sciences & Engineering as well as the Bay Area Math Olympiad, a USAMTS gold medalist, and competed in many math events, including the Stanford Math Tournament, AMC 10, and AIME. He also participated in the HCSSiM and SUMaC summer programs, and does math research through PRIMES-USA. While not doing math, he enjoys working on random coding projects, grinding Wynncraft, and playing piano.'
        },
        {
          name: 'Neil Krishnan',
          image: '/images/bio/neil.jpg',
          title: 'Massachusetts Institute of Technology \'29',
          bio: 'Neil Krishnan graduated from The Harker School in 2025. In addition to getting 1st award in Synopsys Physical Sciences & Engineering and qualifying for CSEF and Broadcom Masters, he has done a lot of math as a five-time AIME qualifier, USAMO silver medalist, USAMTS gold winner (near perfect score), and recipient of multiple distinguished honorable mentions in BMT. He has also participated in in math summer programs, namely Hampshire College Summer Studies in Mathematics and USA-Canada MathCamp. Neil also likes doing mathematical research on friends-and-stranger graphs and graph connectivity. In his free time, he enjoys playing piano and doing NYT mini crosswords (and the regular if he feels smart that day).'
        },
        {
          name: 'Sophia Liu',
          image: '/images/bio/sophia.png',
          title: 'Stanford University \'29',
          bio: 'Sophia Liu graduated from The Harker School in 2025. A lover of graphic design and fine arts, she manages outreach/media for a few organizations, serves as an art editor for The Expressionist, and is a Scholastic Arts national gold and silver medalist. Aside from art, she researches childhood cognitive development and neuroscience.'
        },
        {
          name: 'James Lin',
          image: '/images/bio/james.png',
          bio: 'James Lin is a senior at The Harker School. He is a USACO platinum contestant, three-time AIME qualifier, and USAJMO qualifier. He has also competed in many math and computer science competitions, such as SMT, Teamscode, and LIT. In his free time, he reads and listens to music.'
        },
        {
          name: 'Samuel Tong',
          image: '/images/bio/samuel.png',
          bio: 'Samuel is a senior at The Harker School. He competes in the USACO Gold division, and he uses his expertise in computer science on bioinformatics and drug reaction models. Samuel is a retired fencer, and he loves watching dramas and walking his dog.'
        },
        {
          name: 'Suhani Pahuja',
          image: '/images/bio/suhani.jpg',
          bio: 'Suhani is a senior at Monta Vista High School in Cupertino, California. She is a multiple-time AIME qualifier with a high score of 7 and has earned awards at competitions like PUMaC, SMT, and BMT as well. Suhani is very passionate about teaching mathematics and spreading her knowledge, and is also the president of her school’s math club and an officer since her sophomore year. Suhani is also an avid researcher, competing in regional and state-level research competitions such as Synopsys, JSHS, and CSEF, and publishing her work in journals as well. Apart from math and pursuing research, she has profound interests in biology and physics as well, challenging herself with rigorous coursework and competing and earning awards in the USABO open exam. In her free time, Suhani enjoys running, playing piano, and spending time with her friends and family.'
        },
        {
          name: 'Sid Gaur',
          image: '/images/bio/sid.png',
          bio: 'Sid Gaur is a sophomore at The Harker School. He earned 2nd place statewide at both the California Science and Engineering Fair and the Synopsys Science and Engineering Fair. He was also recognized as a finalist in the Harvard Undergraduate Research Journal Competition. At Harker, he serves as Co-Captain of the Science Bowl Team. Outside of science, Sid enjoys playing badminton and singing in choir.'
        },
        {
          name: 'Jiaqi Wu',
          image: '/images/bio/jiaqi.jpeg',
          bio: 'Jiaqi Wu is a senior at Harvard-Westlake School. She is a US Physics Camp attendee, NAC gold medalist and Math Prize for Girls qualifier. Outside of physics and math, she likes to read and make desserts.'
        },
        {
          name: 'Anushka Polapally',
          image: '/images/bio/anushka.png',
          bio: 'Anushka Polapally is a senior at Obra D. Tompkins High School in Katy, Texas. She is an AIME qualifier and USACO Silver qualifier, along with being an officer of her school’s math club. Anushka is very passionate about teaching competition math to others, shown by her contribution to forming a contest math team and classes at her high school. In her free time, you can find Anushka listening to music, playing with her dog, and eating food with her friends.'
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
