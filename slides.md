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
    Multi-agent decision-making in mice, monkeys and humans
  </h1>

  <!-- Subtitle -->
  <div class="text-lg opacity-70">
    Tim Sit | Duan Lab | 2026-04-23
  </div>

</div>



---
transition: fade
layout: default
clicks: 6
---

# Think of decision-making as games and agents

<div class="grid grid-cols-3 gap-8 w-full mt-2 items-start">

  <!-- Top gradient: increasing left -> right -->
  <div class="absolute top-20 left-0 w-full h-8 pointer-events-none z-0">
    <div class="absolute inset-0 bg-gradient-to-r from-gray-100 via-gray-300 to-gray-600 opacity-40 clip-agent-top"></div>
    <div class="absolute right-2 -top-10 text-2xl font-medium">
      Interactiveness
    </div>
  </div>

  <!-- Bottom gradient: decreasing left -> right -->
  <div class="absolute top-60 left-0 w-full h-8 pointer-events-none z-0">
    <div class="absolute inset-0 bg-gradient-to-r from-gray-600 via-gray-300 to-gray-100 opacity-70 clip-agent-bottom"></div>
    <div class="absolute left-2 top-0 text-2xl font-medium">
      Experimental control
    </div>
  </div>


  <!-- Column 1 -->
  <div class="flex flex-col items-center text-center">
    <div
      v-if="$clicks >= 1"
      class="text-2xl font-semibold mb-4"
    >
      Slot Machine
    </div>

  <img
    v-if="$clicks >= 1"
    src="/slow-machine-v2.png"
    class="w-full max-w-[85%] object-contain -mt-10"
  />

  <!-- Extra slot-machine details only on click 2 -->
  <div
    v-if="$clicks >= 2"
    class="mt-6 flex flex-col items-center"
  >
    <img
      src="/oli-task-schematic.png"
      class="w-full max-w-[100%] object-contain mb-4 -mt-5"
    />

  </div>

  <div
    v-if="$clicks >= 2"
    class="mt-0 text-sm italic leading-snug max-w-[90%]"
  >
  <div class="flex items-center justify-center gap-4 mb-3 -mt-3">
  <img
    src="/oli-head.jpg"
    class="w-14 h-14 rounded-full object-cover border border-gray-300"
  /> 
  <img
    src="/chaofei-head.png"
    class="w-14 h-14 rounded-full object-cover border border-gray-300"
  />
   <img
    src="/jingjie-head.png"
    class="w-14 h-14 rounded-full object-cover border border-gray-300"
  />
  </div>
  <div class="flex items-center justify-center gap-4 mb-3 -mt-4">
  <img
    src="/nikos-head.jpg"
    class="w-14 h-14 rounded-full object-cover border border-gray-300"
  />
   <img
    src="/yang-head.jpg"
    class="w-14 h-14 rounded-full object-cover border border-gray-300"
  />
  </div>

  Gauld* &amp; Bao* et al. 2026<br>
  <span class="not-italic">
    A frontal motor circuit for economic decisions and actions
  </span>
  (bioRxiv)
  </div>


  </div>

  <!-- Column 2 placeholder until click 4 -->
  <div class="flex flex-col items-center text-center">

  <template v-if="$clicks >= 5">
    <div class="text-2xl font-semibold mb-4">
      Rock paper scissors
    </div>
    <img
      src="/mouse-rock-paper-scissors.png"
      class="w-full max-w-[85%] object-contain -mt-5"
    />
  </template>
  <div
      v-if="$clicks >= 6"
      class="mt-0 text-sm italic leading-snug max-w-[90%]"
    >
  <div class="flex items-center justify-center gap-4 mb-3 mt-5">
    <img
      src="/joanna-head.png"
      class="w-14 h-14 rounded-full object-cover border border-gray-300"
    /> 
    <img
      src="/tim-head.jpg"
      class="w-14 h-14 rounded-full object-cover border border-gray-300"
    />
  </div> <br>
<!-- Julia + hiring placeholder -->
  <div class="flex items-center justify-center gap-4 mb-3 -mt-5">
    <img
      src="/julia-head.jpg"
      class="w-14 h-14 rounded-full object-cover border border-gray-300 aspect-square shrink-0 overflow-hidden"
    />

  <div class="w-14 h-14 rounded-full border-2 border-dashed border-gray-500 flex items-center justify-center text-base font-semibold not-italic bg-white text-gray-700 aspect-square shrink-0">
    You? RA
  </div>

  <span class="not-italic">This talk!</span>
  </div>

  Aloor* &amp; Sit* et al. 2026<br>
  <span class="not-italic">
    Strategic stochasticity in mice and monkeys (in prep)
  </span> <br>
  <span class="not-italic">
  Distinct neuromodulatory contributions to strategic decisions in a competitive multi-player game (in prep)
  </span>
  </div>
  </div>

  <!-- Column 3 -->
  <div class="flex flex-col items-center text-center">
    <template v-if="$clicks >= 3">
      <div class="text-2xl font-semibold mb-4">
        Foraging competition
      </div>
      <img
        src="/mouse-racing-towards-a-cheese.png"
        class="w-full max-w-[85%] object-contain -mt-5"
      />
    </template>
    <div
      v-if="$clicks >= 4"
      class="mt-0 text-sm italic leading-snug max-w-[90%]"
    >
    <div class="flex items-center justify-center gap-4 mb-3 mt-4">
    <img
      src="/octagon-task-schematic.png"
      class="w-full max-w-[50%] object-contain mb-4 mt-0"
    />
  <!-- Headshots in 3 rows -->
  <div class="grid grid-cols-2 gap-0 justify-items-center -mt-1 relative z-10">
    <div class="w-14 h-14 rounded-full overflow-hidden border border-gray-300 shrink-0">
    <img
      src="/mehul-head.png"
      class="w-full h-full object-cover scale-100"
    />
  </div>
  <div class="w-14 h-14 rounded-full overflow-hidden border border-gray-300 shrink-0">
    <img
      src="/ivana-head.jpg"
      class="w-full h-full object-cover scale-100"
    />
  </div>
  <div class="w-14 h-14 rounded-full overflow-hidden border border-gray-300 shrink-0">
    <img
      src="/chris-head.png"
      class="w-full h-full object-cover scale-100"
    />
  </div>
    <div class="w-14 h-14 rounded-full overflow-hidden border border-gray-300 shrink-0">
    <img
      src="/orsi-head.png"
      class="w-full h-full object-cover scale-100"
    />
  </div>
  <!-- Last row (centered single image) -->
  <div class="col-span-2 flex justify-center">
    <img src="/roshni-head.jpg" class="w-14 h-14 rounded-full object-cover border border-gray-300" />
    <img src="/tom-head.png" class="w-14 h-14 rounded-full object-cover border border-gray-300" />
    <img src="/bene-head.jpg" class="w-14 h-14 rounded-full object-cover border border-gray-300" />
  </div>
  </div>
  </div>

  Erlich, Ristogi ... Orsolic et al. 2026<br>
  <span class="not-italic">
    Mice dynamically adapt to opponents in competitive multi-player games
  </span>
  (bioRxiv)
  </div>

  </div>

