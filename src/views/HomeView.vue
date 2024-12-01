<script setup>
import BlendsInfluencedBy from "../components/BlendsInfluencedBy.vue";
import MultiArtistSelect from "../components/MultiArtistSelect.vue";
</script>

<template>
  <div class="max-w-[1500px] mx-auto">
    <div class="px-8 mt-8 min-w-[800px] w-full">
      <div class="text-white text-xl font-semibold inline-block">
        Blends influenced by...
        <div class="text-sm font-normal text-[#1781f0]">
          Find new tracks that match your favorites
        </div>
      </div>

      <div class="py-3"></div>

      <div class="flex justify-between w-full gap-8">
        <div class="xl:w-1/3 w-1/2">
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Only Teardrops"
            by="Emilie de Forest"
            to="/artist"
            image="https://is1-ssl.mzstatic.com/image/thumb/Music2/v4/0c/c8/0f/0cc80f43-d7d1-31b5-724a-8b41b22787de/886443998551.jpg/1200x1200bb.jpg"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Kedvesem"
            by="ByeAlex"
            to="/artist"
            image="https://cdn-images.dzcdn.net/images/cover/93c395ff3734e20bbc2f9cb064bc2e2d/0x1900-000000-80-0-0.jpg"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Human"
            by="OneRepublic"
            to="/artist"
            image="https://store.onerepublic.com/cdn/shop/files/1R_OhMyMy_AlbumCover.jpg?v=1686938810"
          />
        </div>
        <div class="xl:w-1/3 w-1/2">
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Sorry Not Sorry"
            by="Demi Lovato"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/en/1/13/Sorry_Not_Sorry_%28Official_Single_Cover%29_by_Demi_Lovato.png"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="The Way You Make Me Feel"
            by="Michael Jackson"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/ru/a/aa/Michael_Jackson_%E2%80%94_The_Way_You_Make_Me_Feel_single_cover.jpg"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="The Moon Is Rising"
            by="Samanta Tīna"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/en/3/3a/The_Moon_Is_Rising.jpg"
          />
        </div>
        <div class="xl:w-1/3 w-1/2">
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Visionary Dream"
            by="Sopho"
            to="/artist"
            image="https://i.discogs.com/4rxAVFSe-3BfWPoSCu_KRnlnM94QGbX2syZiZgps3Dk/rs:fit/g:sm/q:90/h:598/w:600/czM6Ly9kaXNjb2dz/LWRhdGFiYXNlLWlt/YWdlcy9SLTExMjMz/ODY5LTE1MTI5MDUw/NTUtNTc5MS5qcGVn.jpeg"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="willow"
            by="Taylor Swift"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/ru/9/9a/Taylor_Swift_-_Willow.png"
          />
          <BlendsInfluencedBy
            class="pb-1.5"
            text="Ride"
            by="twenty one pilots"
            to="/artist"
            image="https://upload.wikimedia.org/wikipedia/ru/1/19/Twenty_one_pilots_ride_cover.jpg"
          />
        </div>
      </div>

      <div class="px-8 mt-8 min-w-[800px]">
        <div class="text-white text-xl font-semibold inline-block">
          Created for you
        </div>

        <div class="py-3"></div>

        <div class="flex justify-start gap-7">
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Katy Perry, Britney Spears and Drax Project"
            to="/artist"
            :images="{
              one: 'https://miro.medium.com/v2/resize:fit:681/1*EBOL4lka5QjcYoxj6AHp-g.png',
              two: 'https://aimm.edu/hubfs/Blog%20Images/Top%2010%20Album%20Covers%20of%202017/Tyler%20the%20Creator-%20Flower%20boy.jpg',
              three:
                'https://upload.wikimedia.org/wikipedia/commons/3/33/Are_You_Experienced_-_US_cover-edit.jpg',
              four: 'https://www.billboard.com/wp-content/uploads/2022/06/beyonce-Lemonade-album-art-billboard-1240.jpg?w=600',
            }"
          />
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Hailee Steinfeld, Little Mix and Nicki Minaj"
            to="/artist"
            :images="{
              one: 'https://www.usatoday.com/gcdn/authoring/authoring-images/2024/04/18/USAT/73369584007-013-1989-taylors-version-2023.jpeg',
              two: 'https://www.skillshare.com/blog/wp-content/uploads/2016/06/ScreenShot2020-10-20at11.36.46AM.png',
              three:
                'https://qodeinteractive.com/magazine/wp-content/uploads/2020/06/16-Tame-Impala.jpg',
              four: 'https://www.sleek-mag.com/wp-content/uploads/2017/05/takashi_murakami_kanye_west.jpg',
            }"
          />
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Dana International, Claudia Pascoal and Beyoncé"
            to="/artist"
            :images="{
              one: 'https://pure-music.co.uk/wp-content/uploads/2019/04/Thriller-Album-Cover.png',
              two: 'https://www.indieground.net/images/blog/2024/indieblog-best-album-covers-2010s-23.jpg',
              three:
                'https://images.theconversation.com/files/512871/original/file-20230301-26-ryosag.jpg?ixlib=rb-4.1.0&rect=97%2C79%2C5799%2C5817&q=45&auto=format&w=926&fit=clip',
              four: 'https://cdn-images.dzcdn.net/images/cover/967ac8605268db88a1e597394115365d/1900x1900-000000-80-0-0.jpg',
            }"
          />
          <MultiArtistSelect
            class="w-1/4"
            category="daily"
            text="Featuring Raiven, Natalia Barbu and One Direction"
            to="/artist"
            :images="{
              one: 'https://www.billboard.com/wp-content/uploads/media/ariana-grande-sweetner-album-art-2018-billboard-1240.jpg?w=600',
              two: 'https://www.billboard.com/wp-content/uploads/2022/03/48.-Lady-Gaga-%E2%80%98The-Fame-Monster-2009-album-art-billboard-1240.jpg?w=600',
              three:
                'https://www.billboard.com/wp-content/uploads/2023/07/rihanna-anti-cover-2016-billboard-1240.jpg?w=600',
              four: 'https://www.billboard.com/wp-content/uploads/2022/03/35.-Metallica-%E2%80%98Master-of-Puppets-1986-album-art-billboard-1240.jpg?w=600',
            }"
          />
        </div>
      </div>

      <div class="px-8 mt-14 min-w-[800px]">
        <div class="py-3">
          <p class="text-center pb-6 text-[#b117f0] text-sm">
            Unlock Flow by choosing your favorite artists for better
            recommendations
          </p>

          <div class="flex justify-center gap-7 full">
            <div class="flex items-center justify-center relative">
              <img
                src="https://cms-assets.tutsplus.com/cdn-cgi/image/width=850/uploads/users/114/posts/34296/final_image/Final-image.jpg"
                alt=""
                class="absolute -left-36 rounded-full z-0 cursor-pointer"
                width="100"
              />
              <img
                src="https://res.cloudinary.com/zenbusiness/image/upload/v1670445040/logaster/logaster-2021-02-douqir-u4aaozip-1024x1024.jpg"
                alt=""
                class="absolute -left-[80px] rounded-full z-10 cursor-pointer"
                width="100"
              />
              <img
                src="https://www.premadepixels.com/wp-content/uploads/2020/11/Unknown-Album-Cover-PP1.jpg"
                alt=""
                class="rounded-full z-20 cursor-pointer"
                width="100"
              />
              <img
                src="https://www.billboard.com/wp-content/uploads/2022/03/7.-Nirvana-%E2%80%98Nevermind-1991-album-art-billboard-1240.jpg?w=600"
                alt=""
                class="absolute -right-[80px] rounded-full z-10 cursor-pointer"
                width="100"
              />
              <img
                src="https://s.yimg.com/ny/api/res/1.2/TdT5KvjU14pp8TUgwnvMsw--/YXBwaWQ9aGlnaGxhbmRlcjt3PTk2MDtoPTk2MA--/https://media.zenfs.com/en/one37pm_956/72d7b3dc8acef1991bb74d8e90c9ceab"
                alt=""
                class="absolute -right-36 rounded-full z-0 cursor-pointer"
                width="100"
              />
            </div>
          </div>
        <div class="w-full flex justify-center p-3">
          <button 
            type="button" 
            class="text-white text-[15px] font-semibold rounded-full bg-[#EF5465] hover:bg-[#d8384a] px-8 py-2 text-center"
          >
            ADD ARTISTS
          </button>
        </div>
    </div>

    <div class="mt-8 min-w-[800px]">
      <CustomCarousel 
        category="New releases for you"
        :data="[
          { url: 'https://picsum.photos/id/89/300/300', song: 'Foregone', by: 'In Flames', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/101/300/300', song: 'Dark Waters', by: 'Delain', releasedOn: '09/01/2023' },
          { url: 'https://picsum.photos/id/121/300/300', song: 'Heritage', by: 'Distant', releasedOn: '10/01/2023' },
          { url: 'https://picsum.photos/id/134/300/300', song: 'Meanwhile', by: 'Klone', releasedOn: '08/02/2023' },
          { url: 'https://picsum.photos/id/144/300/300', song: 'Truth Decay', by: 'You Me At Six', releasedOn: '10/01/2023' },
          { url: 'https://picsum.photos/id/155/300/300', song: 'This Is Why', by: 'Paramore', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/166/300/300', song: 'The Jaws Of Life', by: 'Pierce The Veil', releasedOn: '09/23/2023' },
          { url: 'https://picsum.photos/id/198/300/300', song: 'The Future Is Your Past', by: 'In The Brian Jonestown Massacre', releasedOn: '07/25/2023' },
          { url: 'https://picsum.photos/id/211/300/300', song: 'The Land, The Water, The Sky', by: 'Black Belt Eagle Scout', releasedOn: '09/22/2023' },
          { url: 'https://picsum.photos/id/223/300/300', song: 'The Day My Father Died', by: 'SYML', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/225/300/300', song: 'Complete Mountain Almanac', by: 'Complete Mountain Almanac', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/239/300/300', song: 'Music From Montana Story', by: 'Kevin Morby', releasedOn: '10/01/2023' },
        ]"
      />
    </div>

    <div class="px-8 mt-8 min-w-[800px]">
      <div class="text-white text-xl font-semibold inline-block">
            Highlights
        </div>

        <div class="py-3"></div>

        <div class="flex items-center gap-8">
          <div class="rounded-lg w-1/2">
            <Highlights 
              by="Some Artist 1"
              song="Awsome Song for you!"
              image="https://picsum.photos/id/220/800/300"
            />
          </div>
          <div class="rounded-lg w-1/2">
            <Highlights 
              by="Some Artist 2"
              song="Another banger BRUV!"
              image="https://picsum.photos/id/229/800/300"
            />
          </div>
        </div>
    </div>

    <div class="mt-8 min-w-[800px]">
      <CustomCarousel 
        category="Popular playlist"
        :data="[
          { url: 'https://picsum.photos/id/54/300/300', song: 'Foregone', by: 'In Flames', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/102/300/300', song: 'Dark Waters', by: 'Delain', releasedOn: '09/01/2023' },
          { url: 'https://picsum.photos/id/126/300/300', song: 'Heritage', by: 'Distant', releasedOn: '10/01/2023' },
          { url: 'https://picsum.photos/id/136/300/300', song: 'Meanwhile', by: 'Klone', releasedOn: '08/02/2023' },
          { url: 'https://picsum.photos/id/146/300/300', song: 'Truth Decay', by: 'You Me At Six', releasedOn: '10/01/2023' },
          { url: 'https://picsum.photos/id/156/300/300', song: 'This Is Why', by: 'Paramore', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/165/300/300', song: 'The Jaws Of Life', by: 'Pierce The Veil', releasedOn: '09/23/2023' },
          { url: 'https://picsum.photos/id/196/300/300', song: 'The Future Is Your Past', by: 'In The Brian Jonestown Massacre', releasedOn: '07/25/2023' },
          { url: 'https://picsum.photos/id/216/300/300', song: 'The Land, The Water, The Sky', by: 'Black Belt Eagle Scout', releasedOn: '09/22/2023' },
          { url: 'https://picsum.photos/id/222/300/300', song: 'The Day My Father Died', by: 'SYML', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/227/300/300', song: 'Complete Mountain Almanac', by: 'Complete Mountain Almanac', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/237/300/300', song: 'Music From Montana Story', by: 'Kevin Morby', releasedOn: '10/01/2023' },
        ]"
      />
    </div>

    <div class="px-8 mt-8 min-w-[800px]">
      <div class="text-white text-xl font-semibold inline-block">
            Highlights
        </div>

        <div class="py-3"></div>

        <div class="flex items-center gap-8">
          <div class="rounded-lg w-1/2">
            <Highlights 
              by="Some Artist 1"
              song="Awsome Song for you!"
              image="https://picsum.photos/id/177/800/300"
            />
          </div>
          <div class="rounded-lg w-1/2">
            <Highlights 
              by="Some Artist 2"
              song="Another banger BRUV!"
              image="https://picsum.photos/id/126/800/300"
            />
          </div>
        </div>
    </div>

    <div class="mt-8 min-w-[800px]">
      <CustomCarousel 
        category="New releases for you"
        :data="[
          { url: 'https://picsum.photos/id/134/300/300', song: 'Foregone', by: 'In Flames', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/144/300/300', song: 'Dark Waters', by: 'Delain', releasedOn: '09/01/2023' },
          { url: 'https://picsum.photos/id/146/300/300', song: 'Heritage', by: 'Distant', releasedOn: '10/01/2023' },
          { url: 'https://picsum.photos/id/78/300/300', song: 'Meanwhile', by: 'Klone', releasedOn: '08/02/2023' },
          { url: 'https://picsum.photos/id/151/300/300', song: 'Truth Decay', by: 'You Me At Six', releasedOn: '10/01/2023' },
          { url: 'https://picsum.photos/id/155/300/300', song: 'This Is Why', by: 'Paramore', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/167/300/300', song: 'The Jaws Of Life', by: 'Pierce The Veil', releasedOn: '09/23/2023' },
          { url: 'https://picsum.photos/id/191/300/300', song: 'The Future Is Your Past', by: 'In The Brian Jonestown Massacre', releasedOn: '07/25/2023' },
          { url: 'https://picsum.photos/id/194/300/300', song: 'The Land, The Water, The Sky', by: 'Black Belt Eagle Scout', releasedOn: '09/22/2023' },
          { url: 'https://picsum.photos/id/177/300/300', song: 'The Day My Father Died', by: 'SYML', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/227/300/300', song: 'Complete Mountain Almanac', by: 'Complete Mountain Almanac', releasedOn: '10/02/2023' },
          { url: 'https://picsum.photos/id/232/300/300', song: 'Music From Montana Story', by: 'Kevin Morby', releasedOn: '10/01/2023' },
        ]"
      />
    </div>

    <div class="pb-40"></div>
  </div>
</template>
