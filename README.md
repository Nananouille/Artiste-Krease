

- __                                         
- |  | _________   ____ _____  ________ ____  
- |  |/ /\_  __ \_/ __ \\__  \ \___   // __ \ 
- |    <  |  | \/\  ___/ / __ \_/    /\  ___/ 
- |__|_ \ |__|    \___  >____  /_____ \\___  >
-    \/             \/     \/      \/    \/ 

(つ◉益◉)つ

#### Krease

![This is an image](https://scontent-cdt1-1.xx.fbcdn.net/v/t39.30808-1/274332014_5277218398964102_8297495416610704222_n.jpg?stp=cp0_dst-jpg_p60x60&_nc_cat=105&ccb=1-7&_nc_sid=c6021c&_nc_ohc=jyyMRQhAbg0AX_RPU-1&tn=JccsvCW0h8j7PqIG&_nc_ht=scontent-cdt1-1.xx&oh=00_AfAZXWpiZf2v4yy-Uk0MbTWH8lZf0OKx8lcSUzahZgfy1A&oe=63C19617)

###level  1:
jouer a paris au stock 
* Jouer a Atelier du  vents
* Jouer blokaus 
* Jouer a Amaze Festival panke gallery berlin  mai 6            100 nanouilles
* joue  a Ins3kaeve      Zurr Klappe berlin    mai 12            100 nanouilles
* Jouer a stereolux 30 mars 2023            100 nanouilles
* Points nanouille:                         400 nanouilles
* cookiecollective partie;                  100 nanouilles
* No School festival                        100 nanouilles
* féstival de la creativité numérique.      100 nanouilles
* Solstice Night Stream December 2022       100 nanouilles
* ROUTENOTE POUR LA DISTRIBUTION DE MUSIQUE  100 nanouilles
* creation dropBox                           100 nanouilles
* Préparation scéne Twitch                    50 nanouilles
* petit streaming de test                     10 nanouilles
* inscription  www.spotify.com                5 nanouilles
* new vintage vsti                            1 nanouilles
##tools
- orca
- processing
- unity
- sardine
- strudel


goal:
* festival x
* Event :
-
-
-
-
-
 log 30 
curl -fsSL https://code-server.dev/install.sh | sh -s -- --dry-run
 no need just npm:  npm install --global code-server --unsafe-perm 
au final  en local : npm install code-server --prefix="C:\Users\vjbli\AppData\Roaming\npm\node_modules\npm\node_modules" 

et donc  :  npm install code-server --prefix="C:\Users\vjbli\AppData\Roaming\npm\node_modules\npm" --unsafe-perm
 
 ![image](https://github.com/Nananouille/Artiste-Krease/assets/8178673/33b340b6-b892-4ef9-bce4-b0b186da09bf)

 
 nfc tangigible music done with osc nfctool that send an url with the osc info with the help of a server  start by a bat file
 

* bar   livebar x
* streaming
* Album
* track on soundcloud 2
* dsp free  https://www.rou
*
*
*tenote.com/rn/welcome_page
* present on  virtual world


log 29  instalation sardine 
log 28    live au blockhaus 


osc(6,-0.015,0.3).diff(osc(60,0.08).rotate(Math.PI/2))
	.modulateScale(noise(3.5,0.25).modulateScale(osc(15).rotate(()=>Math.sin(time/2))),0.6)
	.color(1,0.5,0.4).contrast(1.4)
	.add(src(o0).modulate(o0,.04),.6)
	.invert().brightness(0.1).contrast(2)
	.modulateScale(osc(12),-0.2)
  .out()


log 27 

strudel 
blender upbge


####"##rise in strudel : 

let gg= saw.range(0,28).slow(13)

note(" [ 52*8]").s ("oh").fast(gg).add(gg)
    .clip(1).release(.5).gain("2")

.pianoroll()


#########  use of if in strudel 

let intro = 0;

let run = () => {
  if(intro) {
    return s("bd sd")
  }
  return s("bd*2 sd, hh*4")
}

run()

##########"" mask 
stack

(
  s("bd rim").mask("<1!4 0!8>"),
  s("bd*2,~ sd, hh*4").mask("<0!4 1!8>")
)
arrange
let intro = stack(
  s("bd")
)

let chorus = stack(
  s("bd*2, rim, hh*4")
)

arrange(
  [4, intro],
  [8, chorus],
)

let intro = stack(
  s("bd")
)

let chorus = stack(
  s("bd*2, rim, hh*4")
)

arrange(
  [4, intro],
  [8, chorus],
)

log 26 strudel can directly talk to ableton  isnt that great ! 
"<0 6 [0 6]>"
.scale('D minor')
.legato(.5)
.echo(4, 1/8, .5)
.note().midi('loopMIDI Port 3')
.pianoroll()



log 25
sardin wont work ... 
tidal barely working

dnb  patern is like 
do
  d2 $ every 8 (stutter 2 (3/16)) $ fast 1 $ s"~  ~ sn:2 ~  ~  ~  sn:2*1  ~" 
  d1 $ s"bd ~  ~   ~  ~ bd ~ ~"
  d3 $ fast 4 $ s "bd"  
   
strudel
tempo(120) {
  schedule(0, [
    note(2, every(8, stutter(2, dur(3 / 16))), s("~  ~ sn:2 ~  ~  ~  sn:2*1  ~")),
    note(1, s("bd ~  ~   ~  ~ bd ~ ~")),
    note(3, fast(4, s("bd")))
  ])
}

log 23  midi on sardine and making sardin working :  sardin-config  

clock.tempo=170
your_midi_port: str = 'Springbeats vMIDI4 5'
your_midi = MidiHandler(port_name=your_midi_port)

# Add the MIDI port to the session fishbowl
bowl.add_handler(your_midi)


_play_factory = Player._play_factory
 
def n3(*args, **kwargs):
    return _play_factory(your_midi, your_midi.send, *args, **kwargs)

N3 = your_midi.send  # For sending MIDI Notes

Pa * n3('C1  C4 ', p=1) # playing a chord, one note every 1/4 of a beat.

 p
Pa * n3('C1  G1 ', p='.5!2 0.25!2 .75!4 .75!4 ') 
gg= "[41 21 4 2] [4 5 4 2] [3 1 3 1] [3 4 3 1] [4 2 4 2] [4 5 4 2]"
gg= " [0 4 7 9 10 88 4 7 9 10 11]+20 C5@five "

gg= "[41 . . 77 ] "

gg="(0 1 2)<3,5>"

gg= "C4 ..."
 

Pa * n3(gg, p='4',scal='major') 


log 23 
sardine operationel cmd admin mode 

https://hydra.ojack.xyz/api/#functions/contrast/0

https://hydra.ojack.xyz/?code=b3NjKDIwLjAzOCUyQyUyMDAuMDEyJTJDJTIwNzAwLjQxMyklMEElMDkuc2Nyb2xsWCgwLjA2NSklMEElMDkuYmxlbmQobzApJTBBJTA5LnJvdGF0ZSgxLjQ4MyklMEElMDkuY29sb3JhbWEoMC43MTcpJTBBJTA5LmNvbnRyYXN0KCgpJTIwJTNEJTNFJTIwTWF0aC5zaW4odGltZSklMjAqJTIwNSklMEElMDkubHVtYSgpJTBBJTA5Lm1vZHVsYXRlSHVlKG8wKSUwQSUwOS5zY2FsZSgxLjEzOSklMEElMDkubW9kdWxhdGUob3NjKCklMEElMDklMDkubW9kdWxhdGUodm9yb25vaSgoKSUyMCUzRCUzRSUyMGEuZmZ0JTVCMCU1RCUyMColMjAxMCklMkMlMjAwLjEpKSUwQSUwOS5vdXQoKSUzQg%3D%3D


https://hydra.ojack.xyz/?code=b3NjKDIwLjAzOCUyQyUyMDAuMDEyJTJDJTIwNzAwLjQxMyklMEElMDkuc2Nyb2xsWCgwLjA2NSklMEElMDkuYmxlbmQobzApJTBBJTA5LnJvdGF0ZSgxLjQ4MyklMEElMDkuY29sb3JhbWEoMC43MTcpJTBBJTA5JTJGJTJGLmNvbnRyYXN0KCgpJTIwJTNEJTNFJTIwTWF0aC5zaW4odGltZSklMjAqJTIwNSklMEElMDkubHVtYSgpJTBBJTA5JTJGJTJGLm1vZHVsYXRlSHVlKG8wKSUwQSUwOS5zY2FsZSgxLjEzOSklMEElMDklMkYlMkYubW9kdWxhdGUob3NjKCkubW9kdWxhdGUodm9yb25vaSgoNDQpJTIwJTNEJTNFJTIwYS5mZnQlNUIwJTVEJTIwKiUyMDEwKSUyQyUyMDApKSUwQSUwOSUyRiUyRi5tb2R1bGF0ZShvMCUyQyUyMCgpJTIwJTNEJTNFJTIwbW91c2UueCUyMColMjAwLjAwMDMpJTBBJTBBJTA5Lm91dCgpJTNC

log 22:

play at panke gallery et zurr klappe 
https://soundcloud.com/dekrease/ins3kt-raeve-zur-klappe?si=1d50fee4240a4be2867e817d1c32363e&utm_source=clipboard&utm_medium=text&utm_campaign=social_sharing


Defis:

log 20 bespoke daw free instalation et utilisesation jupiter notebook decouverte bark tts et son spatialisé avec three.js


pip install notebook

créer un python console et apeller import bark1

log 19 :

Clock.bpm = 174
techno
d1 >> play("ddddd", sample=2, dur=1/8, amp=0.8)
d2 >> play("X___X___X___X___", sample=4, dur=1/8, amp=0.8)
d3 >> play("__:___:___:___:_", sample=2, dur=1/8, amp=0.8)

dnb style 1
d1 >> play("----", sample=2, dur=1/4, amp=0.8)
d1.stop()
d2 >> play("x________x_____",drive=.041, sample=1, dur=1/4, amp=.8)
d2 >> play("x________x_____",drive=.041, sample=1, dur=1/4, amp=.8)
d3 >> play("____O_______O___", sample=1, dur=1/4, amp=0.8)
d3 >> play("____O__O____O___", sample=1, dur=1/4, amp=0.8,delay=.0)
d3 >> play("_O__O_______O___", sample=1, dur=1/4, amp=0.8)

d1 >> play(":______:_____:____:_____:____", sample=2, dur=1/8, amp=0.8)



dnb style 2

d1.stop()
d2 >> play("x_____x_____x___x_____x_____x___", sample=4, dur=1/8, amp=0.8)
d3 >> play("____O_____O_________O_____O_____", sample=4, dur=1/8, amp=0.8)
d3 >> play(":______:_____:____:_____:____", sample=2, dur=1/8, amp=0.8)

d4 >> play("-_-_-_-_", sample=4, dur=1/4, amp=2.8)
d5 >> play("_-_-__-_", sample=9, dur=1/4, amp=2.8)
d3.stop()
Clock.clear()





log 14 omniverse 
he Launcher Clean-Up Tool will put the Omniverse Launcher back into a clean slate 
Set your preferred data path and click ‘Next’. Enter your desired credentials for the Administrator Account and then click ‘Complete Setup’.

Nucleus Workstation will now download and install. There are several ways to verify the installation:

    Click the menu icon next to ‘Local Nucleus Service’ and click ‘Settings’ to bring up System Monitor. Check that all services are listed as ‘Running’

    Click the folder icon next to ‘Local Nucleus Service’ to bring up Omniverse Nucleus Navigator. Log in using the Administrator account

    Connect to System Monitor by navigating to http://localhost:3080 in a browser. Check that all apps are listed as ‘Running’

    Connect to Navigator by navigating to http://localhost:34080 in a browser. Log in using ‘admin’ or ‘omniverse’ for both the username and password

log 13 
 py -m venv .
 
 py -3.9-64 -m pip install tts
 
  py -3.9-64 -m pip install python-espeak-ng
  
  https://www.youtube.com/watch?v=Yglxf2WbkLU 
  https://youtu.be/zRaDe08cUIk
  create a python environement     py 3.9-64 -m venv .foldername
  
  on windows 
  
  scripts\activate
  
  Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
  
   tts-server  --model_name tts_models/en/ljspeech/neural_hmm               --vocoder_name    vocoder_models/en/sam/hifigan_v2
 
log 12: dnb tutorial

https://bedroomproducersblog.com/2021/12/24/drop-designer/
https://www.modalics.com/products   EoN free
https://www.edmprod.com/how-to-make-drum-and-bass/



log 10:


-log8
*orca ableton test
https://youtu.be/8om2uak_FKU


-log7
*free vsti beatslicer free



-log6 12/01/2023
* creation on veda
*glsl , detection of sound , video manipulation

-Log4 09/01/2023
* https://www.twitch.tv/videos/1702850185
* being present on many virtual world .
* https://www.spatial.io/s/s-Home-63bbbcc5f2513ed236ee4247
* https://www.spatial.io/s/Kreases-Lo-Fi-Room-63bbbd98f2513ed236ee43b9?share=8948516013531468169

> pip install pyworld==0.3.0

tts_models/en/ljspeech/neural_hmm : work  



- Log3 08/01/2023
* Orca ableton
* https://soundcloud.com/kreasevision-dump/gods    

- vsti:
* keiratune/Synth1/TRipleCheese  (free)

* vst: Deelay (free)
