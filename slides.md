---
# You can also start simply with 'default'
theme: neversink
neversink_slug: SWC Internal Symposium 2026
# some information about your slides (markdown enabled)
title: SWC Internal Symposium 2026
info: |
  Timothy Sit
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/features/drawing
colorSchema: light
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: fade
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
---

<div class="flex flex-col items-center justify-center text-center gap-0 -mt-5">

  <!-- Image appears second -->
  <img 
    src="/Sky_and_Water_1.jpg" 
    class="w-[100%] object-contain pl-0 mt-0"
  />

  <!-- Title -->
  <h1 class="leading-tight !mt-0">
    Multi-agent decision making in mice, monkeys and humans
  </h1>

  <!-- Subtitle -->
  <div class="text-lg opacity-70">
    Tim Sit | 2026-04-23
  </div>

</div>





---
transition: fade
layout: default
---

# Multi-agent behaviour: strategies and stochasticity


- Some motivation on why study multi-agent behaviour
- not just environment changing, but some internal model of others... 


---
transition: fade
layout: default
---

# Two ways of studying multi-agent behaviour



<div class="grid grid-cols-2 gap-6 mt-10 w-full items-start">

<!-- Column 1 -->
<div v-click="1" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-2xl font-semibold leading-snug max-w-xs">
    Animal vs Computer
  </div>

  <img
    src="/animal-experimenter-interaction.svg"
    class="h-80 object-contain rounded-lg"
  />
</div>

<!-- Column 2 -->
<div v-click="2" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-2xl font-semibold leading-snug max-w-xs">
    Animal vs Animal
  </div>

  <img
    src="/animal-animal-interaction.svg"
    class="h-80 object-contain rounded-lg"
  />
</div>

<!-- Highlight circle -->
<div
  v-click="3"
  class="pointer-events-none absolute left-[5%] top-[15%] w-[45%] h-[75%] border-4 border-red-500 rounded-full"
></div>


</div>


---
transition: fade
layout: default
---

# Strategic stochasticity intro?

<div class="flex flex-col items-center justify-center text-center gap-0">

  <!-- Image appears second -->
  <img 
    v-click="1"
    src="/driver-and-humphries-1970.png" 
    class="w-[35%] object-contain  ml-70"
  />

  <!-- Quote appears first -->
  <div v-click="2" class="max-w-3xl text-lg italic leading-relaxed">
    “Protean behaviour is defined as that behaviour which is sufficiently unsystematic 
    to prevent a reactor predicting in detail the position or actions of the actor.”
    <br/>
    <span class="text-sm not-italic opacity-70">
      Michael Chance(1959), Humphries & Driver (1970)
    </span>
  </div>



</div>


---
transition: fade
layout: default
---

# Multiple species exhibit strategic stochasticity

<div class="grid grid-cols-3 gap-6 w-full items-start">

<!-- Column 1 -->
<div v-click="1" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-sm font-semibold leading-snug max-w-xs">
    Fish increase path complexity after being poked
  </div>

  <img
    src="/pacific-blue-eye.jpg"
    class="h-40 object-contain rounded-lg"
  />
  <img
    src="/blue-eye-fish-entropy.png"
    class="h-40 object-contain rounded-lg"
  />
  <div class="text-xs leading-snug italic max-w-xs">
    Herbert-Read et al. 2015<br>
    <span class="not-italic">
      Escape path complexity and its context dependency in Pacific blue-eyes
    </span>
  </div>
</div>

<!-- Column 2 -->
<div v-click="2" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-sm font-semibold leading-snug max-w-xs">
    Male bird absence duration becomes more unpredictable as their mate approach fertile periods
  </div>

  <img
    src="/kittiwake_adult.jpg"
    class="h-40 object-cover object-top rounded-lg mt--5"
  />
  <img
    src="/richard-wagner-2004.png"
    class="h-40 object-contain rounded-lg"
  />
  <div class="text-xs leading-snug italic max-w-xs">
    Richard Wagner et al. 2004<br>
    <span class="not-italic">
      Is Male Unpredictability a Paternity Assurance Strategy?
    </span>
  </div>