</div>

---
transition: fade
layout: default
clicks: 6
---

<h1 class="!text-[1.7rem] !leading-tight">

Rock paper scissors as a way of studying strategic stochasticity

</h1>

<div class="relative w-full h-[560px] mt-1">

  <!-- STEP 3: interim title -->
  <div
    v-if="$clicks >= 3"
    class="absolute -top-2 left-15% -translate-x-1/2 text-xl font-semibold text-center transition-all duration-700"
  >
    Rock paper scissors requires <br> strategic stochasticity
  </div>

  <!-- STEP 4+: final heading for columns -->
  <div
    v-if="$clicks >= 4"
    class="absolute top-8 left-[38%] w-[58%] -mt-10 text-center text-xl font-semibold transition-all duration-700"
  >
    Strategic stochasticity exists in <br> nature and across species
  </div>

  <!-- LEFT / CENTRE cartoon block -->
  <div
    class="absolute transition-all duration-700"
    :class="$clicks < 3
      ? 'top-[60px] left-1/2 -translate-x-1/2 w-[42%]'
      : 'top-[90px] left-[2%] w-[28%]'"
  >
    <!-- First cartoon -->
    <div
      v-if="$clicks === 1"
      class="flex flex-col items-center text-center"
    >
      <img
        src="/mouse-thinking-mouse.png"
        class="w-full max-w-[280px] object-contain"
      />
      <div class="mt-4 text-lg italic text-gray-700 max-w-md">
        “I need to predict what the opponent will play next.”
      </div>
    </div>

  <!-- Second cartoon -->
  <div
    v-if="$clicks >= 2"
    class="flex flex-col items-center text-center"
  >
    <img
      src="/mouse-thinking-mouse-thinking-mouse.png"
      class="w-full max-w-[280px] object-contain"
    />
    <div class="mt-4 text-lg italic text-gray-700 max-w-md">
      “My opponent is predicting my next move, I should randomise to be unpredictable.”
    </div>
  </div>
  </div>

  <!-- MIDDLE COLUMN -->
  <div
    v-if="$clicks >= 5"
    class="absolute top-[50px] left-[38%] w-[26%] flex flex-col items-center text-center transition-all duration-700"
  >
    <div class="text-sm font-semibold leading-snug max-w-xs mb-3">
      Random escape trajectories in prey animals
    </div>

  <img
    src="/driver-and-humphries-1970.png"
    class="w-full max-w-[100%] object-contain rounded-lg"
  />

  <div class="text-xs leading-snug italic max-w-xs mt-3">
    Humphries and Driver 1970<br>
    <span class="not-italic">
      Protean defence by prey animals
    </span>
  </div>
  </div>

  <!-- RIGHT COLUMN -->
  <div
    v-if="$clicks >= 6"
    class="absolute top-[50px] right-[2%] w-[26%] flex flex-col items-center text-center transition-all duration-700"
  >
    <div class="text-sm font-semibold leading-snug max-w-xs mb-3">
      Fish increase path complexity after being poked
    </div>

  <div class="flex flex-col items-center gap-3">
    <img
      src="/pacific-blue-eye.jpg"
      class="h-32 object-contain rounded-lg"
    />
    <img
      src="/blue-eye-fish-entropy.png"
      class="h-32 object-contain rounded-lg"
    />
  </div>

  <div class="text-xs leading-snug italic max-w-xs mt-3">
    Herbert-Read et al. 2015<br>
    <span class="not-italic">
      Escape path complexity and its context dependency in Pacific blue-eyes
    </span>
  </div>
  </div>

</div>

---
transition: fade
layout: two-cols-title
clicks: 13
---

:: title :: 

# Matching pennies:  a simplified game of rock paper scissors

:: left :: 

<div class="w-full">
  <img
    v-if="$clicks < 4"
    src="/symmetric_matching_pennies_0.png"
    class="opacity-100 w-[100%]"
  />
  <img
    v-else-if="$clicks < 5"
    src="/symmetric_matching_pennies_1.png"
    class="opacity-100 w-[100%]"
  />
  <img
    v-else
    src="/symmetric_matching_pennies_2.png"
    class="opacity-100 w-[100%]"
  />
</div>

:: right :: 

<div class="leading-tight space-y-3">

  <v-click at="1">
    <div class="font-semibold">Game logic:</div>
  </v-click>

  <v-click at="2">
    <div class="ml-4">• Simultaneous binary choice</div>
  </v-click>

  <v-click at="3">
    <div class="ml-4">• <i>Matcher</i> wins if same, unmatcher wins if different</div>
  </v-click>

  <v-click at="6">
    <div class="font-semibold pt-2">Strategies:</div>
  </v-click>

  <v-click at="7">
    <div class="ml-4">• Exploit predictable opponents</div>
  </v-click>

  <v-click at="8">
    <div class="ml-4">• Be unpredictable to avoid exploitation</div>
  </v-click>

  <v-click at="9">
    <div class="font-semibold pt-2">Potential game dynamics:</div>
  </v-click>

  <v-click at="10">
    <div class="ml-4">• Nash equilibrium: both players randomise 50/50, with reward rate of 50%</div>
  </v-click>

  <v-click at="11">
    <div class="ml-4">• A player learns to exploit an opponent</div>
  </v-click>

  <v-click at="12">
    <div class="ml-4">• A player learns randomness under competition from a predictive opponent</div>
  </v-click>

</div>

<!-- Centered overlay: Talk overview -->
<div
  v-if="$clicks === 13"
  class="absolute inset-0 flex items-center justify-center z-20"
>

  <!-- content -->
  <div class="relative bg-white rounded-2xl border-5 border-gray-300 shadow-xl p-6 w-[60%] max-w-[900px] text-center">
    
  <div class="text-xl font-semibold mb-4 text-gray-800">
    Talk overview
  </div>


  <img
    src="/overview-cartoon.svg"
    class="w-full object-contain"
  />


  </div>
