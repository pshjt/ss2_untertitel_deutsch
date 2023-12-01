########################
#SS2 Untertitel Deutsch#
########################

Diese Mod fügt System Shock 2 deutsche Untertitel hinzu. Die Untertitel stehen dabei sowohl für die offizielle deutsche Übersetzung als auch das Shock Community Project (https://www.systemshock.org/index.php?topic=7116.0) bereit.

Das Timing der Untertitel entspricht der offiziellen deutschen Audioausgabe.


Anwendung
1. Patche deine SS2-Installation mit SS2Tool (https://www.systemshock.org/index.php?topic=4141.0). Dabei sollte die Option "Game Options" -> "Enable subtitle support" aktiviert sein.
2. Aktiviere diese Mod im Mod-Manager (siehe https://pshjt.github.io/dmm/).


Troubleshooting
# Ich kann keine Untertitel sehen.
--> Stelle sicher, dass die Mod aktiviert ist und Untertitel verfügbar sind. In der cam_ext.cfg sollte am Ende folgender Eintrag auftauchen:
	enable_subtitles
	; subtitles_hide_types movie+player+convo+bark+nonverbal
	subtitles_hide_types nonverbal
	subtitles_dim 20 80 86
	subtitles_font_dir fonts\
	subtitles_font_name mainaa
	subtitles_spacing 1
	;subtitles_bg_color 0 0 0 0
	subtitles_show_descr
	subtitles_max_dist_bark 50
	subtitles_extra_time 800
 
# Ich möchte Untertitel vom Typ "X" entfernen.
--> Ändere die Zeile beginnend mit "subtitles_hide_types" in cam_ext.cfg. Um z.B. Geräusche und Gegnerkommentare zu entfernen, würde die Zeile "subtitles_hide_types bark+nonverbal" lauten. Siehe auch die Dokumentation in docs\newdark\subtitles.txt.

# Ich habe ein ungeklärts Problem - Hilfe!
--> Support gibt es auf SystemShock.org: https://www.systemshock.org/index.php?topic=8395
