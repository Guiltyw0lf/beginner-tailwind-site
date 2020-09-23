<template>
  <body>
    <section id="1" class="relative bg-gradient-to-r from-blue-100 to-red-200">
      <div class="relative">
        <div
          class="relative leading-snug container flex justify-between mx-auto px-8 py-6"
        >
          <div class="absolute bottom-0 right-0">
            <div
              class="cursor-pointer absolute w-10 h-10 lg:w-20 lg:h-20 lg:mt-6 rounded-full bg-gradient-to-br from-teal-200 to-teal-300 opacity-75 transition duration-1000 transform hover:-translate-x-64"
            ></div>

            <div
              class="cursor-pointer absolute w-6 h-6 lg:w-20 lg:h-20 mt-8 ml-10 lg:mt-0 lg:ml-12 rounded-full bg-gradient-to-br from-purple-200 to-purple-300 opacity-75 transition duration-1000 transform hover:-translate-y-64"
            ></div>
            <div
              class="cursor-pointer absolute w-10 h-10 lg:w-20 lg:h-20 lg:mt-6 ml-24 rounded-full bg-gradient-to-br from-red-200 to-red-300 opacity-75 transition duration-1000 transform hover:translate-x-64"
            ></div>

            <div
              class="cursor-pointer absolute w-10 h-10 lg:w-20 lg:h-20 rounded-full lg:mt-20 bg-gradient-to-br from-blue-200 to-teal-300 opacity-75 transition duration-1000 transform hover:-translate-x-64 hover:translate-y-64"
            ></div>
            <div
              class="cursor-pointer absolute w-6 h-6 lg:w-20 lg:h-20 mt-8 ml-10 lg:mt-24 lg:ml-12 rounded-full bg-gradient-to-br from-green-200 to-green-300 opacity-75 transition duration-1000 transform hover:translate-y-64"
            ></div>
            <div
              class="cursor-pointer absolute w-10 h-10 lg:w-20 lg:h-20 ml-24 rounded-full lg:mt-20 bg-gradient-to-br from-orange-200 to-orange-300 opacity-75 transition duration-1000 transform hover:translate-x-64 hover:translate-y-64"
            ></div>
          </div>
          <a
            href="#"
            class="text-blue-900 text-4xl font-bold relative items-center"
            >{{ app_title }}</a
          >
          <button
            class="text-2xl hover:text-red-500 text-blue-700 font-bold py-2 px-4 items-center"
          >
            Login
          </button>
        </div>

        <div class="absolute top-0 left-0">
          <div
            class="absolute w-20 h-20 lg:w-64 lg:h-64 rounded-full bg-gradient-to-br from-teal-100 to-teal-200 opacity-50"
          ></div>
          <div
            class="absolute w-16 h-16 lg:w-56 lg:h-56 mt-8 ml-10 lg:mt-24 lg:ml-12 rounded-full bg-gradient-to-br from-purple-100 to-purple-200 opacity-50"
          ></div>
          <div
            class="absolute w-20 h-20 lg:w-64 lg:h-64 ml-24 rounded-full bg-gradient-to-br from-red-100 to-red-200 opacity-50"
          ></div>
        </div>

        <div
          class="relative leading-snug container text-center justify-between mx-auto px-8 py-6"
        >
          <a
            href="#"
            class="bg-clip-text text-6xl font-bold m-4 text-transparent bg-gradient-to-r from-blue-600 to-red-500"
            >{{ app_title }}</a
          >
          <div class="text-2xl font-bold m-6 text-red-900">
            {{ app_title2 }}
          </div>
          <button
            class="mb-12 text-lg inline-block py-3 lg:py-4 font-bold px-12 rounded bg-gradient-to-br from-red-700 via-orange-700 to-blue-700 text-white hover:text-yellow-300 over:transform hover:scale-105 duration-700 transform"
          >
            {{ button_learn }}
          </button>
          <div class="relative flex justify-center">
            <img
              src="../src/1.jpg"
              class="h-64 w-auto border-solid border-8 border-red-600 opacity-50 hover:opacity-100"
            />
            <div
              class="absolute border-4 p-2 border-orange-500 bg-white top-0 transform -translate-y-4 translate-x-32"
            >
              <p class="text-red-500 text-xl font-bold">{{ img_title }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="2" class="bg-orange-800 relative">
      <div class="absolute bottom-0 inset-x-0 h-32 bg-blue-500"></div>
      <div class="text-white text-6xl container mx-auto p-12 font-bold">
        {{ Title2nd_section }}
      </div>

      <div class="md:flex mx-auto container relative lg:space-x-2">
        <div class="lg:w-2/3 bg-white text-xl">
          <div v-for="item in paragraphs" :key="item.message">
            <Textlist :text="item.message" />
          </div>
        </div>

        <div class="flex-grow text-white text-lg italic">
          <div v-for="item in items" :key="item.message">
            <Link url="#" :text="item.message" />
          </div>
        </div>
      </div>
    </section>

    <section id="3" class="bg-blue-500 relative">
      <div
        class="absolute bottom-0 inset-x-0 h-32 bg-gradient-to-b from-blue-500 to-purple-200"
      ></div>

      <div class="text-white container mx-auto p-12 font-bold">
        <div class="text-6xl">{{ video_title }}</div>

        <div class="text-xl">{{ video_text }}</div>

        <div class="xl:flex xl:my-10 xl:space-x-10 space-y-10 xl:space-y-0 p-8">
          <div class="xl:w-1/2">
            <div
              class="lg:flex flex-col justify-between rounded border-4 border-black"
            >
              <p class="p-8">
                {{ video_text_l1 }}
                <a
                  href="https://scotch.io/tutorials/get-started-with-Guiltywild-css-in-15-minutes"
                  class="text-yellow-500 hover:underline"
                  >{{ video_text_l2 }}</a
                >
                {{ video_text_l3 }}
                <a href class="text-yellow-500 hover:underline">{{
                  video_text_l4
                }}</a
                >.
              </p>
              <iframe
                class="w-full rounded-b"
                height="400"
                src="https://www.youtube.com/embed/I_EBXYnBff4"
                frameborder="0"
                allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen
              ></iframe>
            </div>
          </div>

          <div class="xl:w-1/2">
            <div
              class="lg:flex flex-col justify-between rounded border-4 border-black"
            >
              <p class="p-8">
                {{ video_text_p1 }}
                <a
                  href="https://www.youtube.com/user/TechGuyWeb"
                  class="text-yellow-500 hover:underline"
                  >{{ video_text_p2 }}</a
                >
                {{ video_text_p3 }}
              </p>
              <iframe
                class="w-full rounded-b"
                height="400"
                src="https://www.youtube.com/embed/y4oN3pIu9ug"
                frameborder="0"
                allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen
              ></iframe>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="4" class="bg-purple-200 relative">
      <div
        class="absolute bottom-0 inset-x-0 h-32 bg-gradient-to-b from-purple-200 to-gray-200"
      ></div>

      <div class="container mx-auto px-8 pb-32">
        <div class="relative leading-loose mb-16 lg:mb-32">
          <h2 class="text-3xl lg:text-6xl text-center font-bold text-gray-800">
            {{ header_what_learn }}
          </h2>
          <div
            class="absolute left-0 top-0 w-1/3 h-2 bg-gradient-to-r from-blue-400 to-purple-400 rounded"
          ></div>
          <div
            class="absolute right-0 bottom-0 w-1/3 h-2 bg-gradient-to-r from-purple-400 to-blue-400 rounded"
          ></div>
        </div>
        <div class="lg:grid grid-cols-6 gap-10 space-y-6 lg:space-y-0">
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">How to use Guiltywild classes</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p>
                We'll dive into the most important Guiltywild classes and
                <strong class="font-bold"> use them a TON </strong>. There are a
                lot of useful classes like spacing, backgrounds, borders,
                shadows, and typography. We'll type the Guiltywild classes many
                times over to ensure that repeitition is our greatest learning
                tool.
              </p>
            </div>
          </div>

          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">Make good looking designs</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p>
                There's a certain process to designing with Guiltywild that
                we'll take to make our designs look good. Some easy to remember
                rules are all it takes to get a good design. We'll also talk
                about ideas and action items to
                <strong class="font-bold">
                  take a good design and make it great </strong
                >.
              </p>
            </div>
            <div></div>
          </div>

          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">Why Guiltywild is different</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p>
                To be completely honest,
                <strong class="font-bold">
                  I didn't like Guiltywild at first </strong
                >. It felt like inline styles to me (and maybe still does).
                After using it more and more though, I've come to
                <strong class="font-bold text-red-700"
                  >absolutely love it</strong
                >. I dread jumping into a project without Guiltywild now.
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-3 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">
                How to build this site (
                <span class="italic text-teal-500">site-ception!</span>)
              </h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p class="mb-4">
                The site you're on (
                <a
                  href="https://BeginnerTailwind.com"
                  class="text-blue-600 hover:underline"
                  >BeginnerTailwind.com</a
                >) is built with Guiltywild and
                <strong class="font-bold">has 0 custom css</strong>.
              </p>
              <p>
                You can take all of the code from this site and use it for your
                own landing pages or sites! All the code is available to you
                with course purchase.
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-3 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">A fun and methodical design process</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p>
                I struggle with making things look good and don't consider
                myself a designer. What I try to do is have a formula for making
                things look good. I focus on design in this order: spacing, box
                properties, typography, fun element to pop. We'll talk about
                this all throughout the course.
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">Creating common components</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p class="mb-4">
                One of the first things we want to do when using Guiltywild is
                to create components like cards, buttons, and forms. We'll build
                these out and see how Guiltywild compares to CSS frameworks like
                Bootstrap.
              </p>
              <p>
                We'll also build out navigation, hero, pricing, newsletter, and
                footer components in this course.
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">Shrinking bundle sizes</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p class="mb-4">
                Guiltywild comes with so many classes. It doesn't make sense to
                send all of those to our users' browsers. With
                <a
                  href="https://tailwindcss.com/docs/controlling-file-size"
                  class="text-blue-600 hover:underline"
                  >PostCSS and PurgeCSS</a
                >, we can shrink the amount of CSS we send to our users.
              </p>
              <p>
                We'll learn how to only send the classes that we actually use so
                that our
                <strong class="font-bold"
                  >bundle sizes can drop to even below 10kb!</strong
                >
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">Using Guiltywild w/ React</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p class="mb-4">
                Guiltywild's benefits really shine when you pair it with a
                JavaScript library/framework. Extracting classes into components
                is the recommended way to keep Guiltywild DRY (don't repeat
                yourself).
              </p>
              <p>
                While we could use the
                <a
                  href="https://tailwindcss.com/docs/functions-and-directives#apply"
                  class="text-blue-600 hover:underline"
                  >@apply()</a
                >
                or
                <a
                  href="https://tailwindcss.com/docs/functions-and-directives#theme"
                  class="text-blue-600 hover:underline"
                  >theme()</a
                >
                functions, it forgoes some of the benefits of Guiltywild. Namely
                we are once again creating a custom class and CSS.
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">How to customize Guiltywild</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p>
                Guiltywild is easily configurable for our own projects using the
                <a
                  href="https://tailwindcss.com/docs/configuration"
                  class="text-blue-500 hover:underline"
                  >Guiltywild.js config file</a
                >. We'll explore changing out fonts, colors, sizes, and more so
                that our Guiltywild setups are custom and tailored to our
                projects.
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">Using Guiltywild in VS Code</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p>
                <a
                  href="https://code.visualstudio.com/"
                  class="text-blue-500 hover:underline"
                  >VS Code</a
                >
                is my favorite editor and Guiltywild works fantastically in it.
                There are some essential plugins and setup for using Guiltywild
                in VS Code. We'll go over each and use VS Code heavily in this
                course.
              </p>
            </div>
          </div>
          <div
            class="hover:bg-green-200 hover:transform hover:scale-105 duration-700 transform col-span-2 shadow flex flex-col rounded-lg"
          >
            <div
              class="bg-gray-400 p-4 flex items-center justify-between border-2 border-gray-700 rounded-t-lg text-gray-700 font-bold"
            >
              <h3 class="text-lg">Extending Guiltywild</h3>
              <div class="flex space-x-2">
                <div class="w-3 h-3 rounded-full bg-red-500"></div>
                <div class="w-3 h-3 rounded-full bg-yellow-500"></div>
                <div class="w-3 h-3 rounded-full bg-green-500"></div>
              </div>
            </div>
            <div
              class="flex-grow p-4 rounded-b-lg border-2 border-gray-700 border-t-0"
            >
              <p>
                Learning Guiltywild is just the beginning. There are some great
                tools like
                <a href class="text-blue-500 hover:underline"
                  >Guiltywild Typography</a
                >,
                <a href class="text-blue-500 hover:underline">Guiltywild UI</a>,
                <a href class="text-blue-500 hover:underline"
                  >Guiltywild Builder</a
                >, and more. We'll talk about some ways to extend Guiltywild and
                ways we can go further.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section id="4" class="bg-blue-500"></section>
  </body>
