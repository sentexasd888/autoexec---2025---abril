fps_max 301


mat_setvideomode 1920 1080 1
mat_setvideomode 1920 1080 0




// Font

reloadfont "mat_setvideomode 1920 1080 1; mat_setvideomode 1920 1080 0"

reloadfont






net_graphheight 60 - change height
net_graphproportionalfont 1 - change size
net_graphpos 330 - change position



sensitivity 1.8




mat_monitorgamma 1.6


mat_monitorgamma_tv_enabled 1


fov_desired 90.480003




alias views_65 "echo " 65 viewmodelfovsurvivor ";cl_viewmodelfovsurvivor 65 ;alias changeview views_105"
alias views_105 "echo " 105 viewmodelfovsurvivor ";cl_viewmodelfovsurvivor 105 ;alias changeview views_65"
alias changeview "views_105"
bind "F3" "changeview"




bind "F4" "cl_viewmodelfovsurvivor 180"





bind "DOWNARROW" "cl_crosshair_dynamic 0"

bind "LEFTARROW" "cl_crosshair_dynamic 1"

bind "F8" "toggleconsole"

bind "F9" "openserverbrowser"    // F9 Buscador de servidores.

bind f10 disconnect

bind "Mouse5" "say_team !tank"

bind "Mouse4" "say_team !mvp"

bind "o" "say_team !bonus"

bind "u" "say_team Go Go Go!"

bind "i" "say_team >HELP<"







bind tab "+showscores_custom"
alias "+showscores_custom" "+showscores;net_graph 3";
alias "-showscores_custom" "-showscores;net_graph 1";





//NETWORKING
cl_updaterate           "100"       //Number of packets per second of updates you are requesting from the server
cl_cmdrate          "100"       //Max number of command packets sent to server per second
rate                "100000"    //Max bytes/sec the host can receive data  
cl_interp           "0"     //Interpolate object positions starting this many seconds in past
cl_interp_ratio         "-1"        //Sets the interpolation amount (final amount is cl_interp_ratio / cl_updaterate)
cl_lagcompensation      "1"     //Perform server side lag compensation of weapon firing events.
cl_resend           "1.5"       //Delay in seconds before the client will resend the 'connect' attempt
cl_timeout          "20"        //After this many seconds without receiving a packet from the server, the client will disconnect itself
net_allow_multicast     "0"
sv_region           "3"     //The region of the world to report this server in.
net_splitpacket_maxrate     "30000"     //Max bytes per second when queueing splitpacket chunks
net_splitrate           "3"     //Number of fragments for a splitpacket that can be sent per frame
net_maxroutable         "1200"      //Requested max packet size before packets are split.








// Default Crosshair

cl_crosshair_alpha 255
cl_crosshair_blue 220
cl_crosshair_dynamic 1
cl_crosshair_green 182
cl_crosshair_red 138 
cl_crosshair_thickness 2











//Glows - Learning

 "Supervivientes (Survivor) - Color Azul Tono Claro"

cl_glow_survivor_b 1
cl_glow_survivor_g 0.2
cl_glow_survivor_r 0

  "Infectado de agarre cogiendo al superviviente, Hunter,Jockey,Charger(Survivor) - Color Violeta"

cl_glow_ability_b 1
cl_glow_ability_r 0.5
cl_glow_ability_g 0

  "Superviviente Incapacitado o cogido por infectado (Survivor) - Color Rojo"

cl_glow_survivor_hurt_r 1
cl_glow_survivor_hurt_g 0
cl_glow_survivor_hurt_b 0
 
 "Objetos de cerca(survivor) - Color Azul"

cl_glow_item_b 1
cl_glow_item_g 0
cl_glow_item_r 0

 "Objetos de Distancia(survivor) - Purpura" 

cl_glow_item_far_b 1
cl_glow_item_far_g 0
cl_glow_item_far_r 1

 "Superviviente vomitado (Survivor) - Color Verde Tono Claro"

cl_glow_survivor_vomit_r 0
cl_glow_survivor_vomit_g 1
cl_glow_survivor_vomit_b 0.2
 
 "Superviviente vomitado (Infected) - Color Verde Transparente"

cl_glow_infected_vomit_r 0.2
cl_glow_infected_vomit_g 1
cl_glow_infected_vomit_b 0.5
 
 "Infectado regenerado (Infected) - Color Morado"

cl_glow_infected_g 0
cl_glow_infected_b 1
cl_glow_infected_r 0.2
 
 "Infectado fantasma (Infected) - Color Celeste"

cl_glow_ghost_infected_b 1
cl_glow_ghost_infected_g 1
cl_glow_ghost_infected_r 0

 "Superviviente con salud Alta (Infected) - Color Verde"

cl_glow_survivor_health_high_g 1
cl_glow_survivor_health_high_b 0
cl_glow_survivor_health_high_r 0

 "Superviviente con salud Media (Infected) - Color Amarillo

cl_glow_survivor_health_med_b 0
cl_glow_survivor_health_med_g 1
cl_glow_survivor_health_med_r 1

 "Superviviente con salud baja(Infected) - Color Naranja"

cl_glow_survivor_health_low_b 0
cl_glow_survivor_health_low_r 1
cl_glow_survivor_health_low_g 0.2

 "Superviviente con salud Critica(Infected) - Color Rosado"

cl_glow_survivor_health_crit_b 0.2
cl_glow_survivor_health_crit_g 0
cl_glow_survivor_health_crit_r 1

 "Objetos de Tank(Infected) y Objetos estando en blanco y negro(Survivor) - Color Verde Limon"

cl_glow_thirdstrike_item_r 0.4
cl_glow_thirdstrike_item_g 1
cl_glow_thirdstrike_item_b 0

 "Parpadeo cuando desangra(Infected)"

cl_glow_survivor_health_bleed_pulse 1
cl_glow_survivor_health_bleed_pulse_amount 1
cl_glow_survivor_health_bleed_pulse_speed 50
cl_glow_survivor_health_include_buffer 1












//BunnyHop Scroll

bind "MWHEELUP" "+jump"
bind "MWHEELDOWN" "+jump"
bind "SPACE" "+jump"







//IMPUT LAG KEYS//

bind w +mfwd
bind s +mback
bind a +mleft
bind d +mright
bind "e" "+use"
bind "MOUSE1" "+attack"
bind "MOUSE2" "+attack2"


alias +mfwd "-back;+forward;alias checkfwd +forward"
alias +mback "-forward;+back;alias checkback +back"
alias +mleft "-moveright;+moveleft;alias checkleft +moveleft"
alias +mright "-moveleft;+moveright;alias checkright +moveright"
alias -mfwd "-forward;checkback;alias checkfwd;"
alias -mback "-back;checkfwd;alias checkback;"
alias -mleft "-moveleft;checkright;alias checkleft;"
alias -mright "-moveright;checkleft;alias checkright;"
alias checkfwd; 
alias checkback; 
alias checkleft; 
alias checkright;







