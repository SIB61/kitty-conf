// mapping.conf 

map f5 launch --location=hsplit
map f6 launch --location=vsplit
map f4 launch --location=split
map f7 layout_action rotate

# Move the active window in the indicated direction
map shift+up move_window up
map shift+left move_window left
map shift+right move_window right
map shift+down move_window down

# Switch focus to the neighboring window in the indicated direction
map ctrl+left neighboring_window left
map ctrl+right neighboring_window right
map ctrl+up neighboring_window up
map ctrl+down neighboring_window down

# Resizing windows
map ctrl+shift+left resize_window narrower
map ctrl+shift+right resize_window wider
map ctrl+shift+up resize_window taller
map ctrl+shift+down resize_window shorter 3
# reset all windows in the tab to default sizes
map ctrl+shift+home resize_window reset



// kitty.conf 

# BEGIN_KITTY_THEME
# GitHub Dark
include current-theme.conf
# END_KITTY_THEME

font_family       Fira Code
bold_font         Source Code Pro
italic_font       auto
bold_italic_font  auto
font_size         13.0

disable_ligatures never
#: Cursor colors
enabled_layouts splits
include mapping.conf
cursor #58a6ff
linux_display_server x11


// current-theme.conf

# vim:ft=kitty

## name: GitHub Dark
## author: GitHub
## license: MIT

#: The basic colors

foreground #c9d1d9
background #0C0C0C
selection_foreground #0d1117
selection_background #58a6ff

#:font



#: Tab bar colors

tab_bar_background #010409
active_tab_foreground #c9d1d9
active_tab_background #0d1117
inactive_tab_foreground #8b949e
inactive_tab_background #010409


#: The basic 16 colors

#: black
color0 #484f58
color8 #6e7681

#: red
color1 #ff7b72
color9 #ffa198

#: green
color2 #3fb950
color10 #56d364

#: yellow
color3 #d29922
color11 #e3b341

#: blue
color4 #58a6ff
color12 #79c0ff

#: magenta
color5 #bc8cff
color13 #d2a8ff

#: cyan
color6 #39c5cf
color14 #56d4dd

#: white
color7 #b1bac4
color15 #ffffff




