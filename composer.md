
cara baca version package yg diperlukan
![cara baca version yg diperlukan](https://github.com/taqinasirr/kod/assets/21170527/facbb71a-81e2-492b-bc45-c7c175a8f2bb)


## composer install vs composer update

### composer install

1. If `composer.lock` exist.
   * Process and installs dependencies from the composer.lock file.
  
<br>

2. If `composer.lock` does not exist.
   * Process package installs from composer.json.
   * Creates the composer.lock file based on the installed packages.
  

### composer update
1. Processes dependencies from the composer.json file (installs, updates and removes).
2. Creates or updates the composer.lock file according to the changes.

<br><br>

> senang cerita:  
> composer install - install dependencies kat composer.lock  
> composer update - install dependencies (versi latest) kat composer.json.  pastu update versi latest tu kat composer.lock

<br>

---

<br><br>
fungsi composer.lock
* supaya bila kita share project kita, org lain akan install packages versi yg sama.
* so org tu boleh run project kita tanpa masalah packages n dependencies yg x sama version.
