Monkeystrike 1.0
================

After more than 2 years of partially not very intensive developingthe first official release of Monkeystrike is ready to release. First of all there is a lot of excuses to be made: 2 Years is a very long time but there were long periods of time where everybody was reall inactive and did not really want to go on. Also we revamped Monkeystrike completely for at least 2 times.
Another bad habit of us is the last minute work. We have been under big time pressure because Superpinki was leaving us for 10 weeks and R2-D2 for 2 weeks. There is more important factors like that which made us work our butts off to get everything done in time. This explains some disturbing bugs that we even know of.
So if you are ever going to review Monkeystrike in any way please keep that in mind while writing your criticism.

Furthermore we would like to thank all the people that helped us, were with us and motivated us to finish this project. Then there are people who we got to know really well by the time and who we have become pretty close friends with. We like to refer to it as "the core". Without them we would not have finished Monkeystrike: Ike_Brovlofski (our biggest fan ever), BoBaCk, Thinge, Darkfighter, BigBird, CyBBe, B3N, Sofa, JynxDaddy, Bubba Gump Shrimp, TitaniumMonkey, Beeblebrox.
Special thanks go out to Creme and Thinge our two linux experts and server guys who made a linux server version of Monkeystrike possible.
We also thank everybody that we forgot and/or helped us in any way and I myself (R2-D2) want to thank Blink 182 as well for always supporting me while I was working for Monkeystrike :)


Monkeystrike 1.1 patch
======================

While R2-D2 takes that much needed break, I was tracked down by another mod community friend (who I even yelled at for wakin
me up! Sorry Max) to help the MS team with a few bugs that caused server crashes. While poking about in the code, I even
fixed a few other issues, and if the team is comfortable with it, I'll even put my $0.02 in to help track down some other issues that persist. Thanks guys for bringing us all such a cool mod, and I hope to see you all on the servers :D. 
- sluggo

Bugs fixed:
-----------

- crash on CTB maps.
- fixed issues with golden banana staying 'attached' to dead or disconnected players on CTB maps.
- screen shaking on player connect and improve network performance when first connecting.
- reducted strawberry machinegun damage by 25%.
- fix nasty random crashes, the way the scoring for fs maps was being done was overwriting.
  memory inside the Halflife engine, strawberry team's score was always random as a result.
- removed buggy easter eggs (team and beta testers only).
- fixed a weird crash where skunks tossed by disconnected players would cause server crashes
  (thanks to bigbird, thing`e` and others for helping me find that one).
- new version of ctb_circus
- added missing moon-ms.wad
- new chimpanzee model

Monkeystrike 1.2 patch
======================

Bugs fixed:
----------

- fixed two more crashes in dedicated server code, one related to minimonkeys leap attack
  (after the player died and lost weapons we were accessing their active weapon), and one
  related to skunk farts doing damage after the skunk dies
- fixed resetting scores in fs gameplay, the score would reset when a new player connected
  to the server because of where some code was located, moved to CHalflifeTeamPlay constructor,
  the proper spot for it.
- remove the model command
- changes to fs gameplay:
  - players now get 100 points per capture, team gets one point, this increases the reward for
    working towards the team goal of capturing fruits (new CVAR: mp_fruitbonus)
  - first team to capture (CVAR: mp_fruitlimit) fruits wins, this now works correctly, and
    is also updated when the captures happen, this will switch the map.
- eastereggs are completely removed
- strawberry machine gun now 25% again weakened
- team/class change menus appear on level change
- fixed shotgun reload exploit, maximum is 5 rounds in all cases
- tried to reproduce the demo/voicerecord bug. either it was a phantom (probably not) or the
  client code was old that we delivered in 1.0, or my world is invaded by monkies :).
- added teammate identification system, only in place when teams are in effect (i.e not on
  ms_maps).

