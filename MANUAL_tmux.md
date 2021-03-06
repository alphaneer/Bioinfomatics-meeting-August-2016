#Tmux
Tmux is a **terminal multiplexer**. It allow you to run multiple *panels* in a single *window* (read: tab), that are organized by named *sessions* (read: browser window). Sessions run in the background (like &), so you can run (several) jobs without fear of disconnection.

Here is an example of a window with three panes.

![tmux image 1](https://github.com/Xevkin/Bioinfomatics-meeting-August-2016/blob/master/tmux_1.png)

Tmux operates using shortcuts (there are also long, more explicit commands). If I wanted to create a new window in this session, I input **ctrl-B** and then **C**. **ctrl-B** is the default shortcut combination.

![tmux image 2](https://github.com/Xevkin/Bioinfomatics-meeting-August-2016/blob/master/tmux_2.png)

Say I want to leave tmux and see what other tmux sessions I have running. First I detach the session by pressing **ctrl+B** then **D**. Outside of tmux, I can type **tmux ls** to list all the sessions I have runnning.

![tmux image 3](https://github.com/Xevkin/Bioinfomatics-meeting-August-2016/blob/master/tmux_3.png)

I can then attach whichever session I choose. For example, if I want to see my msmc session: **tmux att -t msmc**.

##Shortcuts
Shortcuts are indispensible when using tmux. All shortcuts are preceded by a prefix (default ctrl and B together).

![tmux image 4](https://github.com/Xevkin/Bioinfomatics-meeting-August-2016/blob/master/tmux-cheatsheet.png)


##Plug-ins
You can also modify your installation of tmux using plugins - use the tmux plugin manager https://github.com/tmux-plugins/tpm to simplify this. An example of a tmux plugin: tmux-resurrect, which allows you to restore a session during a system restart. https://github.com/tmux-plugins/tmux-resurrect