</div>

<!-- Column 3 -->
<div v-click="3" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-sm font-semibold leading-snug max-w-xs">
    Humans can learn to draw random rectangles based on feedback alone
  </div>

  <img
    src="/mondrian.jpg"
    class="h-40 object-contain rounded-lg"
  />
  <img
    src="/ross-and-neuringer-2001.png"
    class="h-40 object-contain rounded-lg"
  />
  <div class="text-xs leading-snug italic max-w-xs">
    Ross and Neuringer 2002<br>
    <span class="not-italic">
      Reinforcement of variations and repetitions along three independent response dimensions
    </span>
  </div>
</div>

</div>


---
transition: fade
layout: default
---


# Studying strategic stochasticity using matching pennies


<div class="relative w-full">

  <img v-click="1" src="/MP_task.png" class="w-full transition-opacity duration-500"
  :class="$clicks >= 2 ? 'opacity-30' : 'opacity-100'" />

  <div v-click="1" class="absolute bottom-4 left-6 text-sm opacity-70">
    Project led by Joanna Aloor
  </div>

  <!-- Monkeys -->
  <div
    v-click="2"
    class="absolute border border-black rounded-sm"
    style="left: 8%; top: 10%; width: 60%;"
  >
    <div class="absolute -top-6 left-0 bg-black/100 text-white text-s px-2 py-0 rounded-sm">
      Monkeys
    </div>
    <img
      src="/lee-2004-cognitive-brain-research.png"
      class="w-full object-contain"
    />
  </div>

  <!-- Rats -->
  <div
    v-click="3"
    class="absolute border border-black rounded-sm"
    style="left: 20%; top: 40%; width: 50%;"
  >
    <div class="absolute -top-6 left-0 bg-black/100 text-white text-s px-2 py-0 rounded-sm">
      Rats
    </div>
    <img
      src="/tervo-cell-2014.png"
      class="w-full object-contain"
    />
  </div>

  <!-- Mice -->
  <div
    v-click="4"
    class="absolute border border-black rounded-sm"
    style="left: 40%; top: 70%; width: 60%;"
  >
    <div class="absolute -top-6 left-0 bg-black/100 text-white text-s px-2 py-0 rounded-sm">
      Mice
    </div>
    <img
      src="/wang-2022-eNeuro.png"
      class="w-full object-contain"
    />
  </div>

</div>





---
transition: fade
layout: default 
---


# Matching pennies experiments


<div class="relative w-full h-[760px]">

<!-- Monkey image -->
<img
  v-click="1"
  src="/monkey-algorithms-cartoon-truncated.svg"
  class="absolute left-1/2 -translate-x-1/2 transition-all duration-700"
  :style="$clicks >= 5
    ? 'top: 0.5rem; width: 55%;'
    : 'top: 3.5rem; width: 70%;'"
/>

<!-- Bullet list -->
<div
  v-if="$clicks >= 2 && $clicks < 5"
  class="absolute left-1/2 top-[250px] -translate-x-1/2 w-[80%]"
>
<ul class="list-disc text-left pl-6 space-y-5">

  <li v-click="2">
    Algorithm 0: coin flip (50/50) for L and R choices
  </li>

  <li v-click="3">
    Algorithm 1: chooses based on stored choice history (sequences of length 4)
  </li>

  <li v-click="4">
    Algorithm 2: chooses based on stored choice and reward history (sequences of length 4) (same as mouse computer opponent)
  </li>

  </ul>
</div>

<!-- Mouse image -->
<img
  v-click="6"
  src="/mouse-against-algorithm-2.svg"
  class="absolute left-1/2 -translate-x-1/2 top-[150px] w-[55%]"
/>

