Packaging Python Projects in 2023 demo
======================================

This is a demo project used in my presentation on pykonik meetup.

[Presentation slides](https://docs.google.com/presentation/d/1cSwpH_iNzyoa2HVrWqeVpnyIqHcPX0skfU2Cqe0W08k/edit?usp=sharing)
[Recording](https://youtu.be/o4bNyhbLWnw?t=5443)

Each commit in this repository is a single "step" from my demo. There are also 2 additional branches with a quick demo 
of setuptools-scm and poetry-dynamic-versioning (named accordingly)

If you're interested, I've used those 2 aliases to jump between commits in my presentation (note it only works on main branch):


    alias n='git reset --hard && git clean -fd . && git checkout $(git rev-list --topo-order HEAD..main | tail -1) && clear'
    alias p="git reset --hard && git clean -fd . && git checkout HEAD~1 && clear"

(note: aliases are fixed, on themo I was missing the `git reset --hard` part)

In the left pane I just had a loop of tree command with a 1s sleep time to show the project structure:

    while true; do clear; tree; sleep 1; done
