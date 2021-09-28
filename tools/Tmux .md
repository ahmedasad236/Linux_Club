# Tmux

**What is tmux?**

Tmux is a terminal multiplexer which enables a number of terminals to be created, accessed, and controlled from a single screen, this is called tmux session.Tmux sessions are persistent, so it means that tmux will continue to run in the background even if you get disconnected.

With Tmux you can easily switch between multiple programs in one terminal, detach them and reattach them to a different terminal.

**How to install tmux on linux?**

On Ubntu & Debian:

    sudo apt-get install tmux

On Arch:

    sudo pacman -S tmux --noconfirm

**How to use tmux ?**

   Starting a tmux session:

     $ tmux

   Creating a named tmux session:

     $ tmux new -s session_name

   Detaching from tmux session (returning back to shell):

     Ctrl+b d

   listing all tmux sessions:

     $ tmux ls

   attaching to a tmux session:

     $ tmux attach-session -t session_number

   useful commands:

      Ctrl+b ?    get a list of all commands

      Ctrl+b c    create a new window 
      Ctrl+b w    choose window from a list 
      Ctrl+b ,    rename the current window 
      Ctrl+b %    split current pane horizontally into two panes

      Ctrl+b "    split current pane vertically into two panes

      Ctrl+b o    go to the next pane

      Ctrl+b ;    toggle between the current and previous pane

      Ctrl+b x    close the current pane
