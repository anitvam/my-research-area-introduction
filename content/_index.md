+++
title = "Overview on my research area"
outputs = ["Reveal"]
+++

# Individual vs Collective Perspective for MAS
## A quick overview of my research area

---

# Brief introduction

- 3rd year PhD Student from `University of Bologna` (`UNIBO`)
- Supervisor: 
![](https://www.unibo.it/uniboweb/utils/UserImage.aspx?IdAnagrafica=503326&IdFoto=e1c80103) [Danilo Pianini](https://www.unibo.it/sitoweb/danilo.pianini/en)
- Research group context: `Pervasive Computing`

---

## Some faces and topics we are currently working on

![](./images/group-act.svg)

---

## What am I into

![](./images/group-act.svg)


<div class="overlay">
  <div class="circle-1">
  </div>
  <div class="circle-2">
  </div>
  <div class="circle-3">
  </div>
  <div class="circle-4">
  </div>
</div>

</circles>

---

## Industry

- Active collaboration with the italian industry `SCM Group` that operates worldwide
- Project: automation for software updates in the context of industrial woodworking machines
  
  challenges:
  - heterogeneous devices
  - globally distributed devices
  - business-critical machines 

- Main skills: 
  * `Software updates` 
  * `Autonomous pipelines` 
  * `Containerization` 
  * `Virtualization` 
  * `Hypervisors`

---

## Deployment

- Experimenting ways to easily manage several heterogeneous devices and use their resources
- Two clusters offered to run experiments for both *students* and *researchers*:
  * AlmaAI cluster
  * Area 4.0 cluster
- **Managed from researchers for researchers**
- Main skills: 
  * `Container orchestration` (`Docker` and `Kubernetes`)
  * `Virtualization` 
  * `Network configuration` 
  * `Network file system`
  * `Clustered storage`

<br />
<br />

<div>
<small style="text-align: left"> 
[*] Baiardi M., Ciatto G., Pianini D. - Infrastructures for the Edge-Cloud Continuum on a Small Scale: A Practical Case Study. ACSOS-C 2023
</small>
</div>

---

## Conceptualization & Tools


- `Macroprogramming / Aggregate Computing`: Controlling multiple devices/entities at once using `space` and `time`. 
  
  Languages, cronologically:
  - `Scafi`[1]: a Scala Domain-Specific Language (DSL)
  - `Collektive`[2]: a Kotlin Multi-platform DSL
- `BDI Agent-Oriented Programming` 
  - `JaKtA`[3]: my master thesis, a Kotlin DSL implementation for modelling `BDI` agents.
- `Simulation`
  - `Alchemist`[4]: a simulator for pervasive computing, inspired from chemistry reactions.
- Main skills: 
  * `Software development`
  * `Software packaging and delivery`
  * `Testing automation` 
  * `Continuous Integration / Continuous Deployment` 
  * `Build systems`


<br />
<br />

<div>
<small style="text-align: left">

[1] [https://github.com/scafi/scafi](https://github.com/scafi/scafi)<br/>
[2] [https://github.com/Collektive/collektive](https://github.com/Collektive/collektive)<br/>
[3] [https://github.com/jakta-bdi/jakta](https://github.com/jakta-bdi/jakta)<br/>
[4] [https://github.com/AlchemistSimulator/Alchemist](https://github.com/AlchemistSimulator/Alchemist)<br/>

</small>
</div>

---

## Aggregate System vs Multi-Agent Systems

- Same purpose: a way for representing entities adhering to (some) Autonomic Computing principles
  - ... but different scopes

- `Aggregate Computing` is for representing elements in the environment which exhibit a `collective` behaviour.

- `Multi-Agent Programming` is for representing each entity decision process in an environment.

---


## *Here lies the difference*

Viewing system interactions in terms of:

{{% multicol  %}}{{% col class="text-center" %}}

information propagating through <br/> collectives of devices

<i class="fa-solid fa-arrow-down"></i>

`Aggregate Computing`

{{% /col %}}{{% col class="text-center" %}}

individual devices with different interactions <br/> with their peers in the environment

<i class="fa-solid fa-arrow-down"></i>

`Multi-Agent Systems`

{{% /col %}}{{% /multicol %}}

---

## Conceptualization strengths

- A good way to describe the problem allows to explore different perspectives of it.

<img src="./images/conceptual difference.png" width=100% />

---

# Aggregate Applications Examples 

---

### Aggregate Swarm simulations

![](https://user-images.githubusercontent.com/23448811/224012578-d375de46-23c3-44e6-99cf-9d937548a1a5.gif)
![](https://user-images.githubusercontent.com/23448811/224012332-290c81e1-effa-4cab-ae03-c603c116dd99.gif)


<div>
<small style="text-align: left"> 

[source: [https://github.com/scafi/macro-swarm](https://github.com/scafi/macro-swarm) 
]

</small>
</div>

---

## Reinforcement Learning using Aggregate Models

{{% multicol %}}{{% col %}}


![](./images/gaguzzi-paper.png)


{{% /col %}}{{% col %}}

<div class="text-center">

![](./images/gnn-inside-aggregate.png)

</div>

- `Aggregate` is used to enhance agents' state during reinforcement learning
- The information is obtained through the adoption of a `Graph Neural Network` in this paper.


{{% /col %}}{{% /multicol %}}


<small style="text-align: left"> 
[*] Gianluca Aguzzi, Mirko Viroli, Lukas Esterle: Field-informed Reinforcement Learning of Collective Tasks with Graph Neural Networks. (2023) <br />
</small>

---
<!-- 
### Federated Learning using Aggregate Models

{{% multicol %}}{{% col %}}

<div class="text-center">

![](./images/federated-learning-aggregate.png) 
<img src ="./images/csm_federated-learning_01_2dea2cd6c5.png" width=50% />

</div>


{{% multicol %}}{{% col %}}

<div class="text-center">


![](images/scr1.png) 
![](images/scr2.png) 
![](images/scr3.png)

</div>

{{% /col %}} {{% /multicol %}}



{{% /col %}}{{% col %}}

- The aim is to overcome limitations of traditional federated learning models, where
  - Clustering is performed by the central server
  - No. of cluster predefined
  - Central server is a Single-Point of failure 

- `Aggregate` improves the model of the network adopting `Self-Coordination Regions` (SCR)
  - Re-election of the leader in case of failure 
  - Regions are selected on similarity metrics, no pre-defined clustering

{{% /col %}}{{% /multicol %}}


<div>
<small>
[*] D. Domini, G. Aguzzi, N. Farabegoli, M. Viroli and L. Esterle, "Proximity-based Self-Federated Learning," 2024 IEEE International Conference on Autonomic Computing and Self-Organizing Systems (ACSOS), Aarhus, Denmark, 2024 <br />
[*] Domini, D., Aguzzi, G., Esterle, L., Viroli, M. (2024). Field-Based Coordination for Federated Learning. In: Castellani, I., Tiezzi, F. (eds) Coordination Models and Languages. COORDINATION 2024
</small>
</div>

 ---
-->

## Project Emerge   

{{% multicol %}}{{% col %}} 

### @ European Researcher's Night 2025

The project involved robots that autonomously locate themselves in a common pattern by using aggregate computing. 

The robots know their position in the space thanks to an `Aruco marker`, and they use the `Collektive` library to compute their position in the chosen pattern and move accordingly.

![alt text](<images/Aggregate Runtime and-2026-02-19-194841.svg>)

{{% /col %}}{{% col class="text-center" %}}

![alt text](images/IMG_8654.gif)

{{% /col %}}{{% /multicol %}}

<div>
<small>
Aguzzi, G. et al. (2025). A Demonstrator for Self-organizing Robot Teams. In: Di Giusto, C., Ravara, A. (eds) Coordination Models and Languages. COORDINATION 2025. Lecture Notes in Computer Science, vol 15731. Springer, Cham. https://doi.org/10.1007/978-3-031-95589-1_12
</small>
</div>

---


## Adaptive Relay Network Using Aggregate Computing

{{% multicol %}}{{% col %}} 
### @ ACSOS 2025

- To enable autonomous navigation there is the need for real-time high-quality information
- To observe the full-picture, data needs to be collected from central points (i.e. shore stations)
- High-fidelity data are collected locally by ships, then summarised at strategic points within the network and finally forwarded toward the land station

<div class="text-center">
  <img src="images/csc.svg" width="40%" />
</div>

{{% /col %}}{{% col class="text-center" %}}

![alt text](images/simulation.gif)

{{% /col %}}{{% /multicol %}}

<div>
<small>
M. Baiardi, D. Pianini, G. Al-Falouji and S. Tomforde, "Robust Communication Through Collective Adaptive Relay Schemes for Maritime Vessels," 2025 IEEE International Conference on Autonomic Computing and Self-Organizing Systems (ACSOS), Tokyo, Japan, 2025, pp. 21-32, doi: 10.1109/ACSOS66086.2025.00019.
</small>
</div>

---

## Runtime replanning for robot missions

{{% multicol %}}{{% col %}}

### @ ACSOS 2025
- Robots are deployed in the field to perform a mission, but they may be subject to unpredictable connectivity failures
- They perform tasks distributed in the environment
- They share their *state* and *tasks* using gossiping distributed consesus through aggregate computing
- They recompute their plan thanks to the shared information to optimise the mission execution

<div class="text-center">
<img src="images/idea.svg" width="70%" />
</div>

{{% /col %}}{{% col class="text-center" %}}

<img src="images/replanning.gif" width="100%" />

{{% /col %}}{{% /multicol %}}

<div>
<small>
G. Aguzzi et al., "A Field-Based Approach for Runtime Replanning in Swarm Robotics Missions," 2025 IEEE International Conference on Autonomic Computing and Self-Organizing Systems (ACSOS), Tokyo, Japan, 2025, pp. 1-10, doi: 10.1109/ACSOS66086.2025.00017.
</small>
</div>  

---

<!--
## Distributed Applications
#### Running on unknown network topologies

<br/>

{{< figure src="images/path2.svg" width="50%" >}}

 ---

#### May be subject to unpredictable connectivity failures

<br />

{{< figure src="images/path2-6.svg" width="50%" >}}

---

#### We need *autonomous* entities <br/>capable to *adapt* their behaviour to the failure <br/>and continue to work as expected 
<br />

{{< figure src="images/path2-6-1.svg" width="50%" >}} 

---

-->


# My research project 
## BDI Multi-Agent Systems

---

## BDI Multi-Agent Systems

<br />

{{< figure src="images/path43-7.svg" width="50%" >}}

<!-- ---

# Agent-Oriented Programming

<br />


{{< figure src="images/rect46.svg" width="50%" >}}

<small>[1] Weiss, Gerhard, Multiagent Systems. MIT Press, 2013</small>

---

# Agent-Oriented Programming

<br />

{{< figure src="images/BDIAgents.svg" width="50%" >}}

<small>[1] Weiss, Gerhard, Multiagent Systems. MIT Press, 2013</small>
-->

--- 

## BDI Multi-Agent Systems

- System’s description through Goals
    - Imperative Paradigm and Functional Paradigm are suboptimal to do so
    - Huge abstraction gap between instruction and notion representation
- BDI tries to minimise this gap in the abstraction
    - Mimicking human-level notions

<div>
<br/>
<small> 
Bratman, Michael. "Intention, plans, and practical reason." (1987) <br />
</small>
</div>

---

# BDI?

## Beliefs, Desires, Intentions

- *Beliefs*: mental state of the agent, that changes over time.
- *Desires*: motivational state of the system.
- *Intentions*: deliberative state of the agent.

<div>
<br />

<small> 
Anand S. Rao and Michael P. Georgeff. "BDI agents: From theory to practice." (1995) <br />
</small>
</div>

---

# AgentSpeak(L)


{{< figure src="images/Interpreting-AgentSpeakL-Programs.png" width="50%" >}}

<div>
<small>
Anand S. Rao. "Agentspeak(L): BDI agents speak out in a logical computable language." (1996) 
</small>
</div>

---

<!-- # BDI Agent Programming Languages

<br />

{{< figure src="images/AOPlang.svg" width="50%" >}}

<br />

<div>
<small style="text-align: left"> 
[1] Collier, R.W., Russell, S.E., Lillis, D.. "Reflecting on agent programming with AgentSpeak(L). I" (2015) <br />
[2] Hindriks, K.V.. "Programming rational agents in GOAL." (2009) <br />
[3] Pokahr, A., Braubach, L., Lamersdorf, W.. "Jadex: A BDI reasoning engine." (2005) <br />
[4] Bordini, R.H., Hübner, J.F., Wooldridge, M.J.. "Programming Multi-Agent Systems in AgentSpeak using Jason." (2007) <br />
[5] D’Urso, F., Longo, C.F., Santoro, C.. "Programming intelligent iot systems with a python-based declarative tool." (2019) <br />
[6] Palanca, J., Rincon, J.A., Carrascosa, C., Julián, V., Terrasa, A.. "A flexible agent architecture in SPADE." (2022)
</small>
</div> 

---

## Jakta: multi-paradigm AOP/BDI+OOP+FP


```kotlin
mas {                                                   // BDI specification
  fun allPlayers(team: String) =
    Regex("""<a\s(\X*?)\sdata-cy="player">(.*)<\/a>""") // Object-oriented regex library
        .findAll(URL("https://www.besoccer.com/team/squad/$team").readText())
        .map { team to it.groupValues[2] }              // Lambda expression (Functional style)

  listOf("napoli", "milan", "internazionale")           // Kotlin standard library
      .flatMap(::allPlayers)                            // Higher-order function (Functional style)
      .forEach { (team, player) ->                      // Destructuring declaration
          agent(player) {
              beliefs { fact { squad(team) } }
              goals { achieve(start) }
              plans {
                  +achieve(start) onlyIf { squad(S).fromSelf } then {
                      execute(print("Hello! I play for", S))
                  }
              }
          }
      }
}.start()
```

<i class="fa-solid fa-file-code"></i> [SoccerMas.kt](https://github.com/jakta-bdi/jakta-examples/blob/main/src/main/kotlin/it/unibo/jakta/agents/examples/soccer/SoccerMas.kt) 

---
-->

# ...Simplified
## An Autonomic Computing MAPE-K cycle

<br/>

{{% multicol %}}{{% col %}}

<img src="images/autonomic-diagram.svg" width="100%" />

<div class="mx-5 text-center">

## *<i class="fa-solid fa-arrow-up"></i> MAPE-K* 
Reference <u>model</u> for *Autonomic* and *self-\** systems design. 

</div>

{{% /col %}}{{% col  %}}

<div class="mx-5 text-center">


<img src="images/bdi-diagram.svg" width="100%" />

## *<i class="fa-solid fa-arrow-up"></i> BDI* 
Reference <u>framework</u> (*AgentSpeak(L)*) for *Multi-Agent Systems*. 

</div>

{{% /col %}}{{% /multicol %}}

<div>
<small> 
Baiardi M. - Supporting Autonomic Computing via BDI Tooling. ACSOS-C 2024
</small>
</div>

---
<!-- 
# MAPE-K vs. BDI: Key differences

### Conceptual vs. practical

* **MAPE-K** defines a conceptual model, needs application-specific implementations
    * favors ad-hoc implementations
* **BDI** is typically reified into a practical tool (a language or library)
    * enforces commitment to a technology

### Architectural vs. formal

* **MAPE-K** defines a reasoning architecture and a loop scheme
* **BDI** has been formalised into AgentSpeak(L)
    * Typical implementations adhere to the formal specification

### Simple vs. complex

* **MAPE-K** is simpler
    * can be implemented on a per-application basis
* **BDI** requires complex matching ad plan-selection algorithms
    * hard to build from scratch in a custom fashion

--- -->

{{% multicol %}}{{% col class="text-center" %}}


# Current project: 
# *JaKtA*

{{% /col %}}{{% col %}}

<img src="images/jakta_website.png" width="100%" />

{{% /col %}}{{% /multicol %}}
<br />

<div>
<small> 
Baiardi, M., Burattini, S., Ciatto, G., & Pianini, D. - Blending BDI Agents with Object-Oriented and Functional Programming with JaKtA. SN Comput. Sci. 5(8): 1003 (2024)

</small>
</div>

---

<img src="images/Ergonomy.png" width="100%" />

---

## JaKtA: *JA*son-like *K*o*T*lin *A*gents

- **For software engineers**: Multi-paradigm AOP/BDI+OOP+FP BDI Multi-Agent Systems programming framework
- **For research**: Using a single tool to express several types of Distributed systems
- **Key features**: flexibility <i class="fa-solid fa-arrow-right"></i> it allows to plug-in other tools (for example `simulation`) 

---

## Simulation as a validation tool for BDI agents

{{% multicol %}}{{% col class="text-center" %}}

- Same code executed in the real deployment and in the simulation
- We identify multiple event granularity mappings between BDI events and DES Simulation events
   - `Atomic MAS Advancements`
   - `Atomic Control-Loop Iterations`
   - `Atomic Control-Loop Phase`
   - `Atomic BDI Event`

<br />
<br />

### Accepted yesterday at JAAMAS!

{{% /col %}}{{% col class="text-center" %}}

<img src="images/samusversion.svg" width="100%" >

{{% /col %}}{{% /multicol %}}

<div>
<small>
M. Baiardi, "Validation of BDI MASs via Simulation," 2024 28th International Symposium on Distributed Simulation and Real Time Applications (DS-RT), Urbino, Italy, 2024, pp. 128-129, doi: 10.1109/DS-RT62209.2024.00029.
</small>
</div>


---

## Generic BDI tool for Multi-Agent Systems

<img src="images/generic_bdi.png" width="100%" />

<div>
<small>
Burattini, S., Baiardi, M., Ciatto, G., & Pianini, D. (2025). The Gap Between BDI Agents and Semantic Hypermedia and What We Can Do About It. In CEUR WORKSHOP PROCEEDINGS (Vol. 4084, pp. 18-27). CEUR-WS.
</small>
</div>

---

## Still a work in progress

- I am **currently** working on a new version of the tool 
  - Abstracting the knowledge representation
  - Multi-platform supprot (JVM, JavaScript, Native)
  - Efficient implementation using coroutines
  - ...and to let agents adopt `aggregated computation` seamlessly 


<br />
<br />

<div>
<small>
M. Baiardi, "Cognitive Agents in the Field: A Hybrid Approach Between Agent-Oriented and Aggregate Computation," 2025 IEEE International Conference on Autonomic Computing and Self-Organizing Systems Companion (ACSOS-C), Tokyo, Japan, 2025, pp. 176-178, doi: 10.1109/ACSOS-C66519.2025.00050.
</small>
</div>