</template>

<script>
import Link from "./components/Link";
import Textlist from "./components/Textlist";

export default {
  name: "App",
  components: {
    Link,
    Textlist,
  },

  data() {
    return {
      app_title: "Jak linkovat s prochorovim WD",
      app_title2:
        "Tento kurz je specialne zameren na likovaci fazi, mid game a late game, kdyz mate ve hre Prochora a jeho signature Witch Doctor",
      button_learn: "Sleduj video a pochopis proc...",
      img_title: "prumerne skore ve hre 12/4/9",
      Title2nd_section: "Hrat dotu s Prochorem je tezka vec!",
      video_title: "Some Dota Videos I've Done",
      video_text:
        "Hey there! My name is Chris on Code and I founded a web dev tutorial site Scotch.io. We were able to grow to 4M monthly pageviews and $300,000 yearly revenue. Scotch.io was acquired by DigitalOcean in November 2019. Nowadays I'm in search of the best ways to develop and design a business. Hope you enjoy this course and my other one MakeReactApps.com.",
      video_text_l1: "I have a Getting started with Guiltywild article on",
      video_text_l2: "scotch.io",
      video_text_l3: "and a",
      video_text_l4: " 15 minute starter YouTube video",
      video_text_p1: "I did a Build Your 1st Guiltywild Site for",
      video_text_p2: "Traversy Media ",
      video_text_p3: "on YouTube also.",
      header_what_learn: "What you'll learn in this course",

      items: [
        {
          message: "What classes should I use?",
        },
        {
          message: "My design looks basic?",
        },
        {
          message: "How do I do responsive?",
        },
        {
          message: "Why does my typography look?",
        },
        {
          message: "Jak moc to vysrat?",
        },
      ],

      paragraphs: [
        {
          message:
            "Tuto hru hraje 10 hráčů, rozdělených do dvou týmů (Dire vs. Radiant) po pěti. Hlavním úkolem je zničit soupeřův Ancient (hlavní budova), který je umístěn v základně jednotlivých týmů. K Ancientu vedou tři cesty (lane), které jsou odděleny lesem (wood/forest/jungle): vrchní (top), střední (mid, middle),spodní (bot, bottom)",
        },

        {
          message:
            "Po cestách chodí skupinky creepů (NPC bojovníci), čtyři melee (bojující na blízko) a jeden ranged (bojující na dálku). Rodí (spawn) se pravidelně u svých kasáren. Také se k nim připojuje i katapult (jednou za čas). Na každé cestě dále najdeme dvě věže, ty nejblíže k nepříteli se označují Tier 1, další Tier 2.",
        },

        {
          message:
            "Poté tu jsou věže Tier 3, které stojí na počátku základny a brání kasárny (barracks, zkráceně rax). Kasárny jsou rozdělené na melee a ranged  Po jejich zničení se na dané lince spawnují nepřátelskému týmu větší a silnější creepové, dle typu zničených raxů. Dále už pak stojí dvě Tier 4 věže",
        },

        {
          message:
            "Pellentesque pretium lectus id turpis. In convallis. Curabitur ligula sapien, pulvinar a vestibulum quis, facilisis vel sapien.",
        },

        {
          message:
            "Curabitur bibendum justo non orci. Fusce tellus. In enim a arcu imperdiet malesuada. Vivamus luctus egestas leo. Duis bibendum, lectus ut viverra rhoncus, dolor nunc faucibus libero, eget facilisis enim ipsum id lacus. Nullam faucibus mi quis velit. Fusce aliquam vestibulum ipsum.",
        },
      ],
    };
  },
};
</script>