</div>

---
transition: fade
layout: side-title
clicks: 5
---

:: title :: 

# Scientific questions


<!-- Left: overview cartoon -->
<div class="relative w-full">
  <div class="rounded-xl border border-gray-300 bg-white p-3 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Highlight left half for question 1 -->
  <div
    v-if="$clicks === 1"
    class="absolute inset-y-0 left-0 w-63% border-4 border-blue-500 rounded-l-lg pointer-events-none"
  ></div>

  <!-- Highlight right half for question 3 -->
  <div
    v-if="$clicks === 3"
    class="absolute inset-y-0 right-0 w-37% border-4 border-red-500 rounded-r-lg pointer-events-none"
  ></div>

  <!-- Optional de-emphasis of the non-highlighted half -->
  <div
    v-if="$clicks === 1"
    class="absolute inset-y-0 right-0 w-37% bg-white/55 pointer-events-none"
  ></div>

  <div
    v-if="$clicks === 3"
    class="absolute inset-y-0 left-0 w-63% bg-white/55 pointer-events-none"
  ></div>
  </div>

  <!-- Highlight left half for question 1 -->
  <div
    v-if="$clicks === 4"
    class="absolute inset-y-0 left-0 w-63% border-4 border-blue-500 rounded-l-lg pointer-events-none"
  ></div>

  <!-- Optional de-emphasis of the non-highlighted half -->
  <div
    v-if="$clicks === 4"
    class="absolute inset-y-0 right-0 w-37% bg-white/55 pointer-events-none"
  ></div>


</div>



:: content :: 




<div class="space-y-6 mt-10">

  <v-click>

  <div :class="$clicks >= 4 ? 'opacity-100' : ''">
    <div 
      class="text-lg transition-all duration-500"
      :class="$clicks >= 4 ? 'text-black-500 font-semibold' : ''"
    >
      1. What are the behavioural strategies used by mice in a game of matching pennies against an opponent with a stationary strategy? How does it differ between humans and monkeys?
    </div>
    <div class="text-sm italic mt-1 ml-4 transition-all duration-500"
         :class="$clicks >= 4 ? 'opacity-90' : 'opacity-70'">
      Aloor, Sit et al. *Strategic stochasticity in mice and monkeys* (in prep)
    </div>
  </div>

  </v-click>

  <v-click>

  <div :class="$clicks >= 4 ? 'opacity-30' : ''">
    <div class="text-lg transition-all duration-500">
      2. Can we find neural signatures of different behavioural strategies, such as differences in reward signalling?
    </div>
    <div class="text-sm italic opacity-70 mt-1 ml-4">
      Aloor, Sit et al. *Distinct neuromodulatory contributions to strategic decisions in a competitive multi-player game* (in prep)
    </div>
  </div>

  </v-click>

  <v-click>

  <div :class="$clicks >= 4 ? 'opacity-100' : ''">
    <div class="text-lg transition-all duration-500">
      3. Do mice and humans change their strategy when playing against a conspecific, where the strategies of the opponent is no longer stationary?
    </div>
    <div class="text-sm italic opacity-70 mt-1 ml-4">
      Ongoing project
    </div>
  </div>

  </v-click>

</div>

---
transition: fade
layout: default
---

# Matching pennies experiments across species



<div class="relative w-full h-[760px]">

<!-- Monkey image -->
<img
  v-click="1"
  src="/monkey-algorithms-cartoon-v3.svg"
  class="absolute left-55% -translate-x-1/2 transition-all duration-700 -mt-10"
  :style="$clicks >= 5
    ? 'top: 0rem; width: 55%;'
    : 'top: 1.5rem; width: 80%;'"
/>

<!-- Bullet list -->
<div
  v-if="$clicks >= 2 && $clicks < 5"
  class="absolute left-1/2 top-[200px] -translate-x-1/2 w-[80%]"
>
<ul class="list-disc text-left pl-6 space-y-2">

  <li v-click="2">
    Algorithm 0: coin flip (50/50) for L and R choices
  </li>

  <li v-click="3">
    Algorithm 1: chooses based on stored choice history <br> (sequences of length 1- 4)
  </li>

  <li v-click="4">
    Algorithm 2: chooses based on stored choice and reward history <br> (sequences of length 1 - 4)
  </li>

  </ul>
</div>

<!-- Mouse image -->
<img
  v-click="6"
  src="/mouse-against-algorithm-2-v2.svg"
  class="absolute left-54% top-16% w-[32%]"
/>

<!-- Mouse justification -->
<div
  v-if="$clicks >= 6"
  class="absolute left-[15%] top-[25%] -translate-y-1/2 w-[35%]"
>
  <div class="px-4 py-3 rounded-lg bg-white/70 backdrop-blur-md shadow-md">
    <div class="text-base font-semibold mb-2">
      Why study mice?
    </div>
    <ul class="list-disc pl-5 space-y-1 text-sm">
      <li>Higher throughput experiments, study of individual differences</li>
      <li>Simultaneous large-scale neural recordings</li>
      <li>Genetic and circuit manipulation tools</li>
    </ul>
  </div>
</div>

<!-- Human image -->
<img
  v-click="7"
  src="/human-vs-algorithm-2-v2.svg"
  class="absolute left-54% top-37% w-[32%]"
/>

<!-- Human justification -->
<div
  v-if="$clicks >= 7"
  class="absolute left-[15%] top-[50%] -translate-y-1/2 w-[35%]"
>
  <div class="px-4 py-3 rounded-lg bg-white/70 backdrop-blur-md shadow-md">
    <div class="text-base font-semibold mb-2">
      Why study humans?
    </div>
    <ul class="list-disc pl-5 space-y-1 text-sm">
      <li>Cross-species comparison</li>
      <li>More flexible, sophisticated strategies</li>
    </ul>
  </div>
</div>



</div>


<!-- Daeyeol Lee headshot + citation -->
<div
  v-if="$clicks >= 1 && $clicks < 5"
  class="absolute bottom-10 left-1/2 -translate-x-1/2 flex flex-col items-center"
>
<!-- Circular image -->
<img
  src="/daeyeol-lee.jpg"
  class="w-16 h-16 rounded-full object-cover border border-gray-300 shadow-md -ml-125"
/>

<!-- Citation -->
<div class="text-xs text-center -mt-10 max-w-md leading-snug opacity-80">
  <i>Lee et al., 2004. </i> Reinforcement learning and decision making in monkeys during a competitive game. <i>Cognitive Brain Research</i> 
