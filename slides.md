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
    Tim Sit | 2026-04-23
  </div>

</div>



---
transition: fade
layout: default
clicks: 6
---

# Multi-agent decision-making tasks are games 

<div class="grid grid-cols-3 gap-8 w-full mt-2 items-start">

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
  <div class="flex items-center justify-center gap-4 mb-3">
  <img
    src="/oli-head.jpg"
    class="w-14 h-14 rounded-full object-cover border border-gray-300"
  /> 
  <img
    src="/chaofei-head.png"
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
    <div class="text-2xl font-semibold mb-4 ">
      Rock paper scissors
    </div>
    <img
      src="/mouse-rock-paper-scissors.png"
      class="w-full max-w-[85%] object-contain"
    />
  </template>
  <div
      v-if="$clicks >= 6"
      class="mt-0 text-sm italic leading-snug max-w-[90%]"
    >
  <div class="flex items-center justify-center gap-4 mb-3 mt-4">
    <img
      src="/joanna-head.png"
      class="w-14 h-14 rounded-full object-cover border border-gray-300"
    /> 
    <img
      src="/tim-head.jpg"
      class="w-14 h-14 rounded-full object-cover border border-gray-300"
    />
    This talk!
  </div>
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
        class="w-full max-w-[85%] object-contain"
      />
    </template>
    <div
      v-if="$clicks >= 4"
      class="mt-0 text-sm italic leading-snug max-w-[90%]"
    >
    <div class="flex items-center justify-center gap-4 mb-3 mt-4">
    <img
      src="/octagon-task-schematic.png"
      class="w-full max-w-[50%] object-contain mb-4 -mt-5"
    />
    <img
      src="/mehul-head.png"
      class="w-14 h-14 rounded-full object-cover border border-gray-300"
    /> 
    <img
      src="/ivana-head.jpg"
      class="w-14 h-14 rounded-full object-cover border border-gray-300"
    />
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
---

# Rock paper scissors as a way of studying strategic stochasticity



---
transition: fade
layout: default
---

# Two ways of studying multi-agent behaviour



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
  v-click="3"
  class="pointer-events-none absolute left-[5%] top-[15%] w-[45%] h-[75%] rounded-full"
  style="
    box-shadow:
      0 0 0 4px rgba(255, 100, 100, 0.4),
      0 0 40px rgba(255, 100, 100, 0.25);
  "
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
layout: two-cols-title
---

:: title :: 

# Studying strategic stochasticity using matching pennies

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
    <div class="ml-4">- Simultaneous binary choice</div>
  </v-click>

  <v-click at="3">
    <div class="ml-4">- Matcher wins if same, unmatcher wins if different</div>
  </v-click>

  <v-click at="6">
    <div class="font-semibold pt-2">Strategies:</div>
  </v-click>

  <v-click at="7">
    <div class="ml-4">- Exploit predictable opponents</div>
  </v-click>

  <v-click at="8">
    <div class="ml-4">- Be unpredictable to avoid exploitation</div>
  </v-click>

  <v-click at="9">
    <div class="font-semibold pt-2">Potential game dynamics:</div>
  </v-click>

  <v-click at="10">
    <div class="ml-4">- Nash equilibrium: both players randomise 50/50</div>
  </v-click>

  <v-click at="11">
    <div class="ml-4">- A player learns to exploit an opponent</div>
  </v-click>

  <v-click at="12">
    <div class="ml-4">- A player learns randomness under competition from a predictive opponent</div>
  </v-click>

</div>


---
transition: fade
layout: side-title
clicks: 5
---

:: title :: 

# Scientific questions

:: content :: 

<div class="space-y-6 mt-10">

  <v-click>

  <div :class="$clicks >= 4 ? 'opacity-100' : ''">
    <div 
      class="text-lg transition-all duration-500"
      :class="$clicks >= 4 ? 'text-blue-500 font-semibold' : ''"
    >
      1. What are the behavioural strategies used by mice in a game of matching pennies against a competitive opponent with a stationary strategy? How does it differ between humans and monkeys?
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
      3. Do mice change their strategy when playing against another mouse, where the strategies of the opponent is no longer stationary?
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


# Matching pennies experiments


<div class="relative w-full h-[760px]">

