I was trying to see how I could make something FIRE. I started with the amencutup and some arpy lines, but wasn't sure where I would go with this. I initially wanted to use a bass sample to play a bass line in the middle after muting the amencutup and arpy samples to create a vibe change, but I wasn't able to get it working due to using n instead of note. Instead, I ended up with a bassfoo, which sounded like an alarm clock, and I came up with the idea of the set being based on waking up.







d4 $ s "[bd | bd | bd | bd | bd | bd*4 | ~ | ~ | ~ | ~ | ~ | ~ | bd | bd | bd | bd | bd*59 | bd | bd | bd*2] ~ [sd | sd | sd | sd | sd | sd*5 | ~ | ~ | ~ | ~ | ~] ~ [bd | bd | bd | bd*5 | bd*2 | bd*3 | bd | bd | bd | bd | ~ | ~ | ~ | ~] ~ [~ | ~ | ~ | ~ | sd | sd | sd | sd | sd | sd | sd | sd | sd | sd | sd | sd | sd | sd | sd | sd*6 | sd*999]" # pan sine
hush
d1 $ s ""
d3 $ s "[hc | ho | hc | ho | hc | ho | hc | ho | hc*5 | ho*7 | ho*300] [~ | ~ | ~ | ~ | ho | hc | ho | hc*3 | ho*3 | hc*5 | ho | hc | ho | hc] [~ | ~ | ~ | ~ | ~ | ~ | hc | hc | ho | hc | ho | hc | ho | ho*251] [~ | ~ | ~ | ~ | hc | ho | hc | ho | hc | ho | hc | ho | hc | ho | ho | hc | ho | hc*351] [~ | ~ | ~ | ~ | hc | ho | hc | ho | hc | ho | hc | ho | hc | ho*613] [~ | ~ | ~ | ~ | ~ | hc | ho | hc | ho | hc | ho | hc | ho | hc] [~ | ~ | ~ | ~ | hc | ho | hc | ho | hc*2 | hc | ho | hc | ho | hc | ho | hc | ho*719 | ho*3 | hc*6 | ho*5 | hc*4] hc ho" # pan sine # gain 0.75
d4 $ n "1 1 4 5 6 2 3 4 5 8 9 2 8 11 32 24 25" # s "amencutup*2"
d4 $ n "1 2 3 1 2 3 1 2 3 4 4 8 8 9 1 1 1 32 31 30 29 5 8 7" # s "amencutup*2"
once $ arp "downup" $ s "bass1*4" # n "bb'min a'min ab'min g'min"
d1 $ s "bassfoo" # n "1"
d2 $ arp "updown" $ n "c'major c'major c'major eb'major eb'major e'major e'major" # s "arpy*4" # gain 0.9 # legato 2
d2 $ arp "updown" $ n "c'major c'major c'major eb'major eb'major e'major e'major" # s "arpy*4" # gain 0.9 # legato 0.5 # phaserdepth 0.7 # phaserrate 0.7
d2 $ arp "updown" $ n "c'minor c'minor c'minor b'major b'major e'minor e'minor" # s "arpy*4" # gain 0.9 # legato 0.5
d2 $ arp "updown" $ n "c'minor c'minor c'minor b'major b'major e'minor e'minor" # s "arpy*4" # gain 0.9 # legato 0.5 # delay 0.3

d2 $ arp "downup" $ n "c'major c'major c'major eb'major eb'major e'major e'major" # s "arpy*4" # delay 0.5 # legato 2 # gain 0.8
d2 $ arp "downup" $ n "c'major c'major c'major eb'major eb'major e'major e'major" # s "arpy*4" # delay 0.5 # legato 0.5 # gain 0.8

d2 $ s "arpy*4" $ every 2 (arp "updown" $ n "c'minor c'minor c'minor b'major b'major e'minor e'minor") $ arp "downup" $ n "c'major c'major c'major eb'major eb'major e'major e'major" # s "arpy*4" # delay 0.5 # legato 0.5 # gain 0.8
d2 $ s""
d4 $ n "32 32 4 5 8 8 9 1 1 1 1 2 2 3 4 6 5 8 7" # s "amencutup*2"
d4 $ n "32 32 4 5 8 8 9 1 1 1 1 2 2 3 4 6 5 8 7" # s "amencutup*3"
d3 $ s "birds" # n "1 1 4 1 5 6 7 1" # pan isaw # gain 1.5
d4 $ s ""
d4 $ n "32 32 4 5 8 8 9 1 1 1 1 2 2 3 4 6 5 8 7" # s "amencutup*2"
d1 $ s ""
d2 $ s ""
d3 $ s ""
d4 $ s ""

d4 $ s "jungle*8" # n "{1 ~ 1 ~ 1 1 ~ ~ 1 ~ ~ 1 1 ~ 1 ~, 6 6 12 6 12 6 6 12 12 13 12 6 6}"

d1 $ s "bassfoo" # n "1"
d3 $ s "birds" # n "1 1 4 1 5 6 7 1" # pan isaw # gain 1.2
d4 $ n "32 32 4 5 8 8 9 1 1 1 1 2 2 3 4 6 5 8 7" # s "amencutup*2"
d2 $ arp "updown" $ n "c'major c'major c'major eb'major eb'major e'major e'major" # s "arpy*4" # gain 0.9 # legato 0.5 # phaserdepth 0.7 # phaserrate 0.7
d1 $ s ""
d3 $ s ""




once $ s "xmas" # speed 0.25
