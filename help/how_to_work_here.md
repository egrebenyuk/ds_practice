## How to work here

---

This help page shows easy steps to fork and start to work with this repository. Detailed instractions how to fork page you can find <a href="https://help.github.com/articles/fork-a-repo/">here</a>. Also, go <a href="https://github.com/jojo1317/Git-quick-reference-for-beginners">here</a> and find Git quick reference for beginners. And go <a href="https://guides.github.com/">here</a> if you want to dig deeper. 


### Fork repo:
<ul>
  <li>On GitHub, navigate to repo and push fork button.</li>
  <li><code>git clone https://github.com/YOUR-USERNAME/ds_practice</code></li>
  <li><code>git remote -v</code></li>
  <li><code>git remote add upstream https://github.com/egrebenyuk/ds_practice.git</code></li>
  <li><code>git remote -v</code></li>
  <li><code>git fetch upstream</code></li>
</ul>


### Get updates from forked repo:
<ul>
  <li><code>git fetch upstream</code></li>
  <li><code>git checkout master</code></li>
  <li><code>git merge upstream/master</code></li>
</ul>  


### Push changes to github:
<ul>
  <li><code>git push origin master</code></li>
</ul>
