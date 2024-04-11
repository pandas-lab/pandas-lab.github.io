---
layout: post
title: "Estimating troop losses on both sides in the Russia-Ukraine war"
featured-img: koi-01.jpeg
authors: [bradford,ydai,nstoehr,aschein,mfernandez,hsajid]
tags: [War, Bayesian Stats]
---

<div class="callout">
This blog post was originally published in ECPR's <a href="https://theloop.ecpr.eu/estimating-troop-losses-on-both-sides-in-the-russia-ukraine-war/"><i>The Loop</i></a> {% cite radford:theloop:2023 %}. It is based on published work by Radford, Dai, Stoehr, Schein, Fernandez, and Sajid {% cite radford:dai:etal:2023 %}. Visit this project's associated <a href="https://github.com/benradford/estimating-conflict-losses">Github repository</a>.
</div>

In February 2022, a simmering conflict between Russia and Ukraine erupted into a full-scale war. Researchers who study wars often define 'war' by the number of deaths experienced in one year of conflict. In addition to its importance in research, assessments of a conflict's losses are integral to accountability and protection of human rights.

> Assessments of a conflict's losses are integral to accountability and protection of human rights

However, precise loss numbers are notoriously difficult to obtain. To better estimate losses obscured by the fog of war, we collected and analysed 4,609 reports about the conflict in Ukraine. We find that Russia has suffered far greater losses than Ukraine, and that both countries likely overestimate the losses of their opponent.

## Individual loss numbers are unreliable

Governments have incentives to manipulate numbers representing losses in a military conflict. Among other reasons, loss numbers may be manipulated to manage public opinion, to boost troops' morale, and to convey particular narratives to allies and opponents. Furthermore, loss numbers are likely to vary across sources simply due to differences in available information from the battlefield.

> Loss numbers may be manipulated to manage public opinion, to boost troops' morale, and to convey particular narratives

In the ongoing Russia-Ukraine conflict, losses reported by different sources vary by orders of magnitude. For example, on 21 September 2022, Russian Defence Minister Sergei Shoigu reported 5,937 Russian soldier fatalities. In the same week, the Ukrainian Ministry of Defence (MoD) reported 55,510 Russian military fatalities. On July 20, 2022, the CIA Director reported around 15,000 Russian fatalities since the invasion.

In our recent paper, we use these and similar reports to better estimate the losses suffered by Russia and Ukraine over the first year of the war. We know the data will likely suffer biases depending on who is reporting losses and whose losses they’re reporting on. However, we see this as an opportunity.

In addition to estimating loss values, we estimate the biases associated with reporting sources. Biases are simply multipliers that scale the actual (unknown) loss numbers up or down. Shoigu’s report of 5,937 fatalities is approximately a tenth of the Ukrainian MoD’s number. Ukraine’s number is likely higher than the actual value. Knowing this, we use a statistical model to estimate these biases while we estimate the actual loss numbers. We begin with the assumption that no sources are biased and we let the data tell us if some sources consistently report above or below others.

<center><img src="../assets/img/posts/estimated-biases.jpeg" style="width:50%"></center>

<p class="caption">Estimated biases for Ukrainian and Russian sources, relative to the country that suffered the loss and the type of loss. Numbers greater than one indicate that sources from that country overestimate losses on average. Numbers less than one indicate underestimation.</p>

## Biases in Russian and Ukrainian sources

We find that Russian sources generally underestimate their own losses and overestimate Ukrainian losses. For every Russian soldier killed, Russian sources report only 0.3 losses. On the contrary, for every Ukrainian soldier killed, Russian sources report 4.3 Ukrainian soldiers killed.

Interestingly, Ukrainian overestimates double Russian soldier deaths. But they tend not to over- or underestimate their own troops’ deaths. Both sides underestimate their own casualties by roughly one half. The table below shows Russian and Ukrainian source biases for military casualties, deaths, and loss of tanks by both sides.

| Loss country  | Loss type	    |  n  | Estimate |
| ------------- |:--------------|----:|---------:|
| Russia        | Tanks	        | 501 |  3,380   |
| Russia        | Casualties    | 130 | 218,800  |
| Russia        | Fatalities    | 523 | 76,687   |
| --------------|---------------|-----|----------|
| Ukraine       | Tanks         | 33  | 2,051    |
| Ukraine       | Casualties    | 16  | 75,538   |
| Ukraine       | Fatalities    | 67  | 17,223   |


<p class="caption">Estimated losses for Ukraine and Russia, at 23 February 2023 </p>


## Our estimates of losses

We find that Russian personnel losses have outpaced Ukrainian personnel losses, with expected loss numbers of 76,687 and 17,223 respectively, as of 23 February 2023. The ratio of casualties to death for Russia and Ukraine are 3:1 and 5:1, respectively. Higher casualty ratios are indicative of better survival rates because they mean fewer wounded soldiers are dying.

> Higher casualty ratios are indicative of better survival rates because they mean fewer wounded soldiers are dying

Importantly, we find that Russian and Ukrainian equipment losses are often comparable by category. For example, the expected losses of tanks for Russia and Ukraine are 3,380 and 2,051, respectively.

Ramifications for Russia
Alexandr Burilkov points out that Putin is under pressure from the ultranationalist forces to continue and escalate the war. But the number of Russian personnel losses and comparable equipment losses is paradoxically high. This reflects a narrative of poorly equipped Russian soldiers and ineffective supply lines. Perhaps those in Putin’s inner circle who are pro-negotiation are better informed about actual losses and the under-equipment of their forces.

The second winter of the Russia-Ukraine war will soon be upon us. With high losses, underequipped forces, and ineffective supply lines, Putin may need to reconsider his choices and move towards a peace plan. Inaccurate reports of how the war is going may bolster popular support, but are an ineffective long-term war strategy.


