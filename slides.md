# Productivity
Brian Besmanoff

:octocat: [bbesmanoff/productivity-talk][repo]

---

# What is "Productivity"?

---

# What is "Productivity"?

> the quality, state, or fact of being able to generate, create, enhance, or
> bring forth goods and services

> http://dictionary.reference.com/browse/productivity

---

# What is "Developer Productivity"?

---

# What isn't "Developer Productivity"?

> “Measuring programming progress by lines of code is like measuring aircraft
> building progress by weight.”
>
> -- Bill Gates

---

## A Quick Story

http://www.folklore.org/StoryView.py?story=Negative\_2000\_Lines\_Of\_Code.txt

---

# What is Developer Productivity?

---

# What is Developer Productivity?
* Getting work done *quickly*

---

# What is Developer Productivity?
* Getting work done *quickly*
* Getting work done *efficiently*

---

# What is Developer Productivity?
* Getting work done *quickly*
* Getting work done *efficiently*
* Getting work done *effectively*

---

# What is This Talk?

---

# What is This Talk?
Tips and tricks for acheiving productivity  

---

![The Pragmatic Programmer][prag_prog_cover]

---

## Inspiration

http://exercism.io/

@r00k: [Increasing Developer Productivity][bens_talk]

---

## Disclaimer:
### Your Results may Vary

---

# Let's Get Started

---

# General Workflow

---

## Keep your Hands Where I can see Them

---

## Keep your Hands Where I can see Them
(home row)

---

### Find tools that help you do this
Window managers for throwing around windows  
Alternative key bindings for applications  
Plugins to existing applications

---

## Practice Typing

---

## Practice Typing
http://play.typeracer.com

---

## Stand Up

---

## Stand Up
Healthy  
Keeps you moving

---

## But I don't have spare $X00 for a desk...

---

## Make one
![Jack Stand Desk][jack_stand]

---

## Stand Up

![Standing Desk][standing_desk]

---

## Use a Similar Toolchain

---

## Making a slideshow?
I :heart: git, vim, and Markdown

I :broken_heart: leaving those things

---

## Making a slideshow?

How can I combine these things?

---

## Making a slideshow?

@jedcn / [reveal-ck][reveal-ck]

---

# Terminal

---

## Know your weaknesses

---

## Know your weaknesses
Alias Everything

---

```bash
ls
vim RsaDecrypt.java
c
ga .
gc
c
ls
vim Triplets.java
c
ls
rm Triplets.java
vim Triplet.java
c
ls
vim RsaDecrypt.java
curl -O http://www.cs.rit.edu/\~ark/462/p4/in.txt
make
java RsaDecrypt in.txt
curl -O http://www.cs.rit.edu/\~ark/462/p4/in.txt
make
java RsaDecrypt in.txt
make
java RsaDecrypt in.txt
histor
history
```

---

## An Example

```bash
alias ackp='ack --pager="less -R"'
alias agp='ag --pager="less -R"'
alias b='bundle'
alias c='clear'
alias g='git'
alias ga='git add'
alias gap='git add --patch'
alias gb='git branch'
alias gbv='git branch -v'
alias gc='git commit'
alias gca='git commit --amend'
alias gcl='git clean'
alias gclfd='git clean -f -d'
alias gco='git checkout'
alias gcob='git checkout -b'
alias gd='git diff'
alias gdc='git diff --cached'
alias gf='git fetch --all'
alias gg='git log --graph --decorate'
alias git_root='cd $(git rev-parse --show-toplevel) || cd .'
alias gl='git log'
alias gm='git merge --no-ff'
alias gml='git merge --log --no-ff'
alias gp='git push'
alias gpo='git push origin'
alias gr='git reset'
alias greb='git rebase'
alias gref='git reflog'
alias grem='git remote -v'
alias grh='git reset --hard'
alias gs='git status'
alias gst='git stash'
alias gstp='git stash pop'
alias ivm='vim' # I've done this too many times recently
alias l='ls -alh'
alias topten='print -l -- ${(o)history%% *} | uniq -c | sort -nr | head -n 10'
alias v='vagrant'
alias vdvu='vagrant destroy -f && vagrant up'
alias x='exit'
```

---

## Embrace the Multiplex

---

## Embrace the Multiplex
`tmux`, `screen`

---

### Plugins Work Even Better
`tmuxifier`

---

### Plugins Work Even Better

![tmuxifier example][tmuxifier]

---

### Bonus: Co-Workers Can't Mess With You

---

## Play with `$PS1`

---

## Play with `$PS1`
It's always there  

Make it work for you

---

## Play with `$PS1`

%B$PREFIX %2~ $(custom\_git\_prompt)%{$M%}%B»%b%{$RESET%} 

---

# Text Editors

---

# Text Editors
## (without starting a holy war)

---

## Embrace Macros

---

## Record Repeated Keystokes

A collection of `<li>`'s commented out per item

---

## Record Repeated Keystokes

A collection of `<li>`'s commented out per item

In vim, `^dW$BhD` can do this

---

## But Recorded...

---

## But Recorded...

`@q` from anywhere on the line



[repo]: https://github.com/bbesmanoff/productivity-talk
[prag_prog_cover]: /images/prag_prog.jpg
[jack_stand]: /images/rig.jpg
[standing_desk]: /images/standing_desk.gif
[tmuxifier]: /images/tmuxifier.png
[bens_talk]: http://original.livestream.com/e4egroundfloor2/video?clipId=pla_de7943c3-3829-4242-8a6a-5cf989227c99
[reveal-ck]: https://github.com/jedcn/reveal-ck