<!-- Monkey image -->
<img
  v-click="1"
  src="/monkey-algorithms-cartoon-v2.svg"
  class="absolute left-55% -translate-x-1/2 transition-all duration-700"
  :style="$clicks >= 5
    ? 'top: 0rem; width: 55%;'
    : 'top: 1.5rem; width: 80%;'"
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
  src="/mouse-against-algorithm-2-v2.svg"
  class="absolute left-54% top-20% w-[32%]"
/>

<!-- Human image -->
<img
  v-click="7"
  src="/human-vs-algorithm-2-v2.svg"
  class="absolute left-54% top-40% w-[32%]"
/>

</div>



---
transition: fade
layout: two-cols-title 
columns: is-5
---

:: title :: 

# Unsupervised discovery of behavioural strategies using GLM-HMM 

:: left :: 

## Model


<img src="/GLM-HMM-cartoon_v1.svg" class="opacity-100 w-[100%]" v-click="1"/>


:: right :: 

## Verification with synthetic data 


<img src="/recovered_glm_weights_4_states_1.svg" class="opacity-100 w-[100%]" v-click="2"/>


<img src="/p_state_4_states.svg" class="opacity-100 w-[100%]" v-click="3"/>


<div v-click="1" class="absolute bottom-40 left-12 w-[35%] text-sm opacity-75">
  <hr class="border-t border-gray-600 opacity-0 mb-2" />
  
  > Ashwood et al 2022: Mice alternate between discrete strategies during perceptual decision-making (Nat Neuro.)
</div>



---
transition: fade
layout: default
clicks: 5
---

# Monkeys adapt their strategy to the competitive pressure of the opponent

<div class="w-full flex justify-center">
  <div class="relative w-full h-[760px] overflow-hidden">

  <!-- Cartoon -->
  <img
    src="/monkey-algorithms-cartoon-v2.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks === 1
      ? 'top: 90px; width: 70%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 2
      ? 'top: 5%; width: 58%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 58%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- Example choices -->
  <img
    src="/monkey_E_example_choices_per_algorithm.svg"
    class="absolute left-[45%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 2
      ? 'top: 35%; width: 52%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 2
      ? 'top: 30%; width: 52%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 3
      ? 'top: 40px; width: 52%; opacity: 1; transform: translateX(-40%) scale(1);'
      : 'top: 0%; width: 52%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- State weights -->
  <img
    src="/monkey_state_weights_colored.svg"
    class="absolute left-[48%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 3
      ? 'top: 24%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 3
      ? 'top: 20%; width: 60%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 44%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  <!-- Per-session summary -->
  <img
    src="/monkey_state_per_session_summary.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 4
      ? 'top: 30%; width: 80%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : 'top: 25%; width: 80%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  </div>
</div>


---
transition: fade
clicks: 4
---


# Mice alternate between bias and stochastic states


<div class="w-full flex justify-center">
  <div class="relative w-full h-[760px] overflow-hidden">

  <!-- Cartoon -->
  <img
    src="/mouse-against-algorithm-2-v2.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks === 1
      ? 'top: 90px; width: 36%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 2
      ? 'top: 5%; width: 36%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 36%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- Example choices -->
  <img
    src="/example_mouse_naive_to_expert_horizontal.svg"
    class="absolute left-[48%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 2
      ? 'top: 35%; width: 68%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 2
      ? 'top: 30%; width: 68%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 3
      ? 'top: 40px; width: 68%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 68%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- GLM-HMM weights -->
  <img
    src="/glmhmm_glm_weights (1).png"
    class="absolute left-[50%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 3
      ? 'top: 26%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 3
      ? 'top: 32%; width: 70%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 5%; width: 70%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  <!-- Learning summary -->
  <img
    src="/average_pstate_smooth_cosyneabstract2025.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 4
      ? 'top: 30%; width: 50%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : 'top: 30%; width: 50%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  </div>
</div>





