---
layout: post
title: FPL Team Composition
header-img: "img/harry-kane-tottenham.jpg"
---

Since last year I have not made any subsequent updates to my genetic algorithm for picking the best fantasy team. In fact, I'm not to sure it is even possible given the long term performance, e.g. Yaya Toure, so instead I wanted to focus on team composition in FPL. Generally speaking, you want to pick players whose matches play to their strengths. I.e., you're not going to pick a Spurs defender when they are playing a good offensive team (I say this as a spurs fan). But, what do those player distributions look like?

![ftd]({{ site.baseurl }}/img/TeamDistributions.png)
*Pictured: All 20 FPL teams from last year. Y-axis is total points over the course of a season.*

Ideally with this type of analysis we would like to see how well the fantasy system rewards certain players on certain teams. That is, just because you fit a system well, doesn't guarantee that you will score well in the FPL system. However, it may have some sort of use in indicating how a team plays. If we take a look at Manchester United and Man City, we'll see that their distributions look a bit different, and interpretation can vary depending on the circumstance. For Man City, you might suggest that it appears that they seem to focus their attacking energy on a couple of players as compared to QPR who totally relied on Charlie Austin. Another team that is difficult to interpret is Arsenal, where Sanchez plays fairly high up the pitch. I would have to predict that Arsenal (no bias) won't finish as high up this year as teams should try to adjust in order to shut him down. Identifying whether or not these are simply the result of desperation or a gameplan will help us to better understand when to pick up certain players.

![ftd]({{ site.baseurl }}/img/Chelsea_Sunderland.png)
*Picture: A closer look at a good team, Chelsea, and a poor one, Sunderland (no offense!)*

![ftd]({{ site.baseurl }}/img/Chelsea_Sunderland_2.png)
*Pictured: Similar to above, except here we take total points and divide it by player cost to get an idea of player ROI (Return on Investment).*

Interestingly enough, a lot of the time I want to try and find the "next" Harry Kane/Michu. The young/unknown star is something that allows you to gain a bit of the differential against other players, and being able to pick them up at the right time (but also knowing when to dump them as well). A bit to the side of this are the players who put up decent enough numbers to make a difference, but lack the name recognition to demand a player cost. I found last year, by looking at the 12/13 data, that Van Persie had quite a low Total Point / Player Cost ratio. He was massively expensive despite his poor output. Some may argue that may have to do with the fact that he is injured a lot, but 1) his ExpG/90 says he's been trending downward for the last 3 seasons anyways and 2) having someone who is injured a lot can be detrimental overall to your team stability-wise. Even with Sunderland, we see that there are some players with decent ratios.

```
> mid[order(mid[,3],decreasing=T),][1:20,]
              V1             V2  V3   V4
2         Hazard        Chelsea 233 10.8
1        Sánchez        Arsenal 207 11.6
4          Silva       Man City 191  9.8
11       Cazorla        Arsenal 168  8.4
6       Fàbregas        Chelsea 165  9.1
18       Eriksen          Spurs 162  7.9
32     Henderson      Liverpool 162  6.6
40        Chadli          Spurs 160  6.2
47       Downing       West Ham 160  5.9
12      Sterling      Liverpool 158  8.3
33    Sigurdsson        Swansea 154  6.5
10          Mata        Man Utd 138  8.5
36          Mané    Southampton 137  6.3
3     Yaya Touré       Man City 134 10.8
17      Coutinho      Liverpool 134  7.9
55       Bolasie Crystal Palace 132  5.6
94 Ki Sung-yueng        Swansea 129  5.1
58      Puncheon Crystal Palace 128  5.5
86         Brunt      West Brom 128  5.2
16         Oscar        Chelsea 126  7.9
```

Simply sorting the top 20 midfielders (by total points) shows us how the name game can be detrimental. Yaya Toure, despite being a huge asset for the 13/14 season, was largely disappointing. I feel bad for anyone who stuck with him on their team for too long. Players like Chadli, Downing, Sigurdsson, Ki, are all the types of players we need to keep an eye on in order to maximize the effectiveness of our benches during the FPL season.

More to come later...
-MT
