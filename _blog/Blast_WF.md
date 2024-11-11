---
title: "CS2 Blast World Final: \"Force or Save?\""
layout: single
---

# Blast World Final save meta

I casually wrapped up watching G2 win the Blast Fall Final in the second to last CS2 event of the calendar year. Extensive qualifiers for this tournament left eight top teams to compete with no clear favorite or expected blowouts. Indeed the tournament favorite, world #1 NAVI, were the first team eliminated.

When I play counter-strike and lose the pistol round (often), its a tough decision whether to buy in the 2nd round, or take the save. I was curious how pro teams made these decisions so I tracked every force and save decision in the tournament.

Of the 64 pistol rounds, there was a perfect 32-32 split between Counter-terrorist (CT) and Terrorist (T) wins. Map picks were fairly spread (Table 1), but Mirage was by far the favorite map pick juxtaposed to Vertigo with only 2 maps played. This follows rumors Vertigo will shortly be replaced with Train in the competitive map pool. Figure 1 also shows the pistol win rate by map.

|-----------------+--------------|
| Mirage | Anubus | Dust II | Inferno | Nuke | Ancient | Vertigo | 
|:-----------:|:----------------:|
| 9 | 5 | 5 | 4 | 4 | 3 | 2 |
|-----------------+--------------|

Table 1: Times each map was played in the 2024 Blast World Final.

<img src="{{ site.url }}{{ site.baseurl }}/assets/images/piston_win_rate.png" alt="">
Figure 1: Pistol round win-rate by map and team.

Next, I checked how often the team which loses the pistol round. Overall, teams forced 54.69% of the time; a slight preference. The results were split across maps and sides as well as shown in Figure 2. Notably, T-side Vertigo, T-side Inferno, and CT-side Ancient never opted for a force buy after losing the pistol while CT-side Nuke and CT-side DustII always chose to force.

<img src="{{ site.url }}{{ site.baseurl }}/assets/images/force_rate.png" alt="">
Figure 2: 2nd round force rate by map and team

Let's check the probability of winning the second round if you force vs. if you do not force. Teams saving in the second round won precisely 0% of their save rounds. More notably, the overall force win success rate was just 14%, so why force at all? We need to look at the resulting 3rd round. The thought behind saving and effectively conceding the 2nd round is to boost your chance of winning the 3rd. Teams that saved had a 50% win rate in the 3rd round while teams that forced sit at 34%.

The overall win rate in the 2nd and 3rd round for teams that lose the pistol is 24.6%. When deciding between forcing and saving, I consider the overall probability of victory in the next two rounds. For the sake of simplicity, lets add the probabilities of round victories given different situations. From here forward P(force) and P(save) refer to the combined probability of the next two rounds given a force or save in the 2nd round. Overall, P(save)=50% (0% + 50%) while P(force)=48% (14% + 34%). Lets check some potential co-factors however that should affect these statistics.

First, lets consider side. CTs forced 64.5% compared to 47% for Ts. CT's P(save)=45%  compared to P(force)=35%, suggesting its better for the CTs to save. The values on T-side were P(save)=53% and P(force)=66% indicating a pretty decent edge for the T-side when forcing.

Successfully planting the bomb on T-side comes with a $300 bonus to the player planting the bomb along with $800 for their teammates in the event of a round loss. Therefore, forcing is a more tempting prospect if the bomb was planted. Across all 64 rounds, the bomb was planted 64% of the time. If the T-side did not plant the bomb, P(force)=60% and P(save)=57%. Surprisingly, a slight edge exists to force even without a plant. There was an effect of planting however. If the T-side planted the bomb in the pistol round, P(force)=70% while P(save)=33%. This value strongly suggests you plant, you buy. 

Now its time for the boring caveats and discussion. First, the sample size is not extensive. 64 pistol rounds may seem like a lot, but when breaking down co-factors such as side and plant, one round can swing these summary statistics by several points. The most obvious caveat to take away when making your own decisions in game is these are top-tier professionals. Their decision-making and subsequent outcomes have little bearing on my own gameplay at least since they're effectively playing a different game than we are. I think pro player's effectiveness with the Desert Eagle epitomizes this point. At only $700 and with a one-shot headshot potential, this weapon is highly effective in the hands of someone that can actually aim and frequently flips round outcomes at the pro level in save and force buy scenarios. Another factor I failed to consider was the game situation. I hypothesize teams are more likely to force buy in the second half when trailing greatly and conversely more likely to save when leading. Although there were 64 pistol rounds, I was missing data for the 2nd and 3rd rounds of the Liquid vs. G2 opening game where G2 was 13-0'd then went on to win the whole damn thing. This analysis convinced me to try and save more on CT while following the "you plant, you buy" adage more often, but the correct answer 100% of the time to give you an advantage is simply buy with your team.