---
transition: fade
layout: default
clicks: 4
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
      : $clicks === 2
      ? 'top: 5%; width: 26%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 26%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- Example choices -->
  <img
    src="/example_human_choices.svg"
    class="absolute left-[48%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 2
      ? 'top: 35%; width: 58%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 2
      ? 'top: 30%; width: 58%; opacity: 1; transform: translateX(-50%) scale(1);'
      : $clicks === 3
      ? 'top: 40px; width: 58%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 58%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'"
  />

  <!-- State weights -->
  <img
    src="/human_solo_mp_states.svg"
    class="absolute left-[50%] -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 3
      ? 'top: 26%; width: 60%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : $clicks === 3
      ? 'top: 22%; width: 60%; opacity: 1; transform: translateX(-50%) scale(1);'
      : 'top: 0%; width: 44%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  <!-- Per-session summary -->
  <img
    src="/human_pstate_over_session.svg"
    class="absolute left-1/2 -translate-x-1/2 transition-all duration-700 ease-in-out"
    :style="$clicks < 4
      ? 'top: 30%; width: 80%; opacity: 0; transform: translateX(-50%) scale(0.96); pointer-events: none;'
      : 'top: 25%; width: 80%; opacity: 1; transform: translateX(-50%) scale(1);'"
  />

  </div>
</div>



---
transition: fade
clicks: 4
---

# Interim summary 


<div class="mt-30">

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



# To what extent do each species manage to show random choice patterns?

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


---
transition: fade
layout: side-title
clicks: 5
---

:: title :: 

# Part I Summary

:: content :: 

<div class="space-y-6 mt-2">

  <v-click>

  <div :class="$clicks >= 4 ? 'opacity-100' : ''">
    <div 
      class="text-lg transition-all duration-500"
    >
      1. What are the behavioural strategies used by mice in a game of matching pennies against a competitive opponent with a stationary strategy? How does it differ between humans and monkeys?
    </div>
    <div class="text-sm italic mt-1 ml-4 transition-all duration-500"
         :class="$clicks >= 4 ? 'opacity-90' : 'opacity-70'">
      Aloor, Sit et al. *Strategic stochasticity in mice and monkeys* (in prep)
    </div>
  </div>

  </v-click>

  <v-clicks>

  - Mouse alternate between bias and stochastic states, increasing the proportion of stochastic states over learning
  - Monkeys are better able to maintain stochastic states from start to end of a session
  - Humans start with a win-stay strategy followed by win-switch and other strategies

  </v-clicks>

  <v-click>

  <div :class="$clicks >= 5 ? 'opacity-100' : ''">
    <div class="text-lg font-bold transition-all duration-500">
      Do mice change their strategy when playing against another mouse, where the strategies of the opponent is no longer stationary?
    </div>
  </div>

  </v-click>

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
clicks: 6
---


# Preliminary result: mice decrease their entropy when playing against a conspecific

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


---
transition: fade
layout: default
---


# Preliminary result: humans also decrease their entropy (slightly) when playing against another human


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
    src="/human_solo_vs_social_entropy_mp_vs_mp_sessions.svg"
    class="absolute left-[20%] bottom-[55%] w-[32%] object-contain"
  />

  <!-- Bottom right (Click 3) -->
  <img
    v-click="3"
    src="/human_solo_vs_social_reward_mp_vs_mp_sessions.svg"
    class="absolute right-[20%] bottom-[54.4%] w-[31%] object-contain"
  />

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
    - We observed changes in choice statistics when animals move from playing against a computer to playing against a conspecific
  </div>

  <div v-click="2" class="text-lg">
    - Question: How does an individuals training history shape their subsequent strategy?
  </div>
</div>

<div class="relative w-full h-[520px] mt-10">

  <!-- ========================= -->
  <!-- TOP ROW: mice             -->
  <!-- ========================= -->

  <!-- Left -->
  <div
    :class="$clicks >= 3 ? 'opacity-100' : 'opacity-0'"
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
    class="absolute right-[2%] top-[20%] w-[30%] bg-amber-50 border border-amber-200 rounded-2xl shadow-xl p-5 rotate-[1deg]"
  >
    <div class="text-lg font-semibold mb-2">
      Other plans
    </div>
    <ul class="list-disc ml-5 text-sm space-y-2">
      <li>simultaneous neuropixel recordings whilst mice play against each other</li>
      <li>modifications of the payoff matrix</li>
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

<div style="transform: translateY(6vh)">

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
<div class="absolute bottom-70 right-10">
  <div class="px-5 py-2 rounded-lg bg-black/25 backdrop-blur-sm">
    <h2 class="text-lg font-semibold text-white/100">
      Joanna: Mouse MP
    </h2>
  </div>
</div>

<!-- Mehul -->
<div class="absolute bottom-30 left-60">
  <div class="px-5 py-2 rounded-lg bg-black/25 backdrop-blur-sm">
    <h2 class="text-lg font-semibold text-white/100">
      Mehul: Mouse vs Mouse
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