</div>

</div>

<!-- Bottom-left overview panel -->
<div
  class="absolute left-[3%] bottom-[3%] w-[18%]"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize left half -->
  <div
    v-if="$clicks < 6"
    class="absolute inset-y-0 left-0 w-30% border-2 border-blue-500 rounded-l-lg pointer-events-none"
  ></div>

  <!-- Optional de-emphasis -->
  <div
    v-if="$clicks < 6"
    class="absolute inset-y-0 right-0 w-70% bg-white/45 pointer-events-none"
  ></div>

  <!-- Emphasize left half -->
  <div
    v-if="$clicks === 6"
    class="absolute inset-y-0 left-0 w-46% border-2 border-blue-500 rounded-l-lg pointer-events-none"
  ></div>

  <!-- Optional de-emphasis -->
  <div
    v-if="$clicks === 6"
    class="absolute inset-y-0 right-0 w-54% bg-white/45 pointer-events-none"
  ></div>

  <!-- Emphasize left half -->
  <div
    v-if="$clicks >= 7"
    class="absolute inset-y-0 left-0 w-63% border-2 border-blue-500 rounded-l-lg pointer-events-none"
  ></div>

  <!-- Optional de-emphasis -->
  <div
     v-if="$clicks >= 7"
    class="absolute inset-y-0 right-0 w-37% bg-white/45 pointer-events-none"
  ></div>

  </div>
</div>





---
transition: fade
layout: two-cols-title 
columns: is-5
---

:: title :: 


<h1 class="!text-[1.6rem] !leading-tight">
  Unsupervised discovery of behavioural strategies using GLM-HMM
</h1>

:: left :: 

## Model


<img src="/GLM-HMM-cartoon_v1.svg" class="opacity-100 w-[100%]" v-click="1"/>


:: right :: 

## Verification with synthetic data 


<img src="/recovered_glm_weights_4_states_1.svg" class="opacity-100 w-[100%]" v-click="2"/>


<img src="/p_state_4_states.svg" class="opacity-100 w-[100%]" v-click="3"/>


<div v-click="1" class="absolute bottom-10 left-12 w-[36%] text-sm opacity-75 leading-snug">
  <hr class="border-t border-gray-600 opacity-20 mb-2" />

  <div>
    <i>Ashwood et al. 2022. </i>Mice alternate between discrete strategies during perceptual decision-making. <i>Nature Neuroscience </i>
  </div>

  <div class="mt-2">
    <i> Bolkan  et al. 2022. </i> Opponent control of behaviour by dorsomedial striatal pathways depends on task demands and internal state. <i>Nature Neuroscience </i>
  </div>
</div>


---
transition: fade
layout: default
clicks: 6
---

<h1 class="!text-[1.4rem] !leading-tight">
Monkeys adapt their strategy to the competitive pressure from their opponent
</h1>

<div class="w-full flex justify-center">
  <div class="relative w-full h-[760px] overflow-hidden">

  <!-- Cartoon -->
  <img
    src="/monkey-algorithms-cartoon-v4.svg"
    class="absolute left-[61%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks === 1
      ? 'top: 90px; width: 95%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 2
      ? 'top: 5%; width: 80%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 3
      ? 'top: 0%; width: 80%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 58%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- Example choices -->
  <img
    src="/monkey_E_example_choices_per_algorithm.svg"
    class="absolute left-[50%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 2
      ? 'top: 35%; width: 52%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 2
      ? 'top: 30%; width: 70%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 3
      ? 'top: 24%; width: 70%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 4
      ? 'top: 40px; width: 70%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 52%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

   <!-- Reward rate per algorithm -->
  <img
    src="/monkey_reward_rate_per_algorithm.svg"
    class="absolute left-[55%] -translate-x-1/2 transition-all duration-700 ease-in-out z-2"
    :style="$clicks < 3
      ? 'top: 55%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 3
      ? 'top: 43%; width: 90%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 50%; width: 55%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- State weights -->
  <img
    src="/monkey_state_weights_colored.svg"
    class="absolute left-[49%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 4
      ? 'top: 24%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 4
      ? 'top: 24%; width: 80%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 2%; width: 60%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  <!-- Per-session summary -->
  <img
    src="/monkey_state_per_session_summary.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 5
      ? 'top: 30%; width: 80%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : 'top: 30%; width: 80%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  </div>
</div>


<!-- Algorithm labels -->
<div v-if="$clicks === 4" class="absolute inset-0 pointer-events-none">

  <!-- Algorithm 0 -->
  <div class="absolute top-[15%] left-[27%] text-[1.1rem] font-semibold text-[#2ca6a4ff]">
    Algorithm 0
  </div>

  <!-- Algorithm 1 -->
  <div class="absolute top-[15%] left-[48%] text-[1.1rem] font-semibold text-[#e3b505ff]">
    Algorithm 1
  </div>

  <!-- Algorithm 2 -->
  <div class="absolute top-[15%] left-[67%] text-[1.1rem] font-semibold text-[#4f6db8ff]">
    Algorithm 2
  </div>

</div>


