# BSidesRDU 2021
### Seeing Through The Deception - How to Detect High Interaction Honeypots in the Wild
#### Jason M. Pittman, Sc.D.
#### September 24th, 2021

<hr>
#### About the Research

A honeypot is an intentionally vulnerable computing system designed to deceive attackers into revealing their tools and techniques. The objective of deceiving attackers is either to develop new countermeasures or distract them from targeting production systems. But do honeypots work, are they effective in these roles?

The honest answer is no one knows. The reason why no one knows is honeypot technology has a hidden bias- it only captures attacks directed to it. This bias might be self-evident but a critical side effect might not be so obvious. Spitzner introduced honeypots in 1999 and within five years research appeared asserting a method to detect and attack them. There are two reasons underpinning the significance of such a discovery.

First, defenders deploy enough honeypots that adversaries have a vested interest in understanding how to attack them.

Second, and less obvious, attackers must have a reliable methodology to detect honeypots.

To that end, we don't know how many attackers don't attack honeypots. Think about it: do you know how an attacker might detect your honeypot or differentiate between deceptive and legitimate systems on your perimeter? After all, attackers have a vested interest in understanding how to detect honeypots in the wild. They don't want to waste time. They don't want to increase risk without raising the potential payout. They want to maintain confidentiality of their tools and techniques.

Oddly enough, existing research is not clear on what network or system attributes reveal a high interaction honeypot. Consequently, no one knows to what extent attackers may be detecting and avoiding honeypots. At best, this limits the ability for researchers to develop more robust honeypots which can evade detection. The worse case however is the calling into question the legitimacy of the technology overall.

Accordingly, in this talk I provide a potential model for honeypot detection along with the results of scanning 59,392 IP Addresses during a series of validation experiments. The findings demonstrate a set of characteristics usable as identification criteria.

#### What is in this repo

You will find two file objects (other than this README): `northstate_scan.txt` and `Seeing Through The Deception.pdf`.

The scan file contains the raw NMAP results, unsorted and unanalzed. 

The PDF file is the presentation deck, including the process I used to operationalize the scan data into a honeypot detection model.

#### What is not in this repo
I opted to not include any of my instrumentation at this time. I made this decision because I want the focus of this research to remain on the theoretical model.

The presentation PDF contains instrumentation details in case you want to reconstruct this work. However, I encourage you to apply your own techniques to (a) further validate the model and (b) add new characterstics to the set *C*.



