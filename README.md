# writeups aka me writing logs for myself

# 4-3-25:
Was told to look into portals, Clipboard, Screenshot,Settings,Notification. 

From my understanding Clipboard portal is used mainly for RemoteDesktops and not for everyday casual use, which brings me to keep the dev on this backend to hold. Only GNOME has implemented a backend for it, that too it was in 2022, so if such a portal was added such recently, i dont think Clipboard portal is such an essential portal to be implemented in our preliminary phase.

https://gitlab.gnome.org/GNOME/xdg-desktop-portal-gnome/-/merge_requests/53

Screenshot portal could be integrated easily with the help of the crate wayshot, which is built by waycrate. https://github.com/waycrate/wayshot

Settings portal by default has only color-scheme, accent, contrast values within them to be transfered to relevent app, if they need these data. So we need to find some other values too that could be provided via this portal, start implementing.

Notification portal could be considered as the most needed portal of the four, even though there is gui code in our repo, notifications backend can be made our own, even though the code for a notification portal is lengthy, i think with time anything is possible.
