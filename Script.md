
// Toggle key
alias toggle_autojump "autojump_on"
bind INS toggle_autojump

// Enable autojump
alias autojump_on "bind space +ajump; alias toggle_autojump autojump_off; echo AutoJump ON"

// Disable autojump
alias autojump_off "bind space +jump; alias toggle_autojump autojump_on; echo AutoJump OFF"

// Main jump logic
alias +ajump "+jump; alias ajump3; alias autoj1 autoj; hjump1; wait 16; ajump"
alias -ajump "-jump; alias ajump1 alias ajump1 autoj; alias autoj1; ajump3; hjump"

alias ajump "ajump1; ajump2"
alias ajump2 "alias ajump3 ajump1"
alias ajump1 "autoj"
alias autoj "+jump; wait 4; -jump; wait 3; autoj1"
alias autoj1 "autoj"

alias hjump "alias hjump4 hjump3; hjump3; wait 15; alias hjump1; alias hjump4"
alias hjump3 "alias hjump1 hjump2; wait 1; hjump4"
alias hjump2 "alias ajump1 alias ajump1 autoj"

// This confirms bhop Script is active
echo
echo
echo ! ! ! ! ! bhop Script is active ! ! ! ! !
echo
echo ! ! ! ! ! bhop Script is active ! ! ! ! !
echo
echo