<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[2%] w-[14%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize left half -->
  <div
    class="absolute inset-y-0 left-0 w-30% border-2 border-blue-500 rounded-l-lg pointer-events-none"
  ></div>

  <!-- Optional de-emphasis -->
  <div
    class="absolute inset-y-0 right-0 w-70% bg-white/45 pointer-events-none"
  ></div>

  </div>

</div>


---
transition: fade
clicks: 5
---


# Mice alternate between bias and stochastic states

<div class="w-full flex justify-center">
  <div class="relative w-full h-[760px] overflow-hidden">

  <!-- Cartoon -->
  <img
    src="/mouse-against-algorithm-2-v2.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks === 1
      ? 'top: 0%; width: 36%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks <= 3
      ? 'top: 0%; width: 36%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 36%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- Purple note -->
  <div
    v-click="1"
    class="absolute top-[6%] right-[4%] max-w-[26%] 
          bg-purple-100 border border-purple-300 
          rounded-xl px-4 py-3 shadow-sm
          transition-all duration-700"
    :style="$clicks <= 3
      ? 'opacity: 1; transform: translateY(0);'
      : 'opacity: 0; transform: translateY(-10px);'"
  >
    <div class="text-purple-800 font-semibold text-sm mb-1">
      Why only algorithm 2?
    </div>
    <div class="text-purple-900 text-sm leading-snug">
      Allows for tracking changes in strategy over learning against the same opponent
    </div>
  </div>

  <!-- Example choices -->
  <img
    src="/example_mouse_naive_to_expert_horizontal.svg"
    class="absolute left-[48%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 2
      ? 'top: 35%; width: 68%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 2
      ? 'top: 20%; width: 68%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 3
      ? 'top: 20%; width: 68%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 4
      ? 'top: 2%; width: 68%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 2%; width: 68%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- Reward rate -->
  <img
    src="/mouse_reward_rate_over_sessions.svg"
    class="absolute left-[46%] -translate-x-1/2 transition-all duration-700 ease-in-out z-[2]"
    :style="$clicks < 3
      ? 'top: 55%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 3
      ? 'top: 43%; width: 62%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 48%; width: 62%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- GLM-HMM weights -->
  <img
    src="/glmhmm_glm_weights (1).png"
    class="absolute left-[48%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 4
      ? 'top: 60%; width: 70%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 4
      ? 'top: 30%; width: 68%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 4%; width: 68%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  <!-- Learning summary -->
  <img
    src="/average_pstate_smooth_cosyneabstract2025.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 5
      ? 'top: 50%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : 'top: 30%; width: 50%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  </div>
</div>


<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[2%] w-[18%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize -->
  <div
    class="absolute inset-y-0 left-12 w-20% border-2 border-blue-500 rounded-lg-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 right-0 w-52% bg-white/45 pointer-events-none"
  ></div>

  </div>

</div>




---
transition: fade
layout: default
clicks: 5
---

# Humans alternate between win-stay and win-switch states

<div class="w-full flex justify-center">
  <div class="relative w-full h-[760px] overflow-hidden">

  <!-- Human image -->
  <img
    src="/human-vs-algorithm-2-v2.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks === 1
      ? 'top: 90px; width: 34%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks <= 3
      ? 'top: 5%; width: 26%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 26%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- Purple note -->
  <div
    v-click="1"
    class="absolute top-[17%] right-[4%] max-w-[26%] 
          bg-purple-100 border border-purple-300 
          rounded-xl px-4 py-3 shadow-sm
          transition-all duration-700"
    :style="$clicks <= 1
      ? 'opacity: 1; transform: translateY(0);'
      : 'opacity: 0; transform: translateY(-10px);'"
  >
    <div class="text-purple-800 font-semibold text-sm mb-1">
      Single session experiments
    </div>
    <div class="text-purple-900 text-sm leading-snug">
      Compared to mice and monkeys, we expect faster learning from humans
    </div>
  </div>


  <!-- Example choices: smooth zoom-out from cropped to full -->
  <div
    class="absolute left-[48%] -translate-x-1/2 overflow-hidden rounded-lg transition-all duration-700 ease-in-out"
    :style="$clicks < 2
      ? 'top: 35%; width: 58%; height: 180px; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 2
      ? 'top: 20%; width: 38%; height: 50%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 3
      ? 'top: 25%; width: 58%; height: 260px; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 4
      ? 'top: 40px; width: 58%; height: 260px; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 58%; height: 260px; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  >
    <img
      src="/example_human_choices.svg"
      class="absolute transition-all duration-700 ease-in-out"
      :style="$clicks < 2
        ? 'max-width: none; width: 360%; left: -115%; top: 0%;'
        : $clicks === 2
        ? 'max-width: none; width: 360%; left: -115%; top: 0%;'
        : $clicks === 3
        ? 'max-width: none; width: 100%; left: 0%; top: 0%;'
        : $clicks === 4
        ? 'max-width: none; width: 100%; left: 0%; top: 0%;'
        : 'max-width: none; width: 100%; left: 0%; top: 0%;'"
    />
  </div>

  <!-- State weights -->
  <img
    src="/human_solo_mp_states.svg"
    class="absolute left-[47%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 4
      ? 'top: 26%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 4
      ? 'top: 22%; width: 60%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 44%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  <!-- Per-session summary -->
  <img
    src="/human_pstate_over_session.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 5
      ? 'top: 30%; width: 80%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : 'top: 25%; width: 80%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  </div>
</div>


<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[2%] w-[18%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize -->
  <div
    class="absolute inset-y-0 left-19.5 w-19% border-2 border-blue-500 rounded-lg-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 right-0 w-35% bg-white/45 pointer-events-none"
  ></div>

  </div>

</div>



---
transition: fade
layout: side-title
clicks: 4
---

:: title ::

# Interim summary 

:: content :: 
<div class="mt-25">

<v-clicks>

1. GLM-HMM captures changes in the monkey's strategy in response to changes in the computer opponent, and succesfully learns randomise in response to a predictive computer opponent 
2. Mice also learn to randomise, going from biased states to stochastic states
3. Humans tend to start with win-stay strategies followed by a mix of win-stay and win-switch strategies

</v-clicks>

</div>

<v-click>

**To what extent do each species manage to show random choice patterns?**

</v-click>

---
transition: fade
clicks: 5
---

<h1 class="!text-[1.5orem] !leading-tight">

To what extent do each species manage to show random choice patterns?

</h1>

<div class="-mt-2">

<img
    src="/all-three-species-vs-algorithm-2.svg"
    class="w-full max-w-[40%] ml-60 object-contain"
  />

<div class="grid grid-cols-3 gap-0 w-full mt-0 items-start">

  <!-- Column 1 -->
  <div v-click="1" class="flex flex-col items-center text-center">
    <div class="text-lg font-semibold leading-snug mb-4">
      Monkeys stay in the stochastic state consistently
    </div>
    <img
      src="/mouse_monkey_inverted_U_shape_p_stochastic_v3.svg"
      class="w-full max-w-[100%] object-contain"
    />
  </div>

  <!-- Column 2 -->
  <div v-click="2" class="flex flex-col items-center text-center">
    <div class="text-lg font-semibold leading-snug mb-4">
      Entropy correlates with P(stochastic)
    </div>
    <img
      src="/mouse_monkey_pstochastic_and_entropy.svg"
      class="w-full max-w-[70%] object-contain"
    />
  </div>

  <!-- Column 3, click 3 -->
  <div
    v-if="$clicks === 3"
    class="flex flex-col items-center text-center"
  >
    <div class="text-lg font-semibold leading-snug mb-4">
      Monkeys show higher entropy during stochastic state
    </div>
    <img
      src="/segment_length_vs_entropy_zoomed_in.svg"
      class="w-full max-w-[70%] object-contain"
    />
  </div>

  <!-- Column 3, click 4 -->
  <div
    v-if="$clicks === 4"
    class="flex flex-col items-center text-center"
  >
    <div class="text-lg font-semibold leading-snug mb-4">
      Monkeys show higher entropy during stochastic state
    </div>
    <img
      src="/segment_length_vs_entropy_zoomed_in_w_human.svg"
      class="w-full max-w-[70%] object-contain"
    />
  </div>

  <!-- Column 3, click 5 -->
  <div
    v-if="$clicks >= 5"
    class="flex flex-col items-center text-center"
  >
    <div class="text-lg font-semibold leading-snug mb-4">
      But reward rates are similar
    </div>
    <img
      src="/three_species_entropy_and_reward_rate.svg"
      class="w-full max-w-[85%] object-contain"
    />
  </div>

</div>

</div>


<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[1%] w-[18%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize -->
  <div
    class="absolute inset-y-0 left-0 w-63% border-2 border-blue-500 rounded-lg-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 right-0 w-35% bg-white/45 pointer-events-none"
  ></div>

  </div>

</div>



---
transition: fade
layout: side-title
clicks: 5
---

:: title :: 

# Part I Summary

<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[25%] w-[30%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />


  <!-- Emphasize -->
  <div
    v-if="$clicks === 2"
    class="absolute inset-y-0 left-20 w-19% border-3 border-blue-500 rounded-lg-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    v-if="$clicks === 2"
    class="absolute inset-y-0 right-0 w-52% bg-white/45 pointer-events-none"
  ></div>


  <!-- Emphasize -->
  <div
    v-if="$clicks === 3"
    class="absolute inset-y-0 left-0 w-28% border-3 border-blue-500 rounded-l-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    v-if="$clicks === 3"
    class="absolute inset-y-0 right-0 w-52% bg-white/45 pointer-events-none"
  ></div>


  <!-- Emphasize -->
  <div
    v-if="$clicks === 4"
    class="absolute inset-y-0 left-33 w-18% border-3 border-blue-500 rounded-lg-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    v-if="$clicks === 4"
    class="absolute inset-y-0 right-0 w-35% bg-white/45 pointer-events-none"
  ></div>

  </div>

</div>



:: content :: 

<div class="space-y-6 mt-4">

  <!-- Question -->
  <div v-click class="space-y-1">
    <div class="text-lg">
    1. What behavioural strategies do mice use in matching pennies against a competitive but stationary opponent?
    <br>
    How does this compare to humans and monkeys?
  </div>

  <div class="text-sm italic text-gray-500 ml-2">
    Aloor, Sit et al. — <span class="italic">in preparation</span>
  </div>
  </div>

  <!-- Bullet points -->
  <div class="mt-4 space-y-3 text-lg">
  <div v-click>
    • Mice alternate between bias and stochastic states, increasing stochasticity with learning
  </div>

  <div v-click>
    • Monkeys maintain stochastic strategies consistently throughout sessions
  </div>

  <div v-click>
    • Humans begin with win-stay, then transition to more mixed strategies
  </div>
</div>

  <!-- Final transition question -->
  <div v-click class="mt-8 text-xl font-semibold text-center">
    Do mice change their strategy when playing against another mouse,
    <br>
    where the opponent is no longer stationary?
  </div>

</div>






---
transition: fade
layout: default
---

# Towards animal vs animal multi-agent behaviour



<div class="grid grid-cols-2 gap-6 mt-30 w-full items-start">

<!-- Column 1 -->
<div v-click="1" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-2xl font-semibold leading-snug max-w-xs">
    Animal vs Computer
  </div>

  <img
    src="/animal-experimenter-interaction-v2.svg"
    class="h-80 object-contain rounded-lg -mt-20"
  />
</div>

<!-- Column 2 -->
<div v-click="1" class="flex flex-col items-center text-center gap-0">
  
  <div class="text-2xl font-semibold leading-snug max-w-xs">
    Animal vs Animal
  </div>

  <img
    src="/animal-animal-interaction-v2.svg"
    class="h-80 object-contain rounded-lg -mt-20"
  />
</div>

<!-- Glow highlight -->
<div
  v-click="2"
  class="pointer-events-none absolute left-[50%] top-[15%] w-[45%] h-[75%] rounded-full"
  style="
    box-shadow:
      0 0 0 4px rgba(255, 100, 100, 0.4),
      0 0 40px rgba(255, 100, 100, 0.25);
  "
></div>
</div>


<!-- Pop-up note -->
  <div
    v-click="3"
    class="absolute left-[10%] bottom-[25%] w-[42%] rounded-2xl bg-yellow-100 border-2 border-yellow-300 shadow-xl p-5 rotate-[-2deg]"
  >
    <div class="text-lg font-bold mb-3">
      What can we learn / test that we can't with animal vs computer?
    </div>

  <ul class="text-base leading-snug space-y-2 pl-5 list-disc">
    <li>
      Do mice change strategy when playing against the choice statistics of another mouse?
    </li>
    <li>
      What choice statistics emerge from animal-vs-animal games? Is it different from animal-vs-computer games?
    </li>
  </ul>
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
  class="w-80% mx-auto -mt-5"
/>

<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const vid = document.getElementById('myvid')
  if (vid) {
    vid.playbackRate = 1.0

    vid.addEventListener('ended', () => {
      vid.removeAttribute('controls')   // hide controls
    })
  }
})
</script>

<!-- Acknowledgement (bottom-left) -->
<div class="absolute bottom-6 left-85">
  <div class="bg-white px-4 py-2 rounded-lg shadow-md flex items-center gap-6">

  <!-- Mehul -->
  <div class="flex items-center gap-2">
    <img
      src="/mehul-head.png"
      class="w-10 h-10 rounded-full object-cover border border-gray-300"
    />
    <div class="text-sm text-black">
      Mehul Ristogi
    </div>
  </div>

  <!-- Jeff -->
  <div class="flex items-center gap-2">
    <img
      src="/jeff-head.png"
      class="w-10 h-10 rounded-full object-cover border border-gray-300"
    />
    <div class="text-sm text-black">
      Jeff Erlich
    </div>
  </div>

  </div>
</div>


<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[1%] w-[18%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize -->
  <div
    class="absolute inset-y-0 left-27 w-19% border-2 border-blue-500 rounded-lg-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 right-0 w-19% bg-white/45 pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 left-0 w-62% bg-white/45 pointer-events-none"
  ></div>


  </div>

</div>



---
transition: fade
layout: default
clicks: 6
---


# Mice decrease their entropy when playing against a conspecific

<div class="relative w-full h-[720px]">

  <!-- ===================== -->
  <!-- TOP ROW: THREE PANELS -->
  <!-- ===================== -->
  <div
    class="absolute left-1/2 -translate-x-1/2 w-full grid grid-cols-3 gap-6 transition-all duration-700"
    :class="$clicks >= 4 ? 'top-[40px]' : 'top-[160px]'"
  >

  <!-- Panel 1 -->
  <div v-if="$clicks >= 1" class="flex flex-col items-center text-center">
    <div class="text-sm font-semibold mb-2">
      Mouse vs Computer
    </div>
    <img
      src="/J29_3_sessions_before_multi.svg"
      class="w-full object-contain transition-all duration-700"
    />
  </div>

  <!-- Panel 2 -->
  <div v-if="$clicks >= 2" class="flex flex-col items-center text-center">
    <div class="text-sm font-semibold mb-2">
      Mouse vs Mouse 1st session
    </div>
    <img
      src="/J29_first_multi.svg"
      class="w-full object-contain transition-all duration-700"
    />
  </div>

  <!-- Panel 3 -->
  <div v-if="$clicks >= 3" class="flex flex-col items-center text-center">
    <div class="text-sm font-semibold mb-2">
      Mouse vs Mouse 3rd session
    </div>
    <img
      src="/J29_three_sessions_since_multi.svg"
      class="w-full object-contain transition-all duration-700"
    />
  </div>

  </div>

  <!-- ===================== -->
  <!-- BOTTOM LEFT (CLICK 4) -->
  <!-- ===================== -->
  <img
    v-if="$clicks >= 5"
    src="/J29_solo_to_multi_entropy.svg"
    class="absolute left-[0%] bottom-[40%] w-[65%] object-contain transition-all duration-700"
  />

  <!-- ===================== -->
  <!-- BOTTOM RIGHT (CLICK 5) -->
  <!-- ===================== -->
  <img
    v-if="$clicks >= 6"
    src="/mouse_solo_vs_social_entropy.svg"
    class="absolute right-[10%] bottom-[45%] w-[20%] object-contain transition-all duration-700"
  />

</div>

<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[1%] w-[18%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize -->
  <div
    class="absolute inset-y-0 left-27 w-19% border-2 border-blue-500 rounded-lg-lg pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 right-0 w-19% bg-white/45 pointer-events-none"
  ></div>

  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 left-0 w-62% bg-white/45 pointer-events-none"
  ></div>


  </div>

</div>



---
transition: fade
layout: default
---


# Humans decrease their entropy  when playing against another human


<div class="w-full flex justify-center">
  <div class="relative w-full h-[75vh]">

  <!-- Top image (Click 1) -->
  <img
    v-click="1"
    src="/example_human_MP_vs_MP_choices_and_highlight.svg"
    class="absolute left-1/2 -translate-x-1/2 top-[0%] w-[70%] object-contain"
  />

  <!-- Bottom left (Click 2) -->
  <img
    v-click="2"
    src="/human_solo_vs_social_entropy_line_plot.svg"
    class="absolute left-[25%] bottom-[43%] w-[25%] object-contain"
  />

  <!-- Bottom right (Click 3) -->
  <img
    v-click="3"
    src="/human_solo_vs_social_reward_mp_vs_mp_sessions.svg"
    class="absolute right-[20%] bottom-[43.4%] w-[31%] object-contain"
  />

  </div>
</div>


<!-- Bottom-left overview panel -->
<div
  class="absolute left-[1%] bottom-[1%] w-[18%] z-0"
>
  <div class="rounded-xl border border-gray-300 bg-white p-2 shadow-sm relative overflow-hidden">
    <img
      src="/overview-cartoon.svg"
      class="w-full object-contain"
    />

  <!-- Emphasize -->
  <div
    class="absolute inset-y-0 left-34.5 w-21% border-2 border-blue-500 rounded-lg-l pointer-events-none"
  ></div>


  <!-- de-emphasis -->
  <div
    class="absolute inset-y-0 left-0 w-80% bg-white/45 pointer-events-none"
  ></div>


  </div>

</div>




---
transition: fade
layout: default
clicks: 7
---

# Animal vs Animal Matching pennies : outlook

<div class="mt-6 space-y-3">
  <div v-click="1" class="text-lg">
  Question: How does an individuals training history shape their subsequent strategy?
  </div>
</div>

<div class="relative w-full h-[520px] mt-10">

  <!-- ========================= -->
  <!-- TOP ROW: mice             -->
  <!-- ========================= -->

  <!-- Left -->
  <div
    :class="$clicks >= 2 ? 'opacity-100' : 'opacity-0'"
    class="absolute left-[0%] top-[0%] w-[60%] transition-all duration-700"
  >
    <div class="relative w-full h-[320px]">

  <img src="/mouse-1.svg" class="absolute left-[18%] bottom-[80%] w-[26%]" />
  <img src="/mouse-2.svg" class="absolute right-[18%] bottom-[80%] w-[26%]" />

  <img
    v-if="$clicks < 5"
    src="/random_environment.svg"
    class="absolute left-1/2 -translate-x-1/2 top-[80px] w-[70%]"
  />

  <div v-if="$clicks >= 5">
    <div class="absolute left-[42%] right-[43%] top-[38px] border-t-3 border-black"></div>
    <div class="absolute left-1/2 -translate-x-1/2 top-[8px] text-base font-semibold">
      MP vs MP
    </div>
  </div>

</div>
  </div>

  <!-- Right -->
  <div
    :class="$clicks >= 4 ? 'opacity-100' : 'opacity-0'"
    class="absolute right-[0%] top-[0%] w-[60%] transition-all duration-700"
  >
    <div class="relative w-full h-[320px]">

  <img src="/mouse-3.svg" class="absolute left-[18%] bottom-[80%] w-[26%]" />
  <img src="/mouse-4.svg" class="absolute right-[18%] bottom-[80%] w-[26%]" />

  <img
    v-if="$clicks < 5"
    src="/structured_environment.svg"
    class="absolute left-1/2 -translate-x-1/2 top-[80px] w-[70%]"
  />

  <div v-if="$clicks >= 5">
    <div class="absolute left-[42%] right-[43%] top-[38px] border-t-3 border-black"></div>
    <div class="absolute left-1/2 -translate-x-1/2 top-[8px] text-base font-semibold">
      2AB vs 2AB
    </div>
  </div>

</div>
  </div>

  <!-- Cross connection (mice) -->
  <div v-if="$clicks >= 5">
    <div class="absolute left-[46%] w-[8%] top-[38px] border-t-3 border-black"></div>
    <div class="absolute left-1/2 -translate-x-1/2 top-[60px] text-base font-semibold">
      MP vs 2AB
    </div>
  </div>

  <!-- ========================= -->
  <!-- BOTTOM ROW: females       -->
  <!-- ========================= -->

  <!-- Left -->
  <div
    v-if="$clicks >= 6"
    class="absolute left-[0%] bottom-[35%] w-[60%] transition-all duration-700"
  >
    <div class="relative w-full h-[200px]">

  <img src="/female-1.svg" class="absolute left-[18%] top-0 w-[26%]" />
  <img src="/female-2.svg" class="absolute right-[18%] top-0 w-[26%]" />

  <div class="absolute left-[42%] right-[43%] top-[38px] border-t-3 border-black"></div>
  <div class="absolute left-1/2 -translate-x-1/2 top-[8px] text-base font-semibold">
    MP vs MP
  </div>

</div>
  </div>

  <!-- Right -->
  <div
    v-if="$clicks >= 6"
    class="absolute right-[0%] bottom-[35%] w-[60%]"
  >
    <div class="relative w-full h-[200px]">

  <img src="/female-3.svg" class="absolute left-[18%] top-0 w-[26%]" />
  <img src="/female-4.svg" class="absolute right-[18%] top-0 w-[26%]" />

  <div class="absolute left-[42%] right-[43%] top-[38px] border-t-3 border-black"></div>
  <div class="absolute left-1/2 -translate-x-1/2 top-[8px] text-base font-semibold">
    2AB vs 2AB
  </div>

</div>
  </div>

  <!-- Cross connection (females) -->
  <div v-if="$clicks >= 6">
    <div class="absolute left-[46%] w-[8%] bottom-[270px] border-t-3 border-black"></div>
    <div class="absolute left-1/2 -translate-x-1/2 bottom-[270px] text-base font-semibold">
      MP vs 2AB
    </div>
  </div>

  <!-- ========================= -->
  <!-- CLICK 7: note popup       -->
  <!-- ========================= -->

  <div
    v-if="$clicks >= 7"
    class="absolute right-[2%] top-[10%] w-[30%] bg-amber-50 border border-amber-200 rounded-2xl shadow-xl p-5 rotate-[1deg]"
  >
    <div class="text-lg font-semibold mb-2">
      Other plans
    </div>
    <ul class="list-disc ml-5 text-sm space-y-2">
      <li>simultaneous neuropixel recordings whilst mice play against each other</li>
      <li>modifications of the payoff matrix</li>
      <li>cross-species gameplay!</li>
    </ul>
  </div>

</div>


---
layout: side-title
color: teal 
transition: fade
---

:: title :: 

# Conclusion 

:: content ::

<div style="transform: translateY(3vh)">

<v-clicks :every="2">

<p class="text-lg font-semibold italic text-teal-600">What are the behavioural strategies used by mice in a game of matching pennies against a competitive opponent?</p>
<p class="text-base text-gray-700 mb-4 ml-4">Mice exhibit bias and stochastic states. Within a session, bias states are more likely to occur in the beginning and end of a session. Across learning, mice are more likely to be in the stochastic state.</p>

<p class="text-lg font-semibold italic text-teal-600">How does this behaviour differ between humans and monkeys?</p>
<p class="text-base text-gray-700 mb-4 ml-4">Monkeys maintain in the stochastic state more consistently. Whereas humans tend to first use a win-stay strategy followed by a mix of strategies</p>

<p class="text-lg font-semibold italic text-teal-600">Do we observed a change in behaviour when switching from playing against a computer to player against a conspecific?</p>
<p class="text-base text-gray-700 ml-4">Preliminary results suggest that individuals reduce their stochasticity when playing against a conspecific opponent, presumably because there is lower competitive pressure to randomise</p>

</v-clicks>

</div>


---
layout: default
color: teal
transition: fade
class: p-0 m-0
---

<div class="fixed inset-0 -m-8">

  <!-- Full screen image -->
  <img 
    src="/delab-retreat-2025.JPG" 
    class="w-full h-full object-cover"
  />

  <!-- Title overlay (no dark overlay, semi-transparent box only) -->
  <div class="absolute top-10 left-1/2 -translate-x-1/2">
    <div class="px-10 py-3 rounded-xl bg-black/30 backdrop-blur-sm">
      <h1 class="text-4xl font-bold text-white">
        Acknowledgements
      </h1>
    </div>
  </div>

<!-- Joanna -->
<div class="absolute bottom-70 right-40">
  <div class="px-5 py-2 rounded-lg bg-black/25 backdrop-blur-sm">
    <h2 class="text-lg font-semibold text-white/100 text-center">
      Joanna <br>Mouse MP
    </h2>
  </div>
</div>

<!-- Mehul -->
<div class="absolute bottom-30 left-65">
  <div class="px-5 py-2 rounded-lg bg-black/25 backdrop-blur-sm">
    <h2 class="text-lg font-semibold text-white/100 text-center">
      Mehul <br> Mouse vs Mouse
    </h2>
  </div>
</div>


<!-- Other acknowledgements -->
<div class="absolute bottom-10 left-10 max-w-[28%]">
  <div class="px-3 py-2 rounded-lg bg-black/20 backdrop-blur-sm">
    
  <div class="text-xs font-bold text-white/80 mb-1">
    Human Pilots
  </div>

  <div class="text-xs text-white/80 leading-snug space-y-0.5">
    <div>George Booth</div>
    <div>Betty C</div>
    <div>Person 3</div>
    <div>Person 4</div>
    <div>Person 5</div>
    <div>Person 6</div>
    <div>Person 7</div>
    <div>Person 8</div>
    <div>Person 9</div>
  </div>

  </div>
</div>

</div>




---
transition: fade
---

# Why not just have the mouse play a computer?


- One scientific question we have is what is the statistics of choices of two mice playing each other, and it is hard to know a priori what model can recreate mouse-like behaviour 
- if we have a good model of how mice adapt to the choice statistics of another mouse, then we can indeed have the mouse play against a simulated mouse opponent. We can even test if it is indeed a good model by comparing mouse vs mouse and mouse vs simulated mouse behaviour

---
transition: fade
---

# Isn't this just some form of two-armed bandit task?




---
transition: fade
---

# What can we learn from simultaneous recordings across animals?




