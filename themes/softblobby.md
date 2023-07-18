<br>

예쁜 유니콘 🦄 테마 !! <a href="https://github.com/gsalami00/softblobby">softblobby</a><br><br>
===
<br>
<ol>
  <li><code>우분투 창 열기</code></li><br>
  <li><pre><code>git clone https://github.com/gsalami00/softblobby</code></pre></li>
  <li><pre><code>cp softblobby/softblobby.zsh-theme ~/.oh-my-zsh/themes/</code></pre></li>
  <li><pre><code>vi ~/.zshrc</code></pre></li>
  <li><code>ZSH_THEME="softblobby" 로 수정</code></li><br>
  <li><pre><code>source ~/.zshrc</code></pre></li>
 </ol>
<br><br><br>

이모티콘 바꾸기&nbsp;&nbsp;&nbsp;<code>💡이모티콘 너무 큰걸로 바꾸면 대참사 날 수도 있음!</code>
---
<ol>
  <li><pre><code>vi ~/.oh-my-zsh/themes/softblobby.zsh-theme</code></pre></li>
  <li><pre><code>source ~/.zshrc</code></pre><br></li>
</ol>
<br>

색상 바꾸기
---
```shell
vi ~/.oh-my-zsh/themes/softblobby.zsh-theme
```
```shell
echo '%F{225}%K{212}╭ <이모티콘>  %D{%b %e %a}.%t  %f%k%F{212}%K{000}\ue0b0%f%k'
```
* 여기에서 ```%F{원하는폰트색상}```, ```%K{원하는배경색상}```임.
* 같은 줄의 다른 ```%F{ }```, ```%K{ }``` 같은 경우, ```%F{앞선배경색상}```, ```%K{다음배경색상}```으로 설정하면 됨.<br><br>

<pre><b>참고</b>🍎 {000}은 아무 색상에 해당하지 않는 투명임</pre>
<br>
<br>

## 1. 2023.07.03.

<img src="https://github.com/redzzzi/THEME/assets/127263392/6f6eaeaf-1fce-4d95-ac74-a83d1f661dd0" width="500px">

<details>
<summary>코드</summary>
<div markdown="1">

```shell
ZSH_THEME_GIT_PROMPT_PREFIX=""
ZSH_THEME_GIT_PROMPT_SUFFIX=""
ZSH_THEME_GIT_PROMPT_DIRTY=""
ZSH_THEME_GIT_PROMPT_CLEAN=""

PROMPT='$(now)$(username)$(directory)$(git_info)%f%k
╰→  '

now () {
    echo '%F{225}%K{212}╭ 🐇  %D{%b %e %a}.%t  %f%k%F{000}%K{000}\ue0b0%f%k'
}

username() {
    echo '%F{212}%K{225}  🌷  %B%n%b   %f%k%F{000}%K{000}\ue0b0%f%k'
}

directory () {
    echo '%F{208}%K{000}  🍀  %0~  %f%k'
}

git_info () {
    GIT_INFO="$(git_prompt_info)"
    if [[ $GIT_INFO == "" ]] then
        echo "%F{000}%K{000}\ue0b0%f%k"
    else
        echo "%F{000}%K{000}\ue0b0%f%k%F{234}%K{147}  🍎   $(git_prompt_info)  %F{000}%K{000}\ue0b0%f%k"
    fi
}
```

</div>
</details>


## 2.

<img src="https://github.com/redzzzi/THEME/assets/127263392/af6994a3-52ef-4bb8-bba0-fc0fa8d42786" width="500px">

<details>
<summary>코드</summary>
<div markdown="1">

```shell
ZSH_THEME_GIT_PROMPT_PREFIX=""
ZSH_THEME_GIT_PROMPT_SUFFIX=""
ZSH_THEME_GIT_PROMPT_DIRTY=""
ZSH_THEME_GIT_PROMPT_CLEAN=""

PROMPT='$(now)$(username)$(directory)$(git_info)%f%k
╰→  '

now () {
    echo '%F{225}%K{212}╭ 🐇  %D{%b %e %a}.%t  %f%k%F{000}%K{000}\ue0b0%f%k'
}

username() {
    echo '%F{212}%K{225}  🌷  %B%n%b   %f%k%F{000}%K{000}\ue0b0%f%k'
}

directory () {
    echo '%F{#DF8EFF}%K{#fcf0ff}  🫧  %0~  %f%k'
}

git_info () {
    GIT_INFO="$(git_prompt_info)"
    if [[ $GIT_INFO == "" ]] then
        echo "%F{#fcf0ff}%K{#fcf0ff}\ue0b0%f%k"
    else
        echo "%F{000}%K{000}\ue0b0%f%k%F{#F0F8FF}%K{#c49adb}  💜   $(git_prompt_info)  %F{000}%K{000}\ue0b0%f%k"
    fi
}
```

</div>
</details>
