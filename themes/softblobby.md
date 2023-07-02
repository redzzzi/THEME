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