<!-- Human image -->
<img
  v-click="7"
  src="/human-vs-algorithm-2.svg"
  class="absolute left-1/2 -translate-x-1/2 top-[300px] w-[55%]"
/>

</div>


---
transition: fade
---

# Participants learn to do the task


<div class="grid grid-cols-3 gap-6 w-full items-start text-center">

<!-- Mouse -->
<div v-click="1" class="flex flex-col items-center gap-4">
  <img src="/mouse-cartoon.svg" class="w-[50%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    naive and expert example choice
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    entropy and reward rate
  </div>
</div>

<!-- Monkey -->
<div v-click="2" class="flex flex-col items-center gap-4">
  <img src="/monkey.svg" class="w-[62%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    naive and expert example choice
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    entropy and reward rate
  </div>
</div>

<!-- Human -->
<div v-click="3" class="flex flex-col items-center gap-4">
  <img src="/human.svg" class="w-[43%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    naive and expert example choice
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    entropy and reward rate
  </div>
</div>

</div>


---
transition: fade
layout: default 
---


# Disecting behavioural strategies using GLM-HMM



<img src="/GLM-HMM-cartoon_v1.svg" class="opacity-100 w-[50%]" v-click="1"/>

<div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
  Some synthetic data here / example data here
</div>

<div class="absolute bottom-4 left-6 text-sm opacity-70">
GLM-HMM from Ashwoord 2022
</div>


---
transition: fade
---

# Cross-species differences in identified states


<div class="grid grid-cols-3 gap-6 w-full items-start text-center">

<!-- Mouse -->
<div v-click="1" class="flex flex-col items-center gap-4">
  <img src="/mouse-cartoon.svg" class="w-[50%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    GLM-HMM cross validation num states plot
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    State weights
  </div>
</div>

<!-- Monkey -->
<div v-click="2" class="flex flex-col items-center gap-4">
  <img src="/monkey.svg" class="w-[62%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    GLM-HMM cross validation num states plot
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    State weights
  </div>
</div>

<!-- Human -->
<div v-click="3" class="flex flex-col items-center gap-4">
  <img src="/human.svg" class="w-[43%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    GLM-HMM cross validation num states plot
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    State weights
  </div>
</div>

</div>


---
transition: fade
---

# Difference in state-switching dynamics across species


<div class="grid grid-cols-3 gap-6 w-full items-start text-center">

<!-- Mouse -->
<div v-click="1" class="flex flex-col items-center gap-4">
  <img src="/mouse-cartoon.svg" class="w-[50%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    Mouse P(stochastic) increase over time
  </div>
</div>

<!-- Monkey -->
<div v-click="2" class="flex flex-col items-center gap-4">
  <img src="/monkey.svg" class="w-[62%]" />

   <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    Monkey show states corresponding to the three algorithms
  </div>
</div>

<!-- Human -->
<div v-click="3" class="flex flex-col items-center gap-4">
  <img src="/human.svg" class="w-[43%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    Human start with win-stay and then do win-switch
  </div>
</div>

</div>








---
transition: fade
layout: default
---

# Towards animal vs animal multi-agent behaviour



<div class="grid grid-cols-2 gap-6 mt-10 w-full items-start">

<!-- Column 1 -->
<div v-click="1" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-2xl font-semibold leading-snug max-w-xs">
    Animal vs Computer
  </div>

  <img
    src="/animal-experimenter-interaction.svg"
    class="h-80 object-contain rounded-lg"
  />
</div>

<!-- Column 2 -->
<div v-click="1" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-2xl font-semibold leading-snug max-w-xs">
    Animal vs Animal
  </div>

  <img
    src="/animal-animal-interaction.svg"
    class="h-80 object-contain rounded-lg"
  />
</div>

<!-- Highlight circle -->
<div
  v-click="2"
  class="pointer-events-none absolute left-[50%] top-[15%] w-[45%] h-[75%] border-4 border-red-500 rounded-full"
></div>


</div>

---
transition: fade
layout: default
---

