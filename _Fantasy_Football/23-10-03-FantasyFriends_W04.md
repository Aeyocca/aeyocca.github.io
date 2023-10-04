---
title: "Fantasy Friends Fantasy Football League Week 4 recap"
date: 2023-10-03
layout: single
---

# We're bad at fantasy football??

In fantasy football, we select players we think will score the most fantasy points. Our available pool of all players is split equitably between our ten rosters through the draft. Player evaluations change suddenly in fantasy football as new information becomes available. Through the first four weeks of the fantasy season, most assume they're predictive accuracy closely aligns with Sunday's results. This league, however, appears no better than a toddler button mashing Mommy's iPad on the waiver wire when it comes to fantasy defenses and the tight end position. For example, both Alan's Two Win Weiners and Bill's Bitch added defenses Sunday at noon before kickoff and found the 6th most, and the top fantasy scoring defenses for the week. In fact, there was no statistical difference in the mean fantasy finishes of started and nonstarted defenses this week (Figure 1; Supplementary Methods).

![defenses_are_stupid](/assets/images/DST_are_stupid_W04.png){:class="img-responsive"}
Figure 1. Student's t-Test results for the mean fantasy finish of fantasy defense and special teams started vs. those not started Week 04 in Fantasy Friends league.

We were even worse with tight-ends this week (Figure 2; Supplementary Methods)!

![TEs_are_stupid](ayocca.github.io/assets/images/TE_are_stupid_W04.png){:class="img-responsive"}
Figure 2. Student's t-Test results for the mean fantasy finish of tight-ends started vs. those not started Week 04 in Fantasy Friends league.

Are we bad at fantasy football? Are we just a bunch of toddlers at the iPad? Are defenses and TEs stupid? Or should we start multiple TEs and defenses? We don't have this issue with


# Matchups

Alan's Two Win Weiners were picked off by Bill's Bitch in this week's toilet bowl. Each squad consisted of mostly duds, one good QB performance, one decent skill position performance, and great defensive scores. Justin Fields (27.9) finally came alive for fantasy purposes throwing 4 TDs against the struggling Denver defense. A pair of turnovers late in the game however sent the Bears to 0-4 on the season. For Bill's Bitch, Jalen Hurts (24.16) produced in a tight division game, and Amon-Ra (16.6) played through his turf toe injury for a decent day. George Kittle however (1.9) was not needed as Christian "The Goat" McCaffery absorbed nearly the entire 49ers offense this week (more on him later). The Weiners streamed the Chargers DST against Raiders rookie Aiden OConnel to the tune of 16 fantasy points, 6th best on the week. Heading into Monday night, Seattle needed 15 points against the Giants for Bill's Bitch to win. A few early sacks had the defense trending up and the victory was sealed by a 97 yard pick-six near the end of the first half. Primetime Kirk Cousins? More like Primetime Danny Dimes who is now 0-7 on Monday Night Football. Fun fact, 



## Weekly predictions

We went perfect this week!!! but still sit at 8-7 total. ESPN projections only went 3-2  but sit at 10-5. This week's winners are: Alan's Two Win Weiners, Am I good?, The Steagles, Token Female, and Red Solo Kupp


## Supplementary Methods

Data were manually curated from https://fantasy.espn.com/football/players/add?leagueId=1804892 (last accesses 10-03-2023 at 8:44pm by AEY). Players were classified as "Started" if they were in a team's starting lineup. Fantasy finishes were counted by sorting "All" players at their respective positions for "LAST". 11 fantasy defenses were on rosters. Cleveland was the only rostered defense (fantasy finish 14) and was therefore classified as "not started". For tight-ends, only the top 32 fantasy finshers were considered. 11 of the 32 were rostered, and nine of those were started. The nine started TEs composed `list_started_TE` and the 21 TEs in the top 32 on the waivers composed `list_nonstarted_TE`. The two TEs in the top 32 that were rostered but not started were excluded from this analysis. Our two sets of fantasy finishes were tested for differences in means using the Student's t-Test under default parameters in R version 4.2.1 (2022-06-23).