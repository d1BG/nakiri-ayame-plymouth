# nakiri-ayame-plymouth
Nakiri Ayame's start stream animation as boot splash (cut ver.)


git clone repo into:
`/usr/share/plymouth/themes/`

run this to set it as ur bootsplash:
`sudo plymouth-set-default-theme -R nakiri-ayame-plymouth`

add `quiet splash` to kernel parameters


if booting is too fast to see the whole animation, you can edit 
`/usr/lib/systemd/system/plymouth-quit.service`
and add 
`ExecStartPre=/usr/bin/sleep 10` (10 or however many secound u wanna delay the boot)
to the `[Service]` category in this file: 
`/usr/lib/systemd/system/plymouth-quit.service`