# Animal vs Animal Matching pennies

<video 
  id="myvid"
  src="/example_multiplayer_synced_video.mp4"
  controls
  class="w-1/2 mx-auto -mt-5"
/>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const vid = document.getElementById('myvid')
  if (vid) {
    vid.playbackRate = 2.0   // 0.5 = half speed, 2.0 = double speed
  }
})
</script>



---
transition: fade
layout: default
---

# Animal vs Animal Matching pennies behaviour


<div class="grid grid-cols-2 gap-6 w-full items-start text-center">

<!-- Mouse -->
<div v-click="1" class="flex flex-col items-center gap-4">
  <img src="/mouse-cartoon.svg" class="w-[25%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    Some example choices 
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    Some quantification of whether they are adapating to opponent / LR model fits
  </div>
</div>

<!-- Human -->
<div v-click="2" class="flex flex-col items-center gap-4">
  <img src="/human.svg" class="w-[22%]" />

  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    Some example choices 
  </div>
  <div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
    Some quantification of whether they are adapating to opponent / LR model fits
  </div>
</div>

</div>



---
transition: fade
layout: default
---

# Animal vs Animal Matching pennies : outlook 



<div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
  Schematic of looking at training history (2AB vs 2AB and 2AB vs MP mice)
</div>

<div class="w-full border-2 border-dashed border-gray-400 rounded-lg py-6 text-sm opacity-70">
  Maybe some preliminary data with 2AB vs 2AB mice choices to show it does do something
</div>



---
layout: side-title
color: teal 
transition: fade
---

:: title :: 

# Conclusion 

:: content ::

<div style="transform: translateY(6vh)">

<v-clicks :every="2">

<p class="text-lg font-semibold italic text-teal-600">How do different animals learn strategic stochasticity?</p>
<p class="text-base text-gray-700 mb-4 ml-4">...</p>

<p class="text-lg font-semibold italic text-teal-600">What are the difference in states and their dynamics?</p>
<p class="text-base text-gray-700 mb-4 ml-4">...</p>

<p class="text-lg font-semibold italic text-teal-600">Do we observed a change in behaviour when switching from playing against a computer to player against a conspecific?</p>
<p class="text-base text-gray-700 ml-4">...</p>

</v-clicks>

</div>




---
layout: credits 
color: light 
speed: 1
loop: true
---

<div class="grid text-size-4 grid-cols-3 w-3/4 gap-y-10 auto-rows-min ml-auto mr-auto">
<div class="grid-item text-center mr-0- col-span-3">
  
</div>
<div class="grid-item text-center mr-0- col-span-3">
  <strong>Cast</strong><br> 
  <span class="font-size-3 mt-0">(In order of appearance)</span>
</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Mouse MP</strong></div>
<div class="grid-item col-span-2">Joanna&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Monkey MP</strong></div>
<div class="grid-item col-span-2">Dae-yeol Lee <br/> Monkeys C, E, F&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Human MP</strong></div>
<div class="grid-item col-span-2">Julia Nicklaus&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Widefield</strong></div>
<div class="grid-item col-span-2">Joanna&nbsp;&nbsp;</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Mice</strong></div>
<div class="grid-item col-span-2">JOA-M-0008<br/>JOA-M-0009<br/>JOA-M-0010<br/>JOA-M-0013<br/>JOA-M-0014<br/>JOA-M-0015<br/>JOA-M-0016<br/>...<br/></div>


<div class="grid-item text-right mr-4 col-span-1"><strong>Humans</strong></div>
<div class="grid-item col-span-2">Orsi <br/> Margot <br/> Chen Chen <br/> Joschua <br/> ... &nbsp;</div>

<div class="grid-item text-right mr-4 col-span-1"><strong>Supervision</strong></div>
<div class="grid-item col-span-2">Ann</div>
<div class="grid-item col-span-3 text-center mt-80px mb-auto font-size-1.5rem"><strong>The end</strong></div>
</div>